---
description: >-
  En esta sección procesaremos el archivo creado en Inkscape para crear un
  sticker utilizando el Plotter para cortar el vinilo.
---

# Corte de vinilo con Plotter

Utilizaremos el siguiente plotter de la marca GCC modelo Puma IVLX .

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_205654712.png" alt=""><figcaption><p>Imagen de la máquina que utilizaremos.</p></figcaption></figure>

Primero debemos encender la máquina con el interruptor.

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_205707693.png" alt=""><figcaption><p>El interruptor está señalado con la flecha amarilla.</p></figcaption></figure>

{% embed url="https://modsproject.org" %}
Link URL a Modsproject.
{% endembed %}

<figure><img src="../../.gitbook/assets/image (2) (1).png" alt=""><figcaption><p>Vista del inicio de Modsproject.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_205816845.png" alt=""><figcaption><p>Zoom a las indicaciones.</p></figcaption></figure>

Como indica la página hacer click derecho en cualquier lugar de la pantalla para abrir un menú.&#x20;

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_205850684.png" alt=""><figcaption><p>Menú después del click derecho.</p></figcaption></figure>

En este menú seleccionar **programs**. Luego se espandirá otro menú y debemos buscar el título **GCC** (marca del plotter que utilizamos en la documentación)  y seleccionar **gcc vinyl cut.**

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_205901516.png" alt=""><figcaption><p>Seleccionamos <strong>gcc vinyl cut</strong>.</p></figcaption></figure>

Ahora tenemos un sistema de nodos programado para utilizar en con una máquina GCC.

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_205911890.png" alt=""><figcaption><p>Pantalla de nodos para utilizar con máquinas GCC.</p></figcaption></figure>

Ahora nos dirigiremos a los nodos que controlan los outputs. Apagaremos el slice de edit **delete (inferior)**, y prenderemos **edit delete (superior).** Digamos que debemos invertir el orden inicial.

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_210036132.png" alt=""><figcaption><p>Edit delete inferior on, debemos cambiarlo a off.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_210046756.png" alt=""><figcaption><p><strong>Edit delete superior</strong> on.</p></figcaption></figure>

Ahora cambiamos la velocidad y fuerza de corte. Los valores por efault son force (fuerza) 50 y speed (velocidad) 2. Después de unas pruebas determinamos que los ajutes que sí nos funciona con el material vinilo que tenemos es force 70 y speed 20.

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_210115275.png" alt=""><figcaption><p>Valores de velocidad y fuerza por default.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_210125796.png" alt=""><figcaption><p>Valores que funcionan con nuestro material.</p></figcaption></figure>

Ahora buscamos la nota de **Start Here** y debemos **select png file** para ingresar los .png que realizamos en Inkscape.

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_210218661.png" alt=""><figcaption><p>Captura de pantalla del nodo para ingresar el .png</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_210232447.png" alt=""><figcaption><p>Menú emergente para seleccionar el .png a cortar en el plotter.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (3) (1).png" alt=""><figcaption><p>Vista luego de seleccionar. </p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (4) (1).png" alt=""><figcaption><p>Vista del sistema de nodos una vez ingresado el .png </p></figcaption></figure>

Ahora debemos dirigirnos a **Cut Raster** y seleccionar **Calculate.**

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_210523195.png" alt=""><figcaption><p>Nodo de Cut Raster.</p></figcaption></figure>

Ahora automáticamente se nos abrirá una ventana donde nos mostrará la trayectoria del corte, y también se nos descargará el archivo compatible para enviar al plotter.

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_210534584.png" alt=""><figcaption><p>Trayectoria del corte de nuestra figura.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_210545001.png" alt=""><figcaption><p>Se descargará el archivo automáticamente.</p></figcaption></figure>

Después de calcular podemos ver los cálculos que nos faltaban.

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_210643941.png" alt=""><figcaption><p>Vista de los nodos después de calcular.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_210654764.png" alt=""><figcaption><p>Zoom a los cálculos de Offset, Edge Detect, Orient Edges, Vectorize.</p></figcaption></figure>

## Ahora debemos abrir el driver de la máquina Uploader.exe

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_210829976.png" alt=""><figcaption><p>Vista de la búsqueda de Uploader </p></figcaption></figure>

