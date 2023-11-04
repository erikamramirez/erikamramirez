---
description: >-
  Esta documentación servirá como una guía completa para la planificación,
  ejecución y presentación exitosa del proyecto de diseño paramétrico con
  Rhinoceros 3D y plotter de corte de vinilo.
cover: ../.gitbook/assets/Captura de pantalla 2023-10-10 162538.png
coverY: 0
---

# Plotter de Vinilo



## <mark style="color:blue;">**4- Crear un diseño 2D multicapa**</mark>

Con el objetivo de realizar un sticker con la plotter de corte de vinilo, realizaremos los siguientes pasos detallados a continuación.

Primero seleccionaremos nuestra imagen.

<figure><img src="broken-reference" alt=""><figcaption><p>Imagen .PNG seleccionada del personaje Jack Frost.</p></figcaption></figure>

Esta imagen .PNG deberá ser convertida a .SVG para poder procesar por el plotter, y también debe ser separado los colores a utilizar por capas. Para poder realizar el siguiente proceso utilizaremos el programa que descargamos en los pasos anteriores de esta documentación Inkscape, se trata de una alternativa a los programas de Adobe sin costo.

{% hint style="info" %}
Podemos utilizar Inkscape tanto con .JPG como con .PNG.
{% endhint %}

<figure><img src="broken-reference" alt=""><figcaption><p>Abrir nuevo documento de Inkscape.</p></figcaption></figure>

Para evitar equivocarnos con el tamaño del sticker que realizaremos, cambiaré el tamaño de la mesa de trabajo en la que trabajaremos. Para esto dirigimos el mouse hacia el menú superior sobre Archivo, y seleccionaremos propiedades del documento o podemos utilizar el comando Mayús+Ctrl+D.

<figure><img src="broken-reference" alt=""><figcaption><p>Menú de archivo.</p></figcaption></figure>

Estimaré las dimensiones de la mesa de trabajo a 100 x 100mm.

<div>

<figure><img src="broken-reference" alt=""><figcaption><p>Dimensiones Default de la mesa de trabajo.</p></figcaption></figure>

 

<figure><img src="broken-reference" alt=""><figcaption><p>Formato personalizado de 100 x 100mm.</p></figcaption></figure>

</div>

<figure><img src="broken-reference" alt=""><figcaption><p>Nueva dimensión de la mesa de trabajo completada.</p></figcaption></figure>

Podemos copiar y pegar la imagen directamente al programa, esto es útil cuando el personaje a color se encuentra sobre un fondo blanco en caso de .JPG, en este ejempo se trata ya directamente de un .PNG sin fondo. Procederemos a copiar desde la web y pegar directamente sobre la mesa de trabajo en Inkscape.

<figure><img src="broken-reference" alt=""><figcaption><p>Click derecho y copiamos desde la documentación.</p></figcaption></figure>

<figure><img src="broken-reference" alt=""><figcaption><p>Click derecho y pegamos en la pesa de trabajo.</p></figcaption></figure>

Ahora volvemos al menú superior y nos ubicaremos sobre ¨Trazo¨ y seleccionamos ¨Vectorizar mapa de bits¨ Mayús+Alt+B.

<div>

<figure><img src="broken-reference" alt=""><figcaption><p>Menú de trazo completo.</p></figcaption></figure>

 

<figure><img src="broken-reference" alt=""><figcaption><p>Seleccionar Vectorizar mapa de bits.</p></figcaption></figure>

</div>

<figure><img src="broken-reference" alt=""><figcaption><p>Ventana lateral de Vectorizar Mapa de Bits.</p></figcaption></figure>

Si uno encuentra satisfactorio el resultado por default al ejecutar el vectorizado de bits se puede dejar de esta manera y aplicar para continuar.

A continuación seleccionamos pasada simple y aplicamos.

<div>

<figure><img src="broken-reference" alt=""><figcaption><p>Ventana de configuración de mapa de bits de nuestra imagen editada en pasada simple.</p></figcaption></figure>

 

<figure><img src="broken-reference" alt=""><figcaption><p>Zoom en pasada simple.</p></figcaption></figure>

