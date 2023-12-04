# Procesado del terreno de vista satelital de Tembiaporã.

Para llevar a cabo el fresado en nuestro proyecto, utilizaremos la herramienta Terrain2stl. Esta página desempeñará un papel fundamental al convertir datos de terreno desde imágenes de vista satelital en archivos STL, permitiéndonos así crear representaciones tridimensionales precisas del relieve.

{% embed url="https://jthatch.com/Terrain2STL/" %}
Página de Terrain2STL,
{% endembed %}

Esta herramienta ya fue utilizada en proyectos anteriores, en la siguiente documentación de este Gitbook se describe su uso y los resultados.

{% content-ref url="../cnc/obtencion-de-modelo-3d-topografico/" %}
[obtencion-de-modelo-3d-topografico](../cnc/obtencion-de-modelo-3d-topografico/)
{% endcontent-ref %}

<figure><img src="../.gitbook/assets/Captura de pantalla 2023-11-29 182524.png" alt=""><figcaption><p>Vista del terreno en la interface de Terrain2STL.</p></figcaption></figure>

{% file src="../.gitbook/assets/terrain-274901.zip" %}
Archico descargable del modelo generado por Terrain2STL.
{% endfile %}

Había supuesto un buen resultado del modelo 3D generado por Terrain2STL de ser impreso en 3D por lo que lo llevé a Meshmixer para prepararlo para la impresión.

### <mark style="color:purple;">Meshmixer</mark>

<figure><img src="../.gitbook/assets/imagen_2023-12-01_095802885 (2).png" alt=""><figcaption><p>Vista del modelo de Terrain2STL en Meshmixer.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-12-01_095837673.png" alt=""><figcaption><p>Zoom de las relieves generadas por Terrain2STL.</p></figcaption></figure>

Como es mi proceso general en Meshmixer, empleo la herramienta Make Solid que se encuentra en la ventana de Edit.

<figure><img src="../.gitbook/assets/Captura de pantalla 2023-11-06 151746.png" alt=""><figcaption><p>Vista de Make Solid en la interface.</p></figcaption></figure>

Para obtener resultados óptimos en Meshmixer, se recomienda configurar los parámetros de '**Solid Type**' en '**Accurate**' y '**Solid Accuracy**' al **máximo**. Esta configuración es suficiente para asegurar una preparación adecuada del modelo.

<div>

<figure><img src="../.gitbook/assets/imagen_2023-12-01_110014750.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/imagen_2023-12-01_110047358.png" alt=""><figcaption><p>Parámetros utilizados.</p></figcaption></figure>

</div>

Seleccionar Accept al encontrarse conforme con el resultado y obtener el modelo modificado con Make Solid.

<figure><img src="../.gitbook/assets/imagen_2023-12-01_110120336.png" alt=""><figcaption></figcaption></figure>

Una vez obtenido el modelo eliminamos el archivo original y sólo mantenemos el modificado.

<div>

<figure><img src="../.gitbook/assets/imagen_2023-12-01_110239825.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/imagen_2023-12-01_110307461.png" alt=""><figcaption></figcaption></figure>

</div>

Una vez completamente editado exportamos en formato .stl para posteriormente procesarlo en Flashprint y Finalmente imprimirlo.

<div>

<figure><img src="../.gitbook/assets/imagen_2023-12-01_110345688.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/imagen_2023-12-01_110541876 (1).png" alt=""><figcaption></figcaption></figure>

</div>

{% file src="../.gitbook/assets/Tembiapora t2stl.stl" %}
Archivo descargable del proceso en Meshmixer.
{% endfile %}

### <mark style="color:purple;">Flashprint</mark>&#x20;

A continuación se detallará el proceso realizado en Flashprint

Importa el archivo en Flashprint y procede a ajustar la escala según sea necesario. En este caso, no es preciso utilizar soportes, ya que se trata de una placa plana prismática.

<figure><img src="../.gitbook/assets/imagen_2023-12-01_112002495.png" alt=""><figcaption><p>Archivo abierto en la interface de Flashprint.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-12-01_112208740.png" alt=""><figcaption><p>Dimensiones impresas.</p></figcaption></figure>

Para ajustar los parámetros de impresión, seleccionamos 'Iniciar Corte', ubicado en el centro de la parte superior.

<figure><img src="../.gitbook/assets/imagen_2023-12-01_112603135.png" alt=""><figcaption><p>ícono de iniciar corte.</p></figcaption></figure>

A continuación se observa los parámetros de Temperatura de la extrusora derecha y la plataforma en la ventana de **Impresora**.

<figure><img src="../.gitbook/assets/imagen_2023-12-01_112631178.png" alt=""><figcaption><p>Vista de los parámetros configurados en Impresora.</p></figcaption></figure>