Una vez que abrimos la aplicación debemos ingresar nuestras configuraciones correspondientes, es decir seleccionar el archivo que creamos en modsproject y seleccionar el port correspondiente.

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_210839494.png" alt=""><figcaption><p>Las configuraciones por default del programa.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_210850831.png" alt=""><figcaption><p>Seleccionamos el archivo .hpgl que cortaremos.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_210901536.png" alt=""><figcaption><p>Cambiamos el Port a Common USB-8021.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_210913383.png" alt=""><figcaption><p>Configuración preparada para cortar nuestra figura.</p></figcaption></figure>

## Corte con el Plotter de Vinilo

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

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_212723961.png" alt="" width="375"><figcaption><p>Baúl con vinilos a seleccionar.</p></figcaption></figure>

Podemos ingresar tal cual el pedazo de material si se encuentra en buen estado. Si se encuentra arrugado podemos pegarlo con cinta de papel a un objeto que nos sirva de tapete.

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_212740278.png" alt="" width="375"><figcaption><p>Ejemplo de vinilo ubicado sobre un tapete improvisado (tapa de carpeta cortada) sujetado con cinta de papel.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_212941458.png" alt="" width="375"><figcaption><p>Palanca a levantar para ingresar el vinilo.</p></figcaption></figure>

Una vez ingresado el material debemos bajar la palanca nuevamente para sujetarlo.

Por supuesto al ubicar nuestro material debemos tener en cuenta el eje de origen para ubicar la hoja.

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_213054417 (3).png" alt="" width="375"><figcaption><p>Material ya ubicado en la máquina.</p></figcaption></figure>

Ahora debemos medir automáticamente el material, para ello debemos seleccionar el botón&#x20;

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_213208899 (1).png" alt="" width="563"><figcaption><p>Recién ingresado el material nos salen estas tres opciones en la pantalla.</p></figcaption></figure>

Nuestro objetivo es que la máquina mida el material ingresado de manera automática así que seleccionaremos la flecha que indica la derecha, ya que la opción para la medición automática es la opción **Single** que se observa en pantalla.&#x20;

A continuación nuestra máquina medirá la hoja de largo y ancho.

Una vez medido nuestro objetivo es ubicar el origen del eje en nuestro papel, para moverlo utilizamos las flechas y una vez que terminamos pulsamos enter.

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_213336251 (1).png" alt="" width="563"><figcaption><p>La pantalla indica un nuevo origen en las coordenadas indicadas.</p></figcaption></figure>

Ahora que terminamos de ubicar las coordenadas del origen para comenzar a cortar debemos dar la orden el el driver desde nuestra laptop o PC.

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_213420635.png" alt="" width="375"><figcaption><p>Vista del driver en la pantalla.</p></figcaption></figure>

Para ejecutar la orden seleccionamos Start y el proceso comenzará.

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_213445334.png" alt=""><figcaption><p>Seleccionar Start en el driver.</p></figcaption></figure>

De esta manera es el proceso para utilizar el plotter de corte.

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_213542560.png" alt="" width="375"><figcaption><p>Vinilo Cortado con la forma que creamos.</p></figcaption></figure>

## Juntar los cortes en una sola figura

Primero debemos tener todas nuestras piezas cortadas.

<div>

<figure><img src="../../.gitbook/assets/image (131).png" alt="" width="375"><figcaption><p>Capa negra.</p></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_214106562.png" alt="" width="375"><figcaption><p>Capa blanca.</p></figcaption></figure>

</div>

<div>

<figure><img src="../../.gitbook/assets/image (132).png" alt=""><figcaption><p>Pieza amarilla.</p></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_214226177.png" alt=""><figcaption><p>Vista de las piezas juntas.</p></figcaption></figure>

</div>

Ahora procedemos a ubicar las capas en orden para obtener la figura final.

<div>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_214353993.png" alt=""><figcaption><p>Capa amarilla sobre la capa anterior.</p></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_214408541.png" alt=""><figcaption><p>Primera capa color blanco.</p></figcaption></figure>

</div>

Siguiendo el proceso obtenemos un sticker de vinilo.

Nuestro primer intento quedó de la siguiente manera.

<div>

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_214442511 (1).png" alt="" width="375"><figcaption><p>Resultado del proceso.</p></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/imagen_2023-11-04_214500219.png" alt="" width="375"><figcaption></figcaption></figure>

</div>

Creo que puede mejorar y me gustaría realizar otro intento.