</div>

<figure><img src="broken-reference" alt=""><figcaption><p>Ahora contamos con nuestra primera capa SVG.</p></figcaption></figure>

Ahora contamos con nuestra primera capa de bits y procederemos a realizar las capas de colores, entonces repetiremos los primeros pasos de seleccionar la imagen principal, trazo y vectorizar la capa de bits. Ahora con la diferencia de que en lugar de ubicarnos en la ventana de Pasada Simple.

<div>

<figure><img src="broken-reference" alt=""><figcaption><p>Ventana de imagen en multicolor.</p></figcaption></figure>

 

<figure><img src="broken-reference" alt=""><figcaption><p>Zoom a la ventana de Multicolor.</p></figcaption></figure>

</div>

Ahora cambiaremos el Modo de detección de Grises a Colores.

<div>

<figure><img src="broken-reference" alt=""><figcaption></figcaption></figure>

 

<figure><img src="broken-reference" alt=""><figcaption></figcaption></figure>

 

<figure><img src="broken-reference" alt=""><figcaption></figcaption></figure>

</div>

Y debemos seleccionar la cantidad de capas de colores que generaremos, para ello cambiaremos los números de ¨pasadas¨ hasta encontrar una cantidad que creamos satisfactoria.

<div>

<figure><img src="broken-reference" alt=""><figcaption><p>Ejemplo de 10 pasadas.</p></figcaption></figure>

 

<figure><img src="broken-reference" alt=""><figcaption><p>Ejemplo de 9 pasadas en vista completa.</p></figcaption></figure>

 

<figure><img src="broken-reference" alt=""><figcaption><p>Resultado de colores con 9 pasadas.</p></figcaption></figure>

</div>

Eliminaremos los colores no necesarios generados por el software y nos quedaremos con la capa azul, amarillo, blanco y negro.

<figure><img src="broken-reference" alt=""><figcaption><p>Segundo intento de generar capas de la imagen .SVG, podemos ver que estas capas de ven más optimizadas en cuando al consumo del material.</p></figcaption></figure>

Seleccionaremos cada capa por turno, por ejemplo seleccionamos la capa azul, lo ubicaremos en la mesa de trabajo, que delimita lo que se verá en la impresión.

<figure><img src="broken-reference" alt=""><figcaption></figcaption></figure>

Para el método que utilizaremos para nuestro corte en el plotter, convertiremos las capas .SVG en .PNG con los siguientes pasos.&#x20;

<figure><img src="broken-reference" alt=""><figcaption><p>Menú de Archivo.</p></figcaption></figure>

* Nos dirigiremos al menú superior en Archivo.
* Seleccionar Exportar o el comando Mayús+Ctrl+E.
* Se abrirá una nueva pestaña lateral en el menú.

<figure><img src="broken-reference" alt=""><figcaption><p>Pestaña lateral.</p></figcaption></figure>

* Antes de seleccionar Exportar debemos convertir el .SVG que se genera por default a .PGN, para ello abriremos el ícono de la carpeta.
* Ahora se abre la pestaña emergente debemos cambiar igualmente el nombre del archivo para diferenciarlos a la hora de exportar al plotter. Por ejemplo ¨Jack Frost capa azul¨.

<figure><img src="broken-reference" alt=""><figcaption><p>El ícono de la carpeta.</p></figcaption></figure>

<figure><img src="broken-reference" alt=""><figcaption><p>Pantalla emergente del nombre de archivo para exportar.</p></figcaption></figure>

<figure><img src="broken-reference" alt=""><figcaption><p>Tipo de .svg de Inkscape.</p></figcaption></figure>

<figure><img src="broken-reference" alt=""><figcaption><p>Buscamos .png y lo seleccionamos.</p></figcaption></figure>

<figure><img src="broken-reference" alt=""><figcaption><p>Una vez que cambiamos el formato y seleccionamos Guardar.</p></figcaption></figure>

<figure><img src="broken-reference" alt=""><figcaption><p>Una vez que terminamos el proceso anterior, ya se genera el documento .png . </p></figcaption></figure>