En la ventana de **General** se presentan las siguientes configuraciones en la que es relevante el alto de capa, en este caso es de 0.18mm.

<figure><img src="../.gitbook/assets/imagen_2023-12-01_112721945.png" alt=""><figcaption><p>Configuraciones de Alto de capa.</p></figcaption></figure>

En la ventana de Relleno se destaca la configuración de porcentaje de relleno y tipo de relleno.

<div>

<figure><img src="../.gitbook/assets/imagen_2023-12-01_112756150.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/imagen_2023-12-01_112814875.png" alt=""><figcaption><p>Parámetros configurados en Relleno.</p></figcaption></figure>

</div>

Una vez terminada las configuraciones se puede procesar los parámetros configurados en su totalidad, para ello seleccionamos Corte ubicado en el menú lateral derecho.

<figure><img src="../.gitbook/assets/imagen_2023-12-01_112837599.png" alt=""><figcaption><p>ícono de Corte.</p></figcaption></figure>

Una vez procesado el Corte podemos **ver las capas** y **descargar el archivo** en el formato procesable por nuestra impresora FlashForge Dreamer. También podemos seleccionar Iniciar Corte para configurar de nuevo nuestro parámetros.

<figure><img src="../.gitbook/assets/imagen_2023-12-01_113907993.png" alt=""><figcaption><p>Opciones a utilizar.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-12-01_114051046.png" alt=""><figcaption><p>Vistas de las capas a imprimir.</p></figcaption></figure>

Se observan a las capas muy alejadas entre sí, por ende se debe volver a configurar los parámetros modificando el alto de capa.

<figure><img src="../.gitbook/assets/imagen_2023-12-01_114440849.png" alt=""><figcaption><p>Zoom a las capas configuradas.</p></figcaption></figure>

Una vez configurado los parámetros para conseguir una mayor definición de las elevaciones obtenemos el siguiente corte.

<figure><img src="../.gitbook/assets/imagen_2023-12-01_114952994.png" alt=""><figcaption></figcaption></figure>

A día de hoy puedo observar que el tiempo de impresión es excesivo para el tamaño de la pieza.

<figure><img src="../.gitbook/assets/imagen_2023-12-01_115022298.png" alt=""><figcaption></figcaption></figure>

{% file src="../.gitbook/assets/Tembiaporá-cut.fpp" %}
Archivo descargable del archivo de Flashprint.
{% endfile %}

{% file src="../.gitbook/assets/Tembiaporá-cut.gx" %}
Archivo procesado en la impresora 3D.
{% endfile %}

Luego procedemos a imprimir en la impresora 3D siguiendo los pasos detallado en la siguiente documentación.

{% content-ref url="../impresion-3d/" %}
[impresion-3d](../impresion-3d/)
{% endcontent-ref %}

Siguiendo los pasos generales para procesar en 3D esperamos a obtener la pieza final.

{% hint style="info" %}
El el proceso se ha identificado que no se debe utilizar acentos en el archivo procesable por la impresora, por lo que debí modificar el nombre para poder imprimir la pieza.
{% endhint %}

### <mark style="color:purple;">Resultado del terreno obtenido con Terrain2stl impreso en 3D</mark>

&#x20;El resultado es una pieza pequeña el cual no se entiende que es una relevación topográfica, el gasto de material no rinde las expectativas y por ende no se recomienda este método.

<figure><img src="../.gitbook/assets/image (189).png" alt=""><figcaption><p>Vista superior del resultado de la impresión 3D.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (190).png" alt=""><figcaption><p>Perspectiva frontal del resultado de la impresión 3D.</p></figcaption></figure>

Normalmente una persona ajena a la fabricación digital se impresiona con los proyectos, sin embargo en este caso no se ha entendido su función y se comprobó que no es conveniente representar la relevación topográfica tan chica y muy plato (debí haber editado un poco).&#x20;

<figure><img src="../.gitbook/assets/imagen_2023-12-04_112535140.png" alt="" width="188"><figcaption><p>Uso de la relevación topográfica.</p></figcaption></figure>

En este caso incluso se dió vuelta a la cara de la representación topográfica.

***

Una variable a Terrain2STL es la página Map2STL.

{% embed url="https://map2stl.com" %}

Aunque Map2STL destaca por su funcionalidad de previsualización del modelo, brindándonos la capacidad de anticipar el resultado final, debemos considerar que este enfoque tiende a generar modelos con una resolución más baja, lo que se conoce como estilo LowPoly.

Por otro lado, Terrain2STL sobresale al proporcionar una definición superior en los resultados, capturando con mayor detalle las complejidades del relieve. Esta calidad mejorada puede ser crucial en proyectos que requieren una representación más precisa del terreno.

<figure><img src="../.gitbook/assets/Captura de pantalla 2023-11-30 094138.png" alt=""><figcaption><p>Vista de la página de Maps2STL.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Captura de pantalla 2023-11-30 100137.png" alt=""><figcaption><p>Vista del resultado de Map2STL.</p></figcaption></figure>

