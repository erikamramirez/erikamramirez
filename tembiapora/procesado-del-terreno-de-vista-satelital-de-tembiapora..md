---
coverY: 0
---

# Procesado del terreno de vista satelital de Tembiaporã.

Para llevar a cabo el fresado en nuestro proyecto, utilizaremos la herramienta Terrain2stl. Esta página desempeñará un papel fundamental al convertir datos de terreno desde imágenes de vista satelital en archivos STL, permitiéndonos así crear representaciones tridimensionales precisas del relieve.

{% embed url="https://jthatch.com/Terrain2STL/" %}
Página de Terrain2STL,
{% endembed %}

Esta herramienta ya fue utilizada en proyectos anteriores, en la siguiente documentación de este Gitbook se describe su uso y los resultados.

{% content-ref url="../cnc/pasos-de-uso-de-la-cnc/obtencion-de-modelo-3d-topografico/" %}
[obtencion-de-modelo-3d-topografico](../cnc/pasos-de-uso-de-la-cnc/obtencion-de-modelo-3d-topografico/)
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

&#x20;



***

Una variable a Terrain2STL es la página Map2STL.

{% embed url="https://map2stl.com" %}

Aunque Map2STL destaca por su funcionalidad de previsualización del modelo, brindándonos la capacidad de anticipar el resultado final, debemos considerar que este enfoque tiende a generar modelos con una resolución más baja, lo que se conoce como estilo LowPoly.

Por otro lado, Terrain2STL sobresale al proporcionar una definición superior en los resultados, capturando con mayor detalle las complejidades del relieve. Esta calidad mejorada puede ser crucial en proyectos que requieren una representación más precisa del terreno.

<figure><img src="../.gitbook/assets/Captura de pantalla 2023-11-30 094138.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Captura de pantalla 2023-11-30 100137.png" alt=""><figcaption><p>Vista del resultado de Map2STL.</p></figcaption></figure>

Para mejorar la definición de los modelos generados por **Map2STL**, se ha aplicado el modificador **Subdivision Surface** en Blender. Esta técnica ha demostrado ser eficaz al suavizar y detallar el modelo resultante.

<figure><img src="../.gitbook/assets/imagen_2023-11-30_102345328.png" alt=""><figcaption><p>Para compensar la definición de Map2STL apliqué el modificador Subdivision Surface de Blender.</p></figcaption></figure>

Sin embargo, tras la aplicación de este modificador, nos enfrentamos a un inconveniente: el archivo resultante se ha vuelto considerablemente pesado. Este desafío plantea la necesidad de explorar estrategias adicionales para optimizar el tamaño del archivo sin comprometer la calidad visual.

## <mark style="color:purple;">Proceso en Meshmixer</mark>

"Ante el desafío del archivo pesado resultante de la aplicación del modificador Subdivision Surface, consideramos la posibilidad de mejorar tanto el peso como la definición utilizando Meshmixer.

Exploraremos cómo las herramientas disponibles en Meshmixer pueden ayudarnos a optimizar el modelo, reduciendo su tamaño sin sacrificar la calidad visual.

<figure><img src="../.gitbook/assets/imagen_2023-11-30_130433255.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-30_130510181.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-30_130916787.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-12-01_110120336.png" alt=""><figcaption></figcaption></figure>

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

### VCarve Pro

### Proceso en la fresadora CNC Roland

### Resultado

## Comparaciones entre los modelos obtenidos