{% hint style="info" %}
Una vez que terminamos de elegir en cambio de formato de .svg a .png el documento ya se genera automáticamente, al seleccionar Exportar al salir de la pestaña emergente sale una nueva pestaña emergente para volver a guardar el archivo.
{% endhint %}

<figure><img src="broken-reference" alt=""><figcaption><p>Aviso de reemplazar el archivo ya guardado.</p></figcaption></figure>

Repetir el mismo proceso con las capas disponibles.

{% hint style="info" %}
El software no reconoce los colores claros así que debemos reemplazar los colores amarillo y blanco o semejante a negro, manteniendo los nombres.
{% endhint %}

Para solucionar el problema cambiar el color de la capa a negro. Como se observa con ¨Jack frost blanco 2¨ y ¨Jack frost amarillo 2¨.

<figure><img src="broken-reference" alt=""><figcaption><p>Una vez obtenido la cantidad de capas de todos los colores pasamos al Plotter.</p></figcaption></figure>

<figure><img src="broken-reference" alt=""><figcaption><p>Cambio de color visto en la ventana en Inkscape.</p></figcaption></figure>

{% hint style="info" %}
En el caso de imprimir en el vinilo destinado a la impresión sobre tela se debe invertir la imagen de la dirección deseada con mirror para poder imprimir correctamente con el vinilo debimos al proceso posterior para impregnar el vinilo a la tela.&#x20;
{% endhint %}

<div>

<figure><img src="broken-reference" alt=""><figcaption><p>Herramienta mirror en Inkscape. </p></figcaption></figure>

 

<figure><img src="broken-reference" alt=""><figcaption><p>Imagen reflejada luego de utilizar Mirror.</p></figcaption></figure>

</div>

Ahora podemos utilizar este archivo en el Plotter.

<mark style="color:purple;">**Plotter**</mark>

Utilizaremos el siguiente plotter de la marca GCC modelo Puma IVLX .

<figure><img src="broken-reference" alt=""><figcaption><p>Imagen de la máquina que utilizaremos.</p></figcaption></figure>

Primero debemos encender la máquina con el interruptor.

<figure><img src="broken-reference" alt=""><figcaption><p>El interruptor está señalado con la flecha amarilla.</p></figcaption></figure>

{% embed url="https://modsproject.org" %}
Link URL a Modsproject.
{% endembed %}

<figure><img src="broken-reference" alt=""><figcaption><p>Vista de inicio de Modsproject.org</p></figcaption></figure>

<figure><img src="broken-reference" alt=""><figcaption><p>Zoom a las indicaciones.</p></figcaption></figure>

Como indica la página hacer click derecho en cualquier lugar de la pantalla para abrir un menú.&#x20;

<figure><img src="broken-reference" alt=""><figcaption><p>Menú después del click derecho.</p></figcaption></figure>

En este menú seleccionar **programs**. Luego se espandirá otro menú y debemos buscar el título **GCC** (marca del plotter que utilizamos en la documentación)  y seleccionar **gcc vinyl cut.**

<figure><img src="broken-reference" alt=""><figcaption><p>Seleccionamos <strong>gcc vinyl cut</strong>.</p></figcaption></figure>

Ahora tenemos un sistema de nodos programado para utilizar en con una máquina GCC.&#x20;

<figure><img src="broken-reference" alt=""><figcaption><p>Pantalla de nodos para utilizar con máquinas GCC.</p></figcaption></figure>

Ahora nos dirigiremos a los nodos que controlan los outputs. Apagaremos el slice de edit **delete (inferior)**, y prenderemos **edit delete (superior).** Digamos que debemos invertir el orden inicial.

<figure><img src="broken-reference" alt=""><figcaption><p>Edit delete inferior on, debemos cambiarlo a off.</p></figcaption></figure>

<figure><img src="broken-reference" alt=""><figcaption><p><strong>Edit delete superior</strong> on.</p></figcaption></figure>