Para mejorar la definición de los modelos generados por **Map2STL**, se ha aplicado el modificador **Subdivision Surface** en Blender. Esta técnica ha demostrado ser eficaz al suavizar y detallar el modelo resultante.

<figure><img src="../.gitbook/assets/imagen_2023-11-30_102345328.png" alt=""><figcaption><p>Para compensar la definición de Map2STL apliqué el modificador Subdivision Surface de Blender.</p></figcaption></figure>

Sin embargo, tras la aplicación de este modificador, nos enfrentamos a un inconveniente: el archivo resultante se ha vuelto considerablemente pesado. Este desafío plantea la necesidad de explorar estrategias adicionales para optimizar el tamaño del archivo sin comprometer la calidad visual.

### <mark style="color:purple;">Proceso en Meshmixer</mark>

Ante el desafío del archivo pesado resultante de la aplicación del modificador Subdivision Surface, consideramos la posibilidad de mejorar tanto el peso como la definición utilizando Meshmixer.

Exploraremos cómo las herramientas disponibles en Meshmixer pueden ayudarnos a optimizar el modelo, reduciendo su tamaño sin sacrificar la calidad visual.

<figure><img src="../.gitbook/assets/imagen_2023-11-30_130433255.png" alt=""><figcaption></figcaption></figure>

Una vez más aplicamos la herramienta "Make Solid" para optimizar el modelo. Recomendamos configurar los parámetros de 'Solid Type' en 'Accurate' y 'Solid Accuracy' al máximo para garantizar una preparación adecuada del modelo. Una vez satisfechos con los resultados, eliminamos el archivo original y conservamos solo la versión modificada.

<figure><img src="../.gitbook/assets/imagen_2023-11-30_130510181.png" alt=""><figcaption><p>Seleccionar Make Solid ubicado en la ventana de Edit en el menú lateral.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-30_130916787.png" alt=""><figcaption><p>Parámetros establecidos para obtener nuestra pieza.</p></figcaption></figure>

Una vez que obtenemos un modelo que satisfaga nuestras expectativas seleccionar Accept.&#x20;

<figure><img src="../.gitbook/assets/imagen_2023-12-01_110120336.png" alt=""><figcaption></figcaption></figure>

Al generar el Make Solid obtenemos dos objetos, por ello a continuación eliminamos el archivo original y conservamos solo la versión modificada.

<div>

<figure><img src="../.gitbook/assets/imagen_2023-11-30_131142216.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/imagen_2023-11-30_131657282.png" alt=""><figcaption></figcaption></figure>

</div>

A continuación debemos exportar el archivo en formato .stl para procesarlo en un formato adecuado para el fresado CNC.

{% file src="../.gitbook/assets/Tembiapora Meshmixer.mix" %}
Archivo de Meshmixer descargable.
{% endfile %}

{% file src="../.gitbook/assets/Tembiapora post meshmixer.stl" %}
Archivo descargable en formato .stl.
{% endfile %}

***

## <mark style="color:purple;">**VCarve Pro y Fresado CNC:**</mark>

<mark style="color:purple;">**Preparación del Modelo:**</mark>

* Asegúrate de tener el modelo optimizado en formato STL listo para el fresado CNC.

{% file src="../.gitbook/assets/Tembiapora post meshmixer.stl" %}
Archivo descargable en formato .stl.
{% endfile %}

<mark style="color:purple;">**Importación del Modelo:**</mark>

* Abre VCarve Pro y selecciona la opción para importar tu modelo STL. Asegúrate de que las unidades y dimensiones coincidan con las del modelo original.

<figure><img src="../.gitbook/assets/Screenshot 2023-11-29 124309.png" alt=""><figcaption><p>Crear un nuevo documento al abrir el programa.</p></figcaption></figure>

Determinar las dimensiones del área de trabajo en coincidencia a las dimensiones de nuestro material a trabajar.

<figure><img src="../.gitbook/assets/Screenshot 2023-11-30 151004.png" alt=""><figcaption></figcaption></figure>

Al llegar a esta fase me olvidé de anotar mis dimensiones a configurar, así que establecí un aproximado que más tarde se puede volver a configurar.

<div>

<figure><img src="../.gitbook/assets/Screenshot 2023-11-30 151106.png" alt=""><figcaption><p>Dimensiones establecidas para el área de trabajo.</p></figcaption></figure>

 

<figure><img src="../.gitbook/assets/Captura de pantalla 2023-11-30 151756.png" alt=""><figcaption><p>Dimensiones de mi archivo .stl</p></figcaption></figure>

</div>

Aceptar las configuraciones.

