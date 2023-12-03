---
description: >-
  Realizaremos un diseño paramétrico de un banco con Grasshopper y lo
  fabricaremos con CNC.
---

# Diseño paramétrico de un banco (Grasshopper)

El diseño paramétrico es una técnica avanzada que te permitirá crear modelos 3D flexibles y adaptables.&#x20;

Seguiremos el siguiente tutorial de un banco en Grasshopper.

{% embed url="https://www.youtube.com/watch?v=aQ0UIOf_50E" %}
Enlace al tutorial
{% endembed %}

El tutorial ya nos provee un archivo zip del trabajo.

{% file src="../../.gitbook/assets/parametricbench.zip" %}
Archivo de Grasshopper.
{% endfile %}

Debemos abrir el archivo y nos aparecerá un archivo de Grasshopper, al abrirlo nos aparecerán los nodos y la vista previa en el viewport de Rhino.

<figure><img src="../../.gitbook/assets/image (13) (1) (1) (1).png" alt=""><figcaption><p>Vista del archivo en el viewport.</p></figcaption></figure>

En el screenshot de abajo se puede ver la configuración de los nodos.

Posee parámetros de cambiar la forma de la curva, grosor de las unidades del material, cantidad de piezas a la izquierda y a la derecha.

<figure><img src="../../.gitbook/assets/image (9) (1) (1) (1).png" alt=""><figcaption><p>Vista de los nodos de Grasshopper.</p></figcaption></figure>

Decidí acortar la cantidad de piezas para ahorrar material en la construcción de la pieza, y también con el fin de personalizarlo.

<figure><img src="../../.gitbook/assets/imagen_2023-11-13_133734594.png" alt=""><figcaption></figcaption></figure>

Seleccionamos con click derecho el último nodo y seleccionamos Bake para obtener la malla del material.

<figure><img src="../../.gitbook/assets/imagen_2023-11-13_133822209.png" alt=""><figcaption></figcaption></figure>

Para obtener la figura 2D de este modelado 3D la forma que sí funciona es duplicar los bordes de las caras, para ello escribimos en la barra de comandos DupFaceBorder.

<figure><img src="../../.gitbook/assets/Captura de pantalla 2023-11-10 172708.png" alt=""><figcaption></figcaption></figure>

De esta forma obtenemos las figuras 2D de las piezas, las cuales convertiremos en .dxf para enviarlo en VCarve Pro.

<figure><img src="../../.gitbook/assets/Captura de pantalla 2023-11-13 140327.png" alt=""><figcaption></figcaption></figure>

Nuestra figura de la barra de intersección presentó problemas al realizar el  Sweep 1 **(barrido 1)**, por  ende su dibujo 2D tambien, consideré mejor utilizar **Trim (Cortar)** en la figura 2D para eliminar la parte sobrante, y luego unir con una nueva recta con **Join (Unir)**.

<div>

<figure><img src="../../.gitbook/assets/imagen_2023-11-13_140533797.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/imagen_2023-11-13_142231096.png" alt=""><figcaption></figcaption></figure>

</div>

No es mala idea utilizar la herramienta Texto o Text para escribir los números de las piezas, la cual se va a fresar superficialmente, para más adelante tener mayor facilidad al unir las piezas.

<div>

<figure><img src="../../.gitbook/assets/imagen_2023-11-13_142523796.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/imagen_2023-11-13_142647188.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/imagen_2023-11-13_142647188 (1).png" alt=""><figcaption></figcaption></figure>

</div>

<figure><img src="../../.gitbook/assets/imagen_2023-11-13_143157040.png" alt=""><figcaption></figcaption></figure>

{% file src="../../.gitbook/assets/Grasshopper nuevo silla.3dm" %}
Archivo de Rhino.
{% endfile %}

{% file src="../../.gitbook/assets/Silla Grasshopper.dxf" %}
Archivo .dxf
{% endfile %}



**Tutorial similar**

{% embed url="https://www.youtube.com/watch?v=gJ3KB0IY9pk" %}

