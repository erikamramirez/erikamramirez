---
description: >-
  En esta sección se documentará el proceso, incluyendo los errores, ajustes en
  el diseño y en el proceso de corte de una lámpara paramétrica fabricada con
  cartón gris.
cover: ../.gitbook/assets/imagen_2023-11-12_010202012.png
coverY: 0
layout:
  cover:
    visible: true
    size: hero
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Lámpara cortada en cartón gris

## <mark style="color:purple;">Proceso de Corte</mark>

Abriremos nuestro programa PowerCut, luego importaremos nuestro archivo .dxf que contiene nuestros vectores.

<div>

<figure><img src="../.gitbook/assets/image (165).png" alt=""><figcaption><p>Ícono Load a seleccionar para importar el archivo.</p></figcaption></figure>

 

<figure><img src="../.gitbook/assets/imagen_2023-11-12_001745618.png" alt=""><figcaption></figcaption></figure>

</div>

Una vez abierto seleccionaremos el conjunto total y seleccionamos el ícono de ubicar a la esquina superior izquierda.

<div>

<figure><img src="../.gitbook/assets/imagen_2023-11-12_001424951.png" alt=""><figcaption><p>Posición original de los vectores.</p></figcaption></figure>

 

<figure><img src="../.gitbook/assets/imagen_2023-11-12_001525293.png" alt=""><figcaption><p>Conjunto ubicado en la esquina superior izquierda.</p></figcaption></figure>

</div>

<figure><img src="../.gitbook/assets/imagen_2023-11-12_001547902.png" alt=""><figcaption><p>Abajo de los cuadrados de colores para asignar las capas de los vectores, encontramos los íconos para ubicar en el centro o en las esquinas, también tipos de justificación.</p></figcaption></figure>

También seleccionamos los vectores a cortar y asignamos una capa con los parámetros de velocidad y potencia para cortar según nuestro material, en este caso el cartón gris.

<figure><img src="../.gitbook/assets/imagen_2023-11-12_001615910.png" alt="" width="243"><figcaption></figcaption></figure>

Seleccionamos **Load**, asignamos un nombre corto y luego procedemos con **Down File**.

<figure><img src="../.gitbook/assets/imagen_2023-11-12_001639684.png" alt="" width="211"><figcaption></figcaption></figure>

Una vez enviado el archivo, el dibujo nos aparece en la pantalla, debemos ubicar en el material el eje, seleccionar fixed y luego iniciar la operación de corte.

<figure><img src="../.gitbook/assets/imagen_2023-11-12_001652552.png" alt=""><figcaption></figcaption></figure>



{% hint style="danger" %}
**¿Qué salió mal?**

Las líneas generadas en Rhino para indicar que se trata de un mesh se ha exportado como vector, no me he percatado y lo tenía que eliminar antes de exportarlo, como no lo he hecho se ha cortado esas líneas también
{% endhint %}

### <mark style="color:purple;">Rediseño y Nuevo Intento</mark>

Repetí el proceso con el archivo corregido pero, el diseño simplemente no funciona y necesita unos cambios

<div>

<figure><img src="../.gitbook/assets/imagen_2023-11-12_001708175.png" alt=""><figcaption><p>Vista de las piezas con las líneas inesperadas ya eliminadas.</p></figcaption></figure>

 

<figure><img src="../.gitbook/assets/imagen_2023-11-12_005510527.png" alt="" width="563"><figcaption><p>Resultado del mal diseño</p></figcaption></figure>

</div>

Para mejorar el diseño de la lámpara, amplié las piezas para soportar su propio peso y alargué el espacio para encastrarlas. Aunque el grosor para encastrar es adecuado, la distancia de profundidad no resultó ideal.



{% hint style="warning" %}
**Nuevo descuido**

Me olvidé de duplicar las piezas.
{% endhint %}

<figure><img src="../.gitbook/assets/imagen_2023-11-12_002337831.png" alt=""><figcaption></figcaption></figure>

Como corté las primeras dos piezas, y recién ahí me di cuenta lo que faltaba, se ve otro nuevo archivo de las piezas que restaba cortar.

<figure><img src="../.gitbook/assets/imagen_2023-11-12_002407769.png" alt=""><figcaption></figcaption></figure>

Una vez terminado el proceso de corte procedemos a ensamblar las piezas

<figure><img src="../.gitbook/assets/imagen_2023-11-12_002425191.png" alt=""><figcaption></figcaption></figure>

Diversos factores influyen en el corte correcto de nuestro material, tanto como las propias mañas de nuestra máquina, la cuál funciona correctamente en la esquina superior izquierda, pero en el centro suele presentar problemas, en este caso vemos que una pieza alejada de la zona superior izquierda no se cortó correctamente, para obtener lo que nos falta, cambiamos de ubicación del eje a la zona lateral izquierda y procesamos los pasos que ya conocemos para obtener la pieza que nos falta.

<div>

<figure><img src="../.gitbook/assets/imagen_2023-11-12_002441224.png" alt=""><figcaption><p>Pieza sin cortar.</p></figcaption></figure>

 

<figure><img src="../.gitbook/assets/imagen_2023-11-12_012041910.png" alt=""><figcaption><p>Ubicamos el eje en la zona lateral y cortamos esa pieza faltante.</p></figcaption></figure>

</div>

Ahora que obtuvimos la pieza faltante, terminamos de ensamblar ¡y finalmente obtenemos nuestro proyecto completo!

## <mark style="color:purple;">Resultado Final</mark>

<div>

<figure><img src="../.gitbook/assets/imagen_2023-11-12_001012652 (1).png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/imagen_2023-11-12_000847690.png" alt=""><figcaption></figcaption></figure>

</div>