Ahora cambiamos la velocidad y fuerza de corte. Los valores por efault son force (fuerza) 50 y speed (velocidad) 2. Después de unas pruebas determinamos que los ajutes que sí nos funciona con el material vinilo que tenemos es force 70 y speed 20.

<figure><img src="broken-reference" alt=""><figcaption><p>Valores de velocidad y fuerza por default.</p></figcaption></figure>

<figure><img src="broken-reference" alt=""><figcaption><p>Valores que funcionan con nuestro material.</p></figcaption></figure>

Ahora buscamos la nota de **Start Here** y debemos **select png file** para ingresar los .png que realizamos en Inkscape.

<figure><img src="broken-reference" alt=""><figcaption><p>Captura de pantalla del nodo para ingresar el .png</p></figcaption></figure>

<figure><img src="broken-reference" alt=""><figcaption><p>Menú emergente para seleccionar el .png a cortar en el plotter.</p></figcaption></figure>

<figure><img src="broken-reference" alt=""><figcaption><p>Vista luego de seleccionar. </p></figcaption></figure>

<figure><img src="broken-reference" alt=""><figcaption><p>vista del sistema de nodos una vez ingresado un .png</p></figcaption></figure>

Ahora debemos dirigirnos a **Cut Raster** y seleccionar **Calculate.**

<figure><img src="broken-reference" alt=""><figcaption><p>Nodo de Cut Raster.</p></figcaption></figure>

Ahora automáticamente se nos abrirá una ventana donde nos mostrará la trayectoria del corte, y también se nos descargará el archivo compatible para enviar al plotter.

<figure><img src="broken-reference" alt=""><figcaption><p>Trayectoria del corte de nuestra figura.</p></figcaption></figure>

<figure><img src="broken-reference" alt=""><figcaption><p>Se descargará el archivo automáticamente.</p></figcaption></figure>

Después de calcular podemos ver los cálculos que nos faltaban.

<figure><img src="broken-reference" alt=""><figcaption><p>Vista de los nodos después de calcular.</p></figcaption></figure>

<figure><img src="broken-reference" alt=""><figcaption><p>Zoom a los cálculos de Offset, Edge Detect, Orient Edges, Vectorize.</p></figcaption></figure>

Ahora debemos abrir el driver de la máquina Uploader.exe

<figure><img src="broken-reference" alt=""><figcaption><p>Vista de la búsqueda de Uploader </p></figcaption></figure>

Una vez que abrimos la aplicación debemos ingresar nuestras configuraciones correspondientes, es decir seleccionar el archivo que creamos en modsproject y seleccionar el port correspondiente.

<figure><img src="broken-reference" alt=""><figcaption><p>Las configuraciones por default del programa.</p></figcaption></figure>

<figure><img src="broken-reference" alt=""><figcaption><p>Seleccionamos el archivo .hpgl que cortaremos.</p></figcaption></figure>

<figure><img src="broken-reference" alt=""><figcaption><p>Cambiamos el Port a Common USB-8021.</p></figcaption></figure>

<figure><img src="broken-reference" alt=""><figcaption><p>Configuración preparada para cortar nuestra figura.</p></figcaption></figure>

## <mark style="color:blue;">**7- Dibujar con la plotter corte de vinilo**</mark>

<details>

<summary>Partes de la máquina a tener en cuenta</summary>

La cortadora que en este caso posee hoja filosa, aunque también se lo puede intercambiar por un lápiz, marcador o semejante para dibujar con el plotter.

![](broken-reference)

Las rueditas que sujetarán el material, además serán útil para la medición automática de la máquina.

![](broken-reference)

Son dos como se puede observar en la siguiente imagen.

![](broken-reference)

En la imagen anterior también podemos observar la regla. En la siguiente imagen podemos ver una imagen un poco mas expandida.

![](broken-reference)

La palanca para sujetar el material ingresado.

![](broken-reference)

Y por supuesto la botonera.

![](broken-reference)

</details>

A continuación se describen los pasos necesarios para utilizar la plotter de corte de vinilo, desde la preparación del material hasta la configuración de la máquina y el proceso de corte.

