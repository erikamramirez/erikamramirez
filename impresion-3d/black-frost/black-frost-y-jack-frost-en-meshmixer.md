# Black Frost y Jack Frost en Meshmixer

### **Make Solid**

"**Make Solid**" en **Meshmixer** es una función que permite convertir un modelo 3D en malla en una estructura sólida. Esto es útil cuando tienes un objeto que está compuesto por una serie de triángulos o polígonos y deseas convertirlo en un objeto sólido que se puede imprimir en 3D o trabajar con él de otras formas.

{% embed url="https://www.youtube.com/watch?v=RpLSGyt5JQA" %}

### Cómo funciona Make Solid

"**Make Solid**" es una herramienta poderosa que se puede utilizar en muchas situaciones, pero realmente ayuda entender cómo funciona.

&#x20;Lo que hace internamente "**Make Solid**" es crear una aproximación de tu forma de entrada utilizando una gran cantidad de pequeños cubos conocidos como voxels.&#x20;

Esta representación nos permite crear un sólido inequívoco a partir de cualquier entrada que envíes. Puede que no sea el sólido que tenías en mente, pero será un sólido.

Una vez que tenemos la representación de voxels, podemos realizar varias acciones para convertirla en una mejor aproximación de tu forma de entrada. Sin embargo, siempre es una aproximación. Al igual que los píxeles en una imagen, estos pequeños bloques tienen una resolución fija.&#x20;

**Los detalles más pequeños que unos pocos bloques es probable que se pierdan, pueden aparecer agujeros en regiones más delgadas que dos bloques y los bordes afilados probablemente se suavicen.**

&#x20;Puedes mejorar la situación **reduciendo el tamaño de los bloques** en **block size,** con un costo computacional adicional.

El uso más evidente de "**Make Solid**" es que puedes introducir cualquier conjunto de capas superpuestas y obtener una sola malla no auto-intersectante adecuada para la impresión en 3D.

&#x20;Hay otros usos, como se describe a continuación. Sin embargo, ten en cuenta que si envías partes ambiguas, como mallas con agujeros, conjuntos coincidentes de triángulos o geometría no-manifold, los resultados pueden no ser los que esperabas.

<details>

<summary>Cálculo no Automático en Make Solid</summary>

A diferencia de muchas herramientas en Meshmixer, la vista previa en la herramienta "**Make Solid**" no se recalcula automáticamente al cambiar los parámetros. En algunos casos, esta herramienta puede tardar bastante tiempo en calcularse, por lo que para iniciar una nueva vista previa, debes hacer clic en el botón "**Update**".

&#x20;En la mayoría de los casos, verás una barra de progreso con un botón de **Cancel**, sin embargo, la cancelación no es instantánea, en casos extremos puede tardar uno o dos minutos después de hacer clic en el botón de cancelar para que tenga efecto.

</details>

<details>

<summary>Control Deslizante</summary>

Ten en cuenta que, para las configuraciones de **Solid Accuracy** y **Mesh Density Settings**, se muestra una opción de Tamaño de Celda debajo del control deslizante.

&#x20;Cada uno de estos controles deslizantes especifica una **tasa de muestreo para la superficie**, esencialmente una cantidad de "pasos" en los que se divide el objeto.

&#x20;**Números más altos significan resultados más precisos a expensas de una computación más lenta** y, en el caso de la **Densidad de Malla**, significativamente **más triángulos.**&#x20;

Para un uso ocasional, los controles deslizantes son suficientes, pero si necesitas resultados repetibles, las casillas de Tamaño de Celda, que son editables si haces clic en ellas, son una forma más precisa de definir el tamaño de paso de subdivisión.

</details>

> Los controles deslizantes de Offset Distance y Min Thickness solo están disponibles cuando el Tipo de Sólido está configurado como "Preciso". Detalles a continuación.

<details>

<summary>Qué pasa al seleccionar Accept.</summary>

Cuando aceptas una operación de Crear Sólido, no modificamos el objeto de entrada. En su lugar, el sólido se agrega a la escena como un nuevo objeto de Malla, con "(sólido)" agregado al nombre original del objeto. El objeto original también se oculta, pero puedes volver a mostrarlo en el Explorador de Objetos.

</details>



### Para utilizar la función "**Make Solid**" en **Meshmixer**, sigue estos pasos:

* Abre Meshmixer y carga el modelo 3D que deseas convertir en sólido.

<figure><img src="../../.gitbook/assets/Captura de pantalla 2023-11-06 145602.png" alt=""><figcaption></figcaption></figure>

* Selecciona el modelo haciendo clic en él.



* En la barra lateral izquierda, selecciona la pestaña "Edit".
* Aparecerán varias opciones, entre las cuales encontrarás "Make Solid". Haz clic en esa opción.

En las ventanas desplegables se encuentra información recopilada del manual de Meshmixer para entender mejor las configuraciones

<details>

<summary><mark style="color:purple;"><strong>Solid Type</strong></mark></summary>

![](<../../.gitbook/assets/image (142).png>)

El menú desplegable Tipo de Sólido controla el comportamiento básico de la herramienta Crear Sólido. Hay cuatro modos disponibles, que se describen a continuación. La imagen a continuación muestra un ejemplo con un objeto original (izquierda) que tiene dos capas superpuestas.

<mark style="color:purple;">**Accurate:**</mark> El modo Preciso (arriba a la derecha) toma la aproximación de voxels y calcula un campo de distancias firmado que aproxima el objeto de entrada. Luego, generamos una malla basada en este campo de distancias. Calcular este campo de distancias es significativamente más costoso que el modo Rápido, y en algunos casos, el resultado puede no ser tan bueno como en el modo Rápido (como en nuestro ejemplo a continuación). Sin embargo, el campo de distancias firmado tiene otros usos, como veremos.

<mark style="color:purple;">**Blocky:**</mark> El modo de Bloque (abajo a la derecha) simplemente genera una malla a partir de los cubos de voxels, lo que da como resultado un objeto con aspecto de bloques. Ten en cuenta que a veces pueden existir intersecciones no-manifold en esta malla.

<mark style="color:purple;">**Fast:**</mark> El modo Rápido (arriba a la izquierda) es el modo predeterminado. En este modo, generamos una malla a partir de la aproximación de voxels y luego proyectamos nuevamente los vértices sobre la superficie de entrada. Esto es bastante rápido y funciona bien en casos sencillos, pero la proyección nuevamente puede introducir artefactos en áreas complejas.

<mark style="color:purple;">**Sharp Edge Preserve:**</mark> El modo de Preservación de Bordes Afilados (abajo a la izquierda) se basa en el modo Rápido, pero después de la proyección nuevamente, intentamos recuperar los bordes afilados del objeto de entrada. La forma en que se hace esto es similar al flujo de trabajo de múltiples pasos descrito en la herramienta Editar > Atraer al Objetivo. Este modo puede ser extremadamente lento y aún así no produce resultados perfectos; sin embargo, puedes resolver rápidamente pequeños defectos utilizando Atraer al Objetivo.

</details>

<details>

<summary><mark style="color:purple;"><strong>Color Transfer Mode</strong></mark></summary>

Después de haber remuestreado su malla de entrada, también podemos remuestrear los colores en esas mallas.&#x20;

Actualmente, solo admitimos colores por vértice en la malla sólida. Entonces, si su objeto de entrada tiene colores por vértice, evaluamos el color interpolado por vértice en cada vértice de la malla sólida. Esto se conoce como el modo Vértice a Vértice.&#x20;

Si su objeto de entrada tiene texturas mapeadas por UV, entonces el modo Material a Vértice resultará en que el mapa de color se "cueza" en los colores por vértice en la malla sólida. Se muestra un ejemplo a continuación. La imagen más a la izquierda muestra la malla original texturizada (con muchos agujeros).&#x20;

El del medio es el resultado predeterminado de Crear Sólido. Puede ver muchos artefactos en la camiseta porque la densidad de vértices es bastante baja en comparación con la resolución de la textura. En la imagen más a la derecha, hemos aumentado la densidad de la malla sólida para obtener una aproximación más nítida. Observe que los agujeros también se han llenado de colores.