<figure><img src="../.gitbook/assets/Screenshot 2023-11-29 124851.png" alt=""><figcaption><p>Seleccionar OK para continuar.</p></figcaption></figure>

Es habitual que utilicemos la ventana de <mark style="color:purple;">**Drawing**</mark> pero para este fresado en el que tallaremos con la CNC nos ubicaremos en la ventana de <mark style="color:purple;">**Modeling**</mark>.

<figure><img src="../.gitbook/assets/Screenshot 2023-11-30 151144.png" alt=""><figcaption><p>Ventana de Modeling sin haber cargado un archivo.</p></figcaption></figure>

Seleccionamos el ícono de la carpeta para abrir el archivo, en la ventana emergente seleccionamos el stl a fresar.

<figure><img src="../.gitbook/assets/imagen_2023-12-03_195344447.png" alt=""><figcaption><p>Se resalta el ícono de la carpeta.</p></figcaption></figure>

Nos dirigimos a la configuración de la edición de la dimensión del modelo. Se ha establecido que la altura a fresar será de 45mm. La razón para modificar este parámetro es que queremos intensificar las curvas del modelo para que el fresado no quede muy plato.

Nuestro material de polifoam es de 250mm de altura, se pegarán dos pedazos de las mismas dimensiones para alcanzar una altura de 500mm en total y que resalte más el modelo.

<figure><img src="../.gitbook/assets/Screenshot 2023-11-30 152340.png" alt=""><figcaption><p>Determinación de la altura a fresar.</p></figcaption></figure>

En la vista de previsualización podemos ver cómo está quedando el modelo y una vez satisfechos con el modelo seleccionamos <mark style="color:purple;">**Position and Import**</mark> para continuar.

<figure><img src="../.gitbook/assets/Screenshot 2023-11-30 152356.png" alt=""><figcaption><p>Previsualización del modelo.</p></figcaption></figure>

Por último se establece la distancia que será fresada, y lo que queda fuera a operar.

<figure><img src="../.gitbook/assets/Screenshot 2023-11-30 152506.png" alt=""><figcaption></figcaption></figure>

Como no entendía bien las funciones de esta configuración he aquí la descripción de las funciones de <mark style="color:purple;">“</mark><mark style="color:purple;">**Importar modelo 3D > Posición**</mark><mark style="color:purple;">”</mark>.&#x20;

<table><thead><tr><th width="193.5">Función</th><th>Descripción</th></tr></thead><tbody><tr><td><mark style="color:purple;"><strong>Posición relativa al plano de modelado</strong></mark></td><td>Esta sección te permite ajustar la posición del modelo 3D en relación con el centro de rotación. Por defecto, VCarve Pro posiciona el modelo en el centro del bloque de material, para aprovechar mejor el material. Cuando se selecciona la opción Desactivado, el movimiento del modelo 3D se hace de la manera habitual.</td></tr><tr><td><mark style="color:purple;"><strong>Profundidad bajo la parte superior</strong></mark></td><td>Esta sección te permite ajustar la profundidad del modelo 3D por debajo de la parte superior del bloque de material. Puedes introducir un valor numérico o usar los botones de flecha para cambiar la profundidad. También puedes usar el control deslizante para ver cómo cambia la profundidad en la vista 3D.</td></tr><tr><td><mark style="color:purple;"><strong>Descartar datos por debajo del plano cero</strong></mark></td><td>Esta sección te permite eliminar los datos del modelo 3D que están por debajo del plano cero, es decir, la parte inferior del bloque de material. Puedes activar o desactivar esta opción con la casilla de verificación. Esta opción puede ser útil para reducir el tamaño del archivo y el tiempo de mecanizado.</td></tr><tr><td><mark style="color:purple;"><strong>Resaltar rebajes</strong></mark></td><td>Esta sección te permite resaltar las partes del modelo 3D que tienen rebajes, es decir, partes que no se pueden mecanizar con una herramienta cilíndrica. Puedes activar o desactivar esta opción con la casilla de verificación. Esta opción puede ser útil para identificar las zonas problemáticas del modelo 3D.</td></tr><tr><td><mark style="color:purple;"><strong>Actualizar rebajes</strong></mark></td><td>Esta sección te permite actualizar los rebajes del modelo 3D después de cambiar la posición o la profundidad del modelo. Puedes hacer clic en el botón de Actualizar rebajes para ver los cambios en la vista 3D.</td></tr><tr><td><mark style="color:purple;"><strong>Aplicar</strong></mark></td><td>Este botón te permite confirmar los cambios que has hecho en el modelo 3D y cerrar el cuadro de diálogo.</td></tr><tr><td><mark style="color:purple;"><strong>Cancelar</strong></mark></td><td>Este botón te permite descartar los cambios que has hecho en el modelo 3D y cerrar el cuadro de diálogo.</td></tr><tr><td><mark style="color:purple;"><strong>Posición e importar ></strong></mark></td><td>Este botón te permite avanzar al siguiente paso del proceso de importación y mecanizado del modelo 3D.</td></tr></tbody></table>

