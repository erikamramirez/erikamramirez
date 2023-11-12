# Test de encastre



<table><thead><tr><th>Parámetros </th><th width="103">Medida </th></tr></thead><tbody><tr><td>Grosor del material</td><td>1.3 mm</td></tr><tr><td>Parámetro del intérvalo (10%)</td><td>0.13 mm</td></tr></tbody></table>

Cálculos para diseñar la prueba del encastre

<img src="../.gitbook/assets/file.excalidraw.svg" alt="" class="gitbook-drawing">

Para el diseño de nuestra pieza en Rhino, emplearé la herramienta de **Polyline** (polilínea) y **Join** (unir). Usar la barra de comandos agiliza este proceso para facilitar la selección de la herramienta.

<figure><img src="../.gitbook/assets/image (151).png" alt=""><figcaption></figcaption></figure>

Facilita el dibujo activar funciones como Osnap, End, Grid Snap, entre otros. En la imagen siguiente, se detallan los parámetros que estaban activos.

<figure><img src="../.gitbook/assets/Captura de pantalla 2023-11-08 164726.png" alt=""><figcaption></figcaption></figure>

Una vez finalizado podemos exportar nuestros vectores al formato necesario para abrir en **PowerCut**, entonces seleccionamos **File**, luego **Exportar como**, y elegimos el formato .dxf

<div>

<figure><img src="../.gitbook/assets/Captura de pantalla 2023-11-08 145435.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/imagen_2023-11-12_173615575.png" alt=""><figcaption></figcaption></figure>

</div>

## <mark style="color:purple;">Proceso en la Cabina de Corte Láser</mark>

Ubicamos el cartón gris y lo fijamos, prendemos la máquina y calibramos la cabeza del láser de ser necesario.

<div>

<figure><img src="../.gitbook/assets/imagen_2023-11-12_165412389.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/imagen_2023-11-12_170439452.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/imagen_2023-11-12_170508255.png" alt=""><figcaption></figcaption></figure>

</div>

Abrimos el Software **PowerCut**, seleccionamos **Load** y elegimos el archivo a procesar.

<div>

<figure><img src="../.gitbook/assets/imagen_2023-11-12_165926807.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/imagen_2023-11-12_165825378.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/imagen_2023-11-12_170009375.png" alt=""><figcaption></figcaption></figure>

</div>

Una vez abierto seleccionamos el ícono para ubicar en la esquina superior izquierda.

<div>

<figure><img src="../.gitbook/assets/imagen_2023-11-12_170025755.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/imagen_2023-11-12_170040995.png" alt=""><figcaption></figcaption></figure>

</div>

<figure><img src="../.gitbook/assets/imagen_2023-11-12_170654801.png" alt=""><figcaption></figcaption></figure>

También seleccionamos un color de capa y establecemos los parámetros de Modo (Cut), Velocidad (Speed: 15) y Power (fuerza: 50). Luego seleccionamos **LOAD** para exportar el archivo a la cortadora láser.

<div>

<figure><img src="../.gitbook/assets/imagen_2023-11-12_170115268.png" alt=""><figcaption><p>Ventana emergente de parámetros</p></figcaption></figure>

 

<figure><img src="../.gitbook/assets/imagen_2023-11-12_170205998.png" alt=""><figcaption></figcaption></figure>

</div>

En la ventana emergente establecemos un nombre corto y seleccionamos **Down File**, ahora hemos exportado nuestro archivo a la máquina.

<div>

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/imagen_2023-11-12_170305418.png" alt=""><figcaption></figcaption></figure>

</div>

Una vez actualizado el archivo a cortar en la máquina, ubicamos la posición del eje con las flechas, seleccionamos **FIXED**, una vez confirmado podemos seleccionar el botón verde para comenzar la operación.

<div>

<figure><img src="../.gitbook/assets/imagen_2023-11-12_165717040.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/imagen_2023-11-12_171931081.png" alt=""><figcaption></figcaption></figure>

</div>

Una vez terminado el proceso probamos qué parámetros que calculamos es el correcto para encastrar nuestras piezas según el grosor del material que poseemos.

<figure><img src="../.gitbook/assets/imagen_2023-11-12_165432903.png" alt=""><figcaption><p>Prueba de encastre</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-12_172315388.png" alt=""><figcaption><p>Nuestros cálculos iniciales</p></figcaption></figure>

Concluyendo este proyecto, nuestro análisis práctico determinó que, para un material de 1.3 mm, el grosor de encastre necesario es de <mark style="color:purple;">**0.91 mm**</mark>. Esta información fundamental servirá de guía para establecer los parámetros de diseño.
