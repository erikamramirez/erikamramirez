# Crear un diseño 2D multicapa

Con el objetivo de realizar un sticker con la plotter de corte de vinilo, realizaremos los siguientes pasos detallados a continuación. Primero seleccionaremos nuestra imagen.

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_203213350.png" alt=""><figcaption><p>Imagen .PNG seleccionada del personaje Jack Frost.</p></figcaption></figure>



Esta imagen .PNG deberá ser convertida a .SVG para poder procesar por el plotter, y también debe ser separado los colores a utilizar por capas. Para poder realizar el siguiente proceso utilizaremos el programa que descargamos en los pasos anteriores de esta documentación Inkscape, se trata de una alternativa a los programas de Adobe sin costo.

{% hint style="info" %}
Podemos utilizar Inkscape tanto con .JPG como con .PNG.
{% endhint %}

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_203225518.png" alt=""><figcaption><p>Abrir nuevo documento de Inkscape.</p></figcaption></figure>

Para evitar equivocarnos con el tamaño del sticker que realizaremos, cambiaré el tamaño de la mesa de trabajo en la que trabajaremos. Para esto dirigimos el mouse hacia el menú superior sobre Archivo, y seleccionaremos propiedades del documento o podemos utilizar el comando Mayús+Ctrl+D.

<figure><img src="../../.gitbook/assets/image (8) (1).png" alt=""><figcaption><p>Menú de Archivo.</p></figcaption></figure>

Estimaré las dimensiones de la mesa de trabajo a 100 x 100mm.

<div>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_203734019.png" alt=""><figcaption><p>Dimensiones Default de la mesa de trabajo.</p></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_203744600.png" alt=""><figcaption><p>Formato personalizado de 100 x 100mm.</p></figcaption></figure>

</div>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_203755292.png" alt=""><figcaption><p>Nueva dimensión de la mesa de trabajo completada.</p></figcaption></figure>

Podemos copiar y pegar la imagen directamente al programa, esto es útil cuando el personaje a color se encuentra sobre un fondo blanco en caso de .JPG, en este ejempo se trata ya directamente de un .PNG sin fondo. Procederemos a copiar desde la web y pegar directamente sobre la mesa de trabajo en Inkscape.

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_203847064.png" alt=""><figcaption><p>Click derecho y copiamos desde la documentación.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_203857356.png" alt=""><figcaption><p>Click derecho y pegamos en la pesa de trabajo.</p></figcaption></figure>

Ahora volvemos al menú superior y nos ubicaremos sobre ¨Trazo¨ y seleccionamos ¨Vectorizar mapa de bits¨ Mayús+Alt+B.

<div>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_203930573.png" alt=""><figcaption><p>Menú de trazo completo.</p></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_203940844.png" alt=""><figcaption><p>Seleccionar Vectorizar mapa de bits.</p></figcaption></figure>

</div>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_203952145.png" alt=""><figcaption><p>Ventana lateral de Vectorizar Mapa de Bits.</p></figcaption></figure>

Si uno encuentra satisfactorio el resultado por default al ejecutar el vectorizado de bits se puede dejar de esta manera y aplicar para continuar.

<div>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_204121724.png" alt=""><figcaption><p>Ventana de configuración de mapa de bits de nuestra imagen editada en pasada simple.</p></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_204134233.png" alt=""><figcaption><p>Zoom en pasada simple.</p></figcaption></figure>

</div>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_204146538.png" alt=""><figcaption><p>Ahora contamos con nuestra primera capa SVG.</p></figcaption></figure>

Ahora contamos con nuestra primera capa de bits y procederemos a realizar las capas de colores, entonces repetiremos los primeros pasos de seleccionar la imagen principal, trazo y vectorizar la capa de bits. Ahora con la diferencia de que en lugar de ubicarnos en la ventana de Pasada Simple.

<div>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_204157171.png" alt=""><figcaption><p>Ventana de imagen en multicolor.</p></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_204207787.png" alt=""><figcaption><p>Zoom a la ventana de Multicolor.</p></figcaption></figure>

</div>

Ahora cambiaremos el Modo de detección de Grises a Colores.

<div>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_204221979.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_204233076.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_204245156.png" alt=""><figcaption></figcaption></figure>

</div>

Y debemos seleccionar la cantidad de capas de colores que generaremos, para ello cambiaremos los números de ¨pasadas¨ hasta encontrar una cantidad que creamos satisfactoria.

<div>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_204316579.png" alt=""><figcaption><p>Ejemplo de 10 pasadas.</p></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_204326146.png" alt=""><figcaption><p>Ejemplo de 9 pasadas en vista completa.</p></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_204335716.png" alt=""><figcaption><p>Resultado de colores con 9 pasadas.</p></figcaption></figure>

</div>

Eliminaremos los colores no necesarios generados por el software y nos quedaremos con la capa azul, amarillo, blanco y negro.

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_204350932.png" alt=""><figcaption><p>Segundo intento de generar capas de la imagen .SVG, podemos ver que estas capas de ven más optimizadas en cuando al consumo del material.</p></figcaption></figure>

Seleccionaremos cada capa por turno, por ejemplo seleccionamos la capa azul, lo ubicaremos en la mesa de trabajo, que delimita lo que se verá en la impresión.

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_204519762.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_204528691.png" alt=""><figcaption><p>Menú de Archivo.</p></figcaption></figure>

* Nos dirigiremos al menú superior en Archivo.
* Seleccionar Exportar o el comando Mayús+Ctrl+E.
* Se abrirá una nueva pestaña lateral en el menú.

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_204554339.png" alt=""><figcaption><p>Pestaña lateral.</p></figcaption></figure>

* Antes de seleccionar Exportar debemos convertir el .SVG que se genera por default a .PGN, para ello abriremos el ícono de la carpeta.
* Ahora se abre la pestaña emergente debemos cambiar igualmente el nombre del archivo para diferenciarlos a la hora de exportar al plotter. Por ejemplo ¨Jack Frost capa azul¨.

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>El ícono de la carpeta.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_204840593.png" alt=""><figcaption><p>Pantalla emergente del nombre de archivo para exportar.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_204855281.png" alt=""><figcaption><p>Tipo de .svg de Inkscape.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_204910200.png" alt=""><figcaption><p>Buscamos .png y lo seleccionamos.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_204921149.png" alt=""><figcaption><p>Una vez que cambiamos el formato y seleccionamos Guardar.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_204932851.png" alt=""><figcaption><p>Una vez que terminamos el proceso anterior, ya se genera el documento .png. </p></figcaption></figure>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_205047439.png" alt=""><figcaption><p>Una vez obtenido la cantidad de capas de todos los colores pasamos al Plotter.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_205102849.png" alt=""><figcaption><p>Cambio de color visto en la ventana en Inkscape.</p></figcaption></figure>

{% hint style="info" %}
En el caso de imprimir en el vinilo destinado a la impresión sobre tela se debe invertir la imagen de la dirección deseada con mirror para poder imprimir correctamente con el vinilo debimos al proceso posterior para impregnar el vinilo a la tela.&#x20;
{% endhint %}

<div>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_205120156.png" alt=""><figcaption><p>Herramienta mirror en Inkscape. </p></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_205132536.png" alt=""><figcaption><p>Imagen reflejada luego de utilizar Mirror.</p></figcaption></figure>

</div>

Ahora podemos utilizar este archivo en el Plotter.