Después de remuestrear tu malla de entrada, también podemos remuestrear los colores en esas mallas. Actualmente, solo admitimos colores por vértice en la malla sólida. Entonces, si tu objeto de entrada tiene colores por vértice, evaluamos el color interpolado por vértice en cada vértice de la malla sólida. Esto se conoce como el modo Vértice a Vértice. Si tu objeto de entrada tiene texturas mapeadas por UV, entonces el modo Material a Vértice resultará en que el mapa de color se "cueza" en los colores por vértice en la malla sólida. Se muestra un ejemplo a continuación. La imagen más a la izquierda muestra la malla texturizada original (con muchos agujeros). La del medio es el resultado predeterminado de Crear Sólido. Puedes ver muchos artefactos en la camiseta porque la densidad de vértices es bastante baja en comparación con la resolución de la textura. En la imagen más a la derecha, hemos aumentado la densidad de la malla sólida para obtener una aproximación más nítida. Observa que los agujeros también se han llenado de colores.

**No Colors:** El modo Sin Colores desactiva la transferencia de colores.![](<../../.gitbook/assets/image (143).png>)

**Automatic:** El modo Automático es el modo predeterminado. En este modo, se utiliza el modo Material a Vértice si el objeto de entrada tiene texturas mapeadas por UV; de lo contrario, se transfieren los colores por vértice.

**Vertex to Vertex:**

</details>

<details>

<summary><mark style="color:purple;"><strong>Solid Accuracy</strong></mark></summary>

Explicamos anteriormente que "Make Solid" aproxima tu objeto con voxels. Esta aproximación en realidad ocurre dos veces.&#x20;

Primero, voxelizamos la forma utilizando la Precisión Sólida como tasa de muestreo. Luego, usamos un segundo conjunto de voxels para crear una malla de la primera aproximación de voxels. La Densidad de Malla es la tasa de muestreo de esta segunda voxelización. Estas tasas de muestreo pueden ser iguales, pero no es necesario que lo sean.

El ejemplo a continuación muestra el modo Rápido con tasas de sólido/malla de 128/128, 32/128, 128/32 y 32/32.&#x20;

El efecto de reducir la Densidad de Malla es evidente: menos triángulos. Reducir la Precisión del Sólido es un poco menos evidente en este modo debido al paso de reproyección. Sin embargo, incluso en la segunda imagen, podemos ver que se pierden algunos detalles debido al sólido subyacente de baja resolución.

![](<../../.gitbook/assets/image (144).png>)

**Cells Size:**

**Mesh Density:**

</details>

<details>

<summary><mark style="color:purple;"><strong>Offset Distance</strong></mark></summary>

&#x20;Un beneficio significativo del Tipo de Sólido Preciso es que podemos calcular superficies de desplazamiento del campo de distancia firmado que hemos calculado. Esto se hace a través del control deslizante Distancia de Desplazamiento.&#x20;

**Distancias positivas resultan en capas externas** y **distancias negativas crean capas internas.** Utilizamos esta capacidad en la Herramienta Hueca.&#x20;

La precisión de la superficie de desplazamiento está en el orden del ancho de una celda.

&#x20;El desplazamiento sigue siendo un sólido sin auto-intersecciones, lo que es una ventaja sobre nuestra herramienta Editar > Desplazar basada en mallas. Sin embargo, ten en cuenta que si la Creación Sólida original ha perdido características delgadas, la superficie de desplazamiento generalmente tendrá los mismos artefactos.&#x20;

Además, solo calculamos el campo de distancia hasta donde sea necesario, por lo que los desplazamientos grandes tomarán más tiempo en encontrarse que los pequeños.

![](<../../.gitbook/assets/image (145).png>)

</details>

<details>

<summary><mark style="color:purple;"><strong>Min Thickness</strong></mark></summary>

Otra capacidad del Tipo de Sólido Preciso es que podemos intentar engrosar selectivamente regiones delgadas de la entrada utilizando la configuración de Grosor Mínimo. El ejemplo a continuación muestra un modelo de caballo que es bastante pequeño (aproximadamente 25 mm de altura). A este tamaño, las patas son muy delgadas. La imagen de la derecha es la versión Sólida con un grosor mínimo de 1.5 mm. Observa cómo las patas delgadas se han engrosado localmente, pero el cuerpo no ha sido modificado.

![](<../../.gitbook/assets/image (146).png>)

Actualmente, la forma en que logramos este engrosamiento es agregando pequeñas esferas con un diámetro establecido como el grosor mínimo. Esto desafortunadamente puede llevar a artefactos. La imagen a continuación muestra el mismo caballo pero con el Grosor Mínimo configurado en 2.0 mm. Observa cómo las patas se han vuelto bastante abultadas y redondeadas. Esto se debe, por supuesto, a las esferas que hemos agregado. Nuestro algoritmo de detección también puede fallar, como lo ha hecho en la oreja derecha del caballo anteriormente. Esta capacidad es en cierto modo un trabajo en progreso, pero podría resultar útil en algunos casos.