Como había sido establecido una dimensión aproximada del material, ahora procedemos a cambiar las dimensiones, primero dirigirse a la ventana de <mark style="color:purple;">Drawing</mark>, luego seleccionar <mark style="color:purple;">**Job Setup**</mark> y encontraremos un menú idéntico al que utilizamos al iniciar cada nuevo proyecto.&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2023-11-30 152603.png" alt=""><figcaption><p>Cambio de dimensión del material en Job Setup.</p></figcaption></figure>

Ahora debemos seleccionar en el menú de <mark style="color:purple;">**Modeling ¨Crear contorno vectorial alrededor de los componentes seleccionados¨**</mark>

<figure><img src="../.gitbook/assets/imagen_2023-12-04_000458500.png" alt=""><figcaption><p>El ícono a utilizar se encuentra en Modeling, en la misma ubicación en donde importamos nuestro archivo .stl.</p></figcaption></figure>

Esta función _crea un límite vectorial alrededor de los componentes que hayas seleccionado en tu espacio de trabajo._&#x20;

Esto puede ser útil para definir un área específica para aplicar cambios o realizar operaciones en esos componentes seleccionados.&#x20;

Por ejemplo, puedes querer aplicar un efecto o transformación específica solo a ciertos componentes de tu modelo 3D, y esta función te permitiría seleccionar exactamente qué partes del modelo se verán afectadas.&#x20;

Es una herramienta útil para tener un control más preciso sobre tus ediciones y transformaciones en el software de modelado 3D.

<figure><img src="../.gitbook/assets/Screenshot 2023-11-30 152659.png" alt=""><figcaption><p><strong>Crear contorno vectorial alrededor de los componentes seleccionados.</strong></p></figcaption></figure>

<mark style="color:purple;">**Configuración en Toolpath:**</mark>

Selecciona <mark style="color:purple;">**Toolpath**</mark> para configurar las herramientas de corte adecuadas en VCarve Pro. Ajusta parámetros como velocidad de corte, profundidad de paso y otros según el material y el tipo de fresa que estés utilizando.

No debemos olvidar seleccionar en el área de trabajo el objeto para editar en <mark style="color:purple;">**Toolpath.**</mark>

Para el mecanizado seleccionaremos el ícono de <mark style="color:purple;">**3D Roughing Toolpath**</mark><mark style="color:purple;">.</mark>

<figure><img src="../.gitbook/assets/Screenshot 2023-11-30 152919.png" alt=""><figcaption><p>Seleccionar 3D Roughing Toolpath en la selección de Operaciones.</p></figcaption></figure>

Una vez seleccionada la operación nos aparecerá el menú de parámetros a configurar de esa operación.

<figure><img src="../.gitbook/assets/Screenshot 2023-11-30 153203.png" alt=""><figcaption><p>Parámetros a editar en Toolpath de Rough Machinig Toolpath.</p></figcaption></figure>

A continuación una explicación general sobre qué trata cada configuración a realizar.