Seleccionar el vinilo a utilizar para cada capa del sticker.

<figure><img src="broken-reference" alt=""><figcaption><p>Baúl con vinilos a seleccionar.</p></figcaption></figure>

Podemos ingresar tal cual el pedazo de material si se encuentra en buen estado. Si se encuentra arrugado podemos pegarlo con cinta de papel a un objeto que nos sirva de tapete.

<figure><img src="broken-reference" alt=""><figcaption><p>Ejemplo de vinilo ubicado sobre un tapete improvisado (tapa de carpeta cortada) sujetado con cinta de papel.</p></figcaption></figure>

A continuación debemos levantar la palanca

<figure><img src="broken-reference" alt=""><figcaption><p>Palanca a levantar para ingresar el vinilo.</p></figcaption></figure>

Una vez ingresado el material debemos bajar la palanca nuevamente para sujetarlo.

Por supuesto al ubicar nuestro material debemos tener en cuenta el eje de origen para ubicar la hoja.

<figure><img src="broken-reference" alt=""><figcaption><p>Material ya ubicado en la máquina.</p></figcaption></figure>

Ahora debemos medir automáticamente el material, para ello debemos seleccionar el botón&#x20;

<figure><img src="broken-reference" alt=""><figcaption><p>Recién ingresado el material nos salen estas tres opciones en la pantalla.</p></figcaption></figure>

Nuestro objetivo es que la máquina mida el material ingresado de manera automática así que seleccionaremos la flecha que indica la derecha, ya que la opción para la medición automática es la opción **Single** que se observa en pantalla.&#x20;

A continuación nuestra máquina medirá la hoja de largo y ancho.

Una vez medido nuestro objetivo es ubicar el origen del eje en nuestro papel, para moverlo utilizamos las flechas y una vez que terminamos pulsamos enter.

<figure><img src="broken-reference" alt=""><figcaption><p>La pantalla indica un nuevo origen en las coordenadas indicadas.</p></figcaption></figure>

Ahora que terminamos de ubicar las coordenadas del origen para comenzar a cortar debemos dar la orden el el driver desde nuestra laptop o PC.

<figure><img src="broken-reference" alt=""><figcaption><p>Vista del driver en la pantalla.</p></figcaption></figure>

Para ejecutar la orden seleccionamos Start y el proceso comenzará.

<figure><img src="broken-reference" alt=""><figcaption><p>Seleccionar Start en el driver.</p></figcaption></figure>

De esta manera es el proceso para utilizar el plotter de corte.

<figure><img src="broken-reference" alt=""><figcaption><p>Vinilo Cortado con la forma que creamos.</p></figcaption></figure>

## <mark style="color:blue;">**5- Hacer sticker o dibujar imagen paramétrica**</mark>

Primero debemos tener todas nuestras piezas cortadas.

<figure><img src="broken-reference" alt=""><figcaption><p>Pieza cortada de negro.</p></figcaption></figure>

<figure><img src="broken-reference" alt=""><figcaption><p>Pieza cortada en blanco.</p></figcaption></figure>

<figure><img src="broken-reference" alt=""><figcaption><p>Pieza cortada en amarillo.</p></figcaption></figure>

<figure><img src="broken-reference" alt=""><figcaption><p>Vistas de piezas en conjunto.</p></figcaption></figure>

Ahora procedemos a ubicar las capas en orden para obtener la figura final.

<div>

<figure><img src="broken-reference" alt=""><figcaption><p>Capa amarilla sobre la capa anterior.</p></figcaption></figure>

 

<figure><img src="broken-reference" alt=""><figcaption><p>Primera capa color blanco.</p></figcaption></figure>

</div>

Siguiendo el proceso obtenemos un sticker de vinilo.

Nuestro primer intento quedó de la siguiente manera.

<figure><img src="broken-reference" alt=""><figcaption><p>Resultado del proceso.</p></figcaption></figure>

<figure><img src="broken-reference" alt=""><figcaption><p>Resultado final del intento.</p></figcaption></figure>

Creo que puede mejorar y me gustaría realizar otro intento.