![](<../../.gitbook/assets/image (147).png>)

</details>

<details>

<summary><mark style="color:purple;"><strong>Cull Edge Threshole</strong></mark></summary>

La estrategia que utilizamos para generar la malla a partir de la aproximación sólida que creamos inicialmente produce mallas con muchos triángulos pequeños y delgados. El control deslizante Umbral de Eliminación de Bordes controla un proceso de postprocesamiento que descarta estos bordes diminutos. Eliminamos cualquier borde que sea una fracción de la longitud del borde del voxel. El control deslizante especifica esta fracción, siendo 100 el 25% de la longitud del borde. Ten en cuenta que esta limpieza puede introducir artefactos, especialmente en áreas muy suaves o delgadas. Puedes obtener mejores resultados configurando este valor en 0 y volviendo a generar manualmente la malla utilizando la herramienta Editar > Remesh, aunque será mucho más lento.

![](<../../.gitbook/assets/image (148).png>)

</details>

<details>

<summary><mark style="color:purple;"><strong>Close Open Boundaries</strong></mark></summary>

"Make Solid" funciona mejor con objetos de entrada que son un conjunto de capas cerradas. Sin embargo, también puedes ejecutarlo con mallas que contienen agujeros. En este caso, nuestro comportamiento predeterminado es llenar automáticamente los agujeros antes de intentar crear el sólido, utilizando el modo Mínimo de la herramienta Editar > Borrar y Rellenar. Sin embargo, en el caso especial en el que tu objeto de entrada sea un conjunto de parches de malla abiertos adyacentes, entonces cada límite del parche se tratará como un agujero y se llenará. Esto probablemente producirá resultados terribles, como se muestra en el ejemplo a continuación. En este caso, puedes desmarcar la opción "Cerrar Límites Abiertos" para omitir el paso de llenado de agujeros.

![](<../../.gitbook/assets/image (149).png>)

</details>

<details>

<summary><mark style="color:purple;"><strong>Auto Repair Result</strong></mark></summary>

El algoritmo de malla que utilizamos en "Make Solid" puede, en algunos casos, dejar agujeros pequeños y/o crear algunos bordes no-manifold. Puedes limpiarlos ejecutando el Inspector después. La opción de Reparación Automática del Resultado te ahorra el trabajo y lo hace automáticamente. Sin embargo, a veces puedes desear limpiar estos artefactos manualmente. Y, en casos raros, esta reparación automática puede ser la causa de un bloqueo. Por lo tanto, proporcionamos esta opción para desactivar el postproceso de reparación automática.

</details>

<details>

<summary><mark style="color:purple;">Transfer Groups</mark></summary>

Cuando está habilitada, la opción de Transferir Grupos intenta asignar los grupos de caras de tus objetos de entrada a la malla sólida de salida. Esto se hace de manera similar a la transferencia de color anterior. Para cada triángulo en la malla sólida, encontramos el triángulo más cercano en la malla de entrada y usamos el grupo de caras de ese triángulo. Sin embargo, debido a que los triángulos tienen formas diferentes, esto siempre generará un límite irregular en la malla sólida y, en algunos casos, triángulos desconectados del mismo grupo de caras. Puedes intentar limpiar esto utilizando la opción Seleccionar > Modificar > Suavizar Límite.

![](<../../.gitbook/assets/image (150).png>)

</details>

* Aparecerá un cuadro de diálogo con varias configuraciones. Puedes ajustar los parámetros según tus necesidades, como la resolución, el tipo de sólido y otros ajustes avanzados.

Parámetros

* Después de configurar los parámetros, haz clic en "Update" para comenzar el proceso de conversión.
* Meshmixer procesará el modelo y lo convertirá en una estructura sólida según tus especificaciones.
* Una vez que se complete el proceso, tendrás un modelo sólido que puedes guardar o seguir editando según sea necesario.

"Make Solid" es una característica poderosa que te permite transformar modelos 3D en mallas en objetos sólidos que son más adecuados para la impresión 3D u otras aplicaciones. Asegúrate de ajustar los parámetros de acuerdo a tus necesidades específicas antes de aplicar la función.