<table><thead><tr><th width="183.5">Función</th><th>Descripción</th></tr></thead><tbody><tr><td><mark style="color:purple;"><strong>Selección de herramienta</strong></mark><img src="../.gitbook/assets/image (191).png" alt=""></td><td>Esta función te permite seleccionar la herramienta/broca que se utilizará para el mecanizado.</td></tr><tr><td><mark style="color:purple;"><strong>Límite</strong></mark><img src="../.gitbook/assets/image (195).png" alt=""></td><td><p></p><p>Esta función te habilita para establecer el límite del mecanizado.</p><ul><li><mark style="color:purple;"><strong>Model Boundary</strong>:</mark> Esta función emplea los límites combinados de todos los componentes en el trabajo. Representa el área del modelo compuesto que contiene componentes.</li><li><mark style="color:purple;"><strong>Material Boundary</strong>:</mark> Utiliza el límite del bloque de material completo.</li><li><mark style="color:purple;"><strong>Selected Vector(s)</strong>:</mark> Utiliza los vectores seleccionados como límite de mecanizado. Estos vectores seleccionados pueden emplearse para crear un perfil de herramienta.</li><li><mark style="color:purple;"><strong>Selected Level</strong>:</mark> Utiliza los límites combinados de todos los componentes en el nivel especificado. Similar a <strong>Model Boundary</strong>, pero específico para el nivel nombrado.</li><li><mark style="color:purple;"><strong>Level:</strong></mark> No se encontró información específica sobre esta función en el software de control de máquinas CNC.</li><li><mark style="color:purple;"><strong>Boundary Offset:</strong></mark> Cuando estás mecanizando un objeto elevado, la herramienta a menudo no mecanizará completamente el borde. Este campo se utiliza para especificar un desplazamiento al límite de mecanizado seleccionado, aumentando su tamaño para permitir que la herramienta sobrepase el borde real si es necesario.</li></ul></td></tr><tr><td><mark style="color:purple;"><strong>Margen de Mecanizado</strong></mark><img src="../.gitbook/assets/image (202).png" alt=""></td><td>El tamaño del <mark style="color:purple;"><strong>margen de mecanizado</strong></mark> tiene un impacto crítico en la calidad y eficiencia del proceso. Un margen excesivo aumenta la carga de trabajo, reduce la productividad y eleva los costos de materiales, herramientas y electricidad, mientras que un margen muy pequeño puede no corregir defectos previos ni compensar errores de sujeción, conduciendo a productos defectuosos. El principio clave en la elección del margen es minimizarlo, siempre y cuando se asegure la calidad del producto.</td></tr><tr><td><mark style="color:purple;"><strong>Estrategia de desbaste</strong></mark><img src="../.gitbook/assets/image (196).png" alt=""></td><td><p>Esta función te permite elegir la estrategia de desbaste y perfil para el mecanizado.</p><p><mark style="color:purple;"><strong>Estrategia de Desbaste</strong></mark><strong>:</strong> El desbaste es crucial en las etapas iniciales del mecanizado, dando forma al material cerca de la geometría deseada. Dos opciones están disponibles:</p><ul><li><mark style="color:purple;"><strong>Z Level</strong></mark><strong>:</strong> Utiliza trayectorias de bolsillo 2D para eliminar material alrededor del modelo 3D, respetando el límite especificado.</li><li><mark style="color:purple;"><strong>3D Raster</strong></mark><strong>:</strong> Calcula un patrón de trama en la superficie 3D y mecaniza dentro del vector seleccionado(s), permitiendo control sobre el ángulo de la trama.</li></ul><p><mark style="color:purple;"><strong>Perfil</strong></mark><strong>:</strong> Selecciona el perfil para el mecanizado, con opciones para perfiles externos, internos o en vectores seleccionados. Ajusta automáticamente el diámetro y ángulo de la herramienta para la profundidad de corte deseada. Dos opciones disponibles:</p><ul><li><mark style="color:purple;"><strong>Last</strong></mark><strong>:</strong> Realiza el corte de perfil después de la trama en cada nivel.</li><li><mark style="color:purple;"><strong>Level by level</strong></mark><strong>:</strong> Realiza el corte de perfil antes de la trama en cada nivel.</li></ul><p><mark style="color:purple;"><strong>Orden</strong></mark><strong>:</strong> Elige el orden de mecanizado, aunque las opciones no están claras en la captura de pantalla.</p><p><mark style="color:purple;"><strong>Ángulo de Trama:</strong></mark> Introduce el ángulo de trama para el mecanizado, determinando el patrón de corte en la superficie 3D. Un ángulo de 0° genera un patrón principalmente paralelo al eje X, mientras que 90° es principalmente paralelo al eje Y.</p></td></tr><tr><td><mark style="color:purple;"><strong>Ramp Plunge Moves</strong></mark><img src="../.gitbook/assets/image (199).png" alt=""></td><td>Esta función reduce la presión sobre la broca y la máquina, mejorando la calidad del corte en el punto de entrada al cortar en ángulo. Al seleccionar esta función y establecer una distancia de rampa, la herramienta cortará en un ángulo específico. Por ejemplo, si se corta un agujero circular de 2" de diámetro a través de un material de 1/2" de espesor con una distancia de rampa de 0.375, el corte inicial comenzará 0.375" dentro del vector y finalizará en el punto de 2" del agujero. Este enfoque tiene como objetivo reducir la carga del husillo y disminuir la acumulación de calor.</td></tr><tr><td><mark style="color:purple;"><strong>Z seguro</strong></mark><img src="../.gitbook/assets/image (197).png" alt=""></td><td><p></p><p><mark style="color:purple;"><strong>Safe Z</strong>:</mark> Esta función se relaciona con la altura segura en el eje Z, la cual es la distancia que la herramienta se eleva por encima de la pieza de trabajo durante movimientos no relacionados con el corte para evitar colisiones con la pieza o los sujetadores. En este caso, el valor es de 3.0 mm.</p><p><mark style="color:purple;"><strong>Home-Position</strong>:</mark> Esta función se refiere a la posición de inicio o "home" de la máquina. Es la posición a la cual la máquina retorna después de completar una tarea. En sistemas CNC, la posición de inicio suele ser el punto más alejado en todos los ejes, es decir, el punto (0,0,0). En este caso, la posición de inicio es X: 0.00, Y: 0.00, Z: 12.00.</p></td></tr><tr><td><mark style="color:purple;"><strong>Calcular trayectoria de herramienta</strong></mark><img src="../.gitbook/assets/image (198).png" alt=""></td><td>Esta función te permite calcular la trayectoria de la herramienta para el mecanizado.</td></tr><tr><td><mark style="color:purple;"><strong>Cerrar</strong></mark></td><td>Esta función te permite cerrar la ventana.</td></tr></tbody></table>

#### <mark style="color:purple;">Editar Tool en Toolpath</mark>

En tools se estable el tipo de broca a utilizar que sería de punta redonda de diámetro de 1/4, y la velocidad a 12000 rpm, también el <mark style="color:purple;">**Feed Units**</mark> a mm/sec.

<figure><img src="../.gitbook/assets/Screenshot 2023-11-30 153121.png" alt=""><figcaption><p>Edición en Tools.</p></figcaption></figure>

<table><thead><tr><th width="208.5">Tipo de Herramienta</th><th>Esta función permite seleccionar el tipo de herramienta que se va a utilizar. Los tipos de herramientas pueden variar dependiendo del software, pero generalmente incluyen opciones como fresas de extremo plano, fresas de nariz de bola, taladros, etc.</th></tr></thead><tbody><tr><td><mark style="color:purple;"><strong>Unidades</strong></mark></td><td>Esta función permite seleccionar las unidades de medida que se utilizarán para los parámetros de la herramienta. Las opciones suelen ser milímetros (mm) o pulgadas (in).</td></tr><tr><td><mark style="color:purple;"><strong>Diámetro</strong></mark></td><td>Esta función permite ingresar el diámetro de la herramienta. El diámetro se refiere al ancho de la herramienta.</td></tr><tr><td><mark style="color:purple;"><strong>Parámetros de Corte</strong></mark></td><td>Estos son los parámetros que controlan cómo se realiza el corte. Pueden incluir cosas como la profundidad de corte, la velocidad de avance, la velocidad de giro, etc.</td></tr><tr><td><mark style="color:purple;"><strong>Velocidades de Avance</strong></mark></td><td>Estas son las velocidades a las que se mueve la herramienta durante el corte. Pueden incluir la velocidad de avance en el eje X, Y y Z.</td></tr><tr><td><mark style="color:purple;"><strong>Modelo 3D de la Herramienta</strong></mark></td><td>Esta es una representación visual de la herramienta basada en los parámetros ingresados.</td></tr></tbody></table>

#### <mark style="color:purple;">Edit Passes</mark>

| Función                    | Descripción                                                                                                                                                                                  |
| -------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Profundidad total de corte | Permite especificar la profundidad total de corte para la herramienta. En este caso, el valor es de 47.077 mm1.                                                                              |
| Profundidades de paso      | Permite especificar las profundidades de cada paso de corte. En este caso, los valores son 7.842, 8.929, 9.523, 11.361, 15.262, 19.2581. Estas funciones controlan cómo se realiza el corte. |

<figure><img src="../.gitbook/assets/Screenshot 2023-11-30 153432.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Screenshot 2023-11-30 153641.png" alt=""><figcaption></figcaption></figure>



<mark style="color:purple;">**Estrategia de Fresado:**</mark>

* Planifica la estrategia de fresado. Decide entre el fresado en pasadas escalonadas, fresado en espiral u otras estrategias dependiendo de la complejidad de tu modelo y la herramienta seleccionada.



<mark style="color:purple;">**Trayectorias de Herramientas:**</mark>

* Genera las trayectorias de herramientas. VCarve Pro te permitirá previsualizar cómo se llevará a cabo el fresado. Ajusta según sea necesario para optimizar la eficiencia y la calidad.



<mark style="color:purple;">**Configuración de Profundidad:**</mark>

* Asegúrate de configurar correctamente las profundidades de corte para cada operación. Esto es crucial para obtener el relieve y detalles deseados en tu modelo.



<mark style="color:purple;">**Simulación:**</mark>

* Utiliza la función de simulación en VCarve Pro para revisar cómo se ejecutará el fresado. Esto te ayudará a identificar posibles problemas antes de enviar el trabajo a la fresadora CNC.



<mark style="color:purple;">**Postprocesamiento:**</mark>

* Después de revisar y simular, genera el código G (Código de Control Numérico) necesario para la fresadora CNC. Asegúrate de seleccionar el postprocesador correcto para tu máquina.



{% file src="../.gitbook/assets/3D Roughing 1.rol" %}
GCode del fresado del relieve.
{% endfile %}

{% file src="../.gitbook/assets/Profile 1.rol" %}
GCode de realización del perfil.
{% endfile %}

<details>

<summary><mark style="color:purple;">Código G o GCode</mark></summary>

Un código G, abreviatura de "código geométrico" o "código de control numérico", es un conjunto de comandos alfanuméricos utilizados en programación CNC (Control Numérico por Computadora).&#x20;

Estos códigos indican a la máquina herramienta, como un fresadora o un torno CNC, las instrucciones específicas para llevar a cabo una tarea determinada, como movimientos, velocidades, y operaciones de herramientas.&#x20;

Los códigos G son esenciales para traducir el diseño digital en movimientos físicos y acciones de la máquina durante el proceso de fabricación.&#x20;

Cada código G tiene una función específica, como desplazamientos, cambios de herramientas, o control de velocidad, contribuyendo a la precisión y automatización en la producción.

</details>

## <mark style="color:purple;">Proceso en la fresadora CNC Roland</mark>

En el desarrollo de la tarea en la fresadora CNC Roland, se siguieron cuidadosamente los siguientes pasos:

<mark style="color:purple;">**1. Encendido y Posicionamiento Inicial:**</mark>

* Inicialmente, se encendió la fresadora y se realizó el posicionamiento inicial.&#x20;
* El material de trabajo, previamente cortado y adherido con cinta doble faz, fue centrado en la plataforma.
* &#x20;Dos piezas superpuestas se utilizaron para obtener un bloque de trabajo de 500 mm de altura, como se había configurado en VCarve Pro.
* Se debe marcar el centro del material con diagonales tal cómo habíamos establecido en VCarve Pro el eje del centro como punto inicial.

<mark style="color:purple;">**2. Centrado de Ejes X e Y:**</mark>

* Se establecieron el punto 0 de los ejes X e Y utilizando el mando de la fresadora para garantizar una alineación precisa del material con respecto a las coordenadas del programa.

<mark style="color:purple;">**3. Centrado del Eje Z:**</mark>

* Para el eje Z, se utilizó el imán de la máquina para asegurar una referencia precisa. Este paso es crucial para la profundidad correcta de fresado y la calidad del resultado final.

<mark style="color:purple;">**4. Importación Secuencial de Códigos G:**</mark>

* Se importaron por turno los códigos G generados en VCarve Pro. Primero, se procesó el código de fresado para esculpir las montañas, seguido por el código de perfil para eliminar excedentes en los laterales y obtener la forma final deseada.

<mark style="color:purple;">**5. Proceso de Fresado de Montañas:**</mark>

* Se ejecutó el código G correspondiente al fresado de las montañas. La fresadora siguió las instrucciones para esculpir las elevaciones y detalles precisos del terreno.

<mark style="color:purple;">**6. Cambio y Proceso de Fresado de Perfil:**</mark>

* Después de completar el fresado de las montañas, se cambió a la herramienta necesaria y se procesó el código de perfil. Esto eliminó los excedentes laterales, proporcionando la forma final de la pieza.

<mark style="color:purple;">**7. Evaluación Continua:**</mark>

* Durante todo el proceso, se llevó a cabo una evaluación continua para asegurar que la fresadora estuviera siguiendo las trayectorias correctas y que el material se estuviera trabajando según lo planificado.



<mark style="color:purple;">**8. Finalización y Extracción:**</mark>

* Una vez que ambos códigos G se completaron con éxito, se detuvo la fresadora. La pieza final fresada fue cuidadosamente retirada de la mesa.



### <mark style="color:purple;">Resultado del terreno de Tembiaporã fresado</mark>

<table><thead><tr><th width="196.33333333333331">Aspecto</th><th>Terrain2STL (Impresión 3D)</th><th>Maps2STL (Fresado CNC)</th></tr></thead><tbody><tr><td><strong>Resolución y Detalle</strong></td><td>Alta resolución y detalle.</td><td>Resolución más baja (LowPoly)</td></tr><tr><td><strong>Tamaño del Modelo</strong></td><td>Puede ser muy pequeño. En casos grandes, pérdida innecesaria de filamento y tiempo.</td><td>Tarda, pero el resultado cumple expectativas.</td></tr><tr><td><strong>Experiencia de Usuario</strong></td><td>Para comprobar las configuraciones se debe descargar el archivo innecesariamente.</td><td>Permite la previsualización del archivo online. Interfaz agradable y fácil de usar. </td></tr><tr><td><strong>Mejoras Necesarias</strong></td><td>Utilizar Meshmixer para optimizar el modelo para la impresión.</td><td>Se debe suavizar el mesh del objeto sin falta o de lo contrario el resultado no será satisfactorio.</td></tr><tr><td><strong>Conclusión</strong></td><td>Ideal para modelos pequeños.</td><td>Eficiente para proyectos a mayor escala.</td></tr><tr><td><strong>Observaciones</strong></td><td>Modelos grandes pueden ser una pérdida innecesaria de recursos.</td><td>Requiere mejoras previas, pero ofrece flexibilidad y eficiencia.</td></tr></tbody></table>

## <mark style="color:purple;">Comparaciones entre los modelos obtenidos</mark>

