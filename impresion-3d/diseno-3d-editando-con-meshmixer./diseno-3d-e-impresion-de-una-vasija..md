---
description: >-
  Para el diseño utilizaremos Grasshopper, y para el procesamiento para la
  impresión utilizaremos Flashprint y Meshmixer.
---

# Diseño 3D e Impresión de una vasija.

{% embed url="https://www.instructables.com/Customizable-Low-Poly-Vase-With-Grasshopper-Walk-t/" %}
Link para descargar el modelo a imprimir.
{% endembed %}

Una vez que descargamos el archivo procedemos a abrir Rhino, luego Grasshopper para abrir el documento.

&#x20;A continuación modificar los parámetros.

<figure><img src="../../.gitbook/assets/image (14) (1) (1) (1) (1).png" alt=""><figcaption><p>Vista de los nodos en Grasshopper.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (15) (1) (1) (1) (1).png" alt=""><figcaption><p>Vista del modelo de los scripts realizados en Grasshopper vistos del viewport.</p></figcaption></figure>

El autor del trabajo especifica los pasos a seguir.

<figure><img src="../../.gitbook/assets/image (17) (1) (1) (1) (1).png" alt=""><figcaption><p>Pasos a seguir señalizados.</p></figcaption></figure>

En la zona inferior encontramos los nodos de parámetros modificables.

La unidad utilizada es centímetros.

Los parámetros son:

* Altura
* Cantidad de segmentos.
* Lados.
* Giro.
* Radio de la tapa inferior.
* Radio de la tapa superior.
* Subdivisiones de paneles.
* Grosor.

<figure><img src="../../.gitbook/assets/image (16) (1) (1) (1) (1).png" alt=""><figcaption><p>Vista de los parámetros modificables.</p></figcaption></figure>

Procedemos a configurar los parámetros predeterminados por el autor a nuestro parecer.&#x20;

<figure><img src="../../.gitbook/assets/image (19) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Para crear el modelo debemos realizar bake en el nodo final de nuestro script.

{% hint style="info" %}
El término ¨Bake¨ (hornear objetos) en Grasshopper y Rhino se refiere al proceso de transferir o convertir la geometría digital que creas en Grasshopper en objetos o superficies físicas en el entorno de modelado de Rhino.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (20) (1).png" alt=""><figcaption><p>Nodo el cual debemos realizar bake.</p></figcaption></figure>

Procedemos a hacer click derecho en el nodo, y seleccionamos Bake.

<figure><img src="../../.gitbook/assets/image (21) (1).png" alt=""><figcaption></figcaption></figure>

Al seleccionar nos aparece una pestaña emergente, en la que añadiremos el nombre, y seleccionaremos la casilla de Agrupar. Luego seleccionamos ok.

<figure><img src="../../.gitbook/assets/image (22) (1).png" alt=""><figcaption><p>Vista de la pestaña emergente.</p></figcaption></figure>

Una vez terminado el proceso anterior, obtendremos el modelo en el viewport.

<figure><img src="../../.gitbook/assets/image (23) (1).png" alt=""><figcaption><p>Meshes alejados de la vista previa del script de Grasshopper (lila)</p></figcaption></figure>

Una vez realizado podemos eliminar la pestaña de Grasshopper.

Ya que mi intensión es que el modelo sirva de maceta. Crearemos un círculo en la tapa inferior y lo extruiremos, y después realizaremos una diferencia boleana.

<figure><img src="../../.gitbook/assets/image (24) (1).png" alt=""><figcaption><p>Podemos observar una curva de círculo en el centro.</p></figcaption></figure>

Extruimos el círculo, y después tapamos con ¨cap¨, de esta manera creamos un mesh con el que podemos proceder a crear una diferencia boleana.

<figure><img src="../../.gitbook/assets/image (96).png" alt=""><figcaption><p>Vista del cilindro en el viewport.</p></figcaption></figure>

En teoría ahora podríamos realizar una diferencia boleana, sin embargo tuve problemas con el objeto creado con Grasshopper.

<figure><img src="../../.gitbook/assets/image (97).png" alt=""><figcaption><p>ícono de Boolean Difference.</p></figcaption></figure>

La solución consistió en exportar ya el objeto y el cilindro a Meshmixer.

{% hint style="info" %}
Para exportar los archivos de Rhino a Meshmixer es necesario exportar como .stl
{% endhint %}

<figure><img src="../../.gitbook/assets/image (98).png" alt=""><figcaption><p>Exportar como .stl</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (100).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (99).png" alt=""><figcaption><p>El modelo se ve deformado con menos polígonos en el viewport de Meshmixer.</p></figcaption></figure>

La diferencia boleana se pudo realizar en Meshmixer y una vez terminado, exportamos el modelo a Flashprint, con la intención de imprimir.

También podemos aumentar la cantidad de polígonos en Meshmixer para lograr mayor exactitud en la impresión.

**Exportar a Flashprint**

Si el modelo es demasiado grande se debe escalar para que entre en el cubo que se observa en el viewport.

<figure><img src="../../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Modelo 3D dentro del cubo en el viewport.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (5) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Modelo 3D que sobrepasa el tamaño del cubo, por ende es necesario escalar.</p></figcaption></figure>

Debemos aumentar aumentar la calidad de polígonos del mesh para mayor precisión en nuestra impresión.

<figure><img src="../../.gitbook/assets/image (4) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Modelo 3D con mayor cantidad de polígonos.</p></figcaption></figure>

{% hint style="info" %}
A tener en cuenta la reducción de polígonos luego de haber aumentado, hasta encontrar el equilibrio entre una gran cantidad de polígonos y la capacidad a procesar por la notebook y la propia impresora 3D.
{% endhint %}

Antes de enviar el objeto a la máquina debemos configurar algunos parámetros. Por ejemplo la temperatura de la extrusora, en este caso sólo usaremos la derecha por lo que sólo especificaremos la temperatura derecha a 220 grados.

También determinaremos la temperatura a calentar la plataforma, en este caso 60 grados.

{% hint style="info" %}
La temperatura de la extrusora se determina de acuerdo al material que utilizaremos.
{% endhint %}

El tamaño de la boquilla que tenemos es de 0.4 mm.

<figure><img src="../../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Configuraciones listas para exportar a la máquina.</p></figcaption></figure>

En esta impresora debemos exportar los archivos y configuraciones por medio de una tarjeta MicroSD.

<figure><img src="../../.gitbook/assets/93acadf1-2d2a-4ec8-baa1-879eb382897e.jpg" alt=""><figcaption><p>Vista de la tarjeta MicroSD.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/47e8ebd4-dfdf-4ef2-87bc-a5a20dabdd4a.jpg" alt=""><figcaption><p>Vista de la tarjeta MicroSD ingresada en la máquina.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (6) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Vista de la máquina 3D que utilizaremos.</p></figcaption></figure>

En la imagen superior observamos la plataforma, para empezar debemos subir esta plataforma más próximo a la extrusora.

<figure><img src="../../.gitbook/assets/image (7) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>En esta imagen podemos ver la plataforma acercada a la extrusora.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/WhatsApp Image 2023-10-29 at 12.00.26 (2).jpeg" alt=""><figcaption><p>Seleccionar Tools.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/WhatsApp Image 2023-10-29 at 12.26.54.jpeg" alt=""><figcaption><p>Seleccionar Manual.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (45).png" alt=""><figcaption><p>Mover la plataforma en el eje z y después retroceder.</p></figcaption></figure>

Por supuesto debemos limpiar la plataforma de ser necesario, podemos utilizar alguna herramienta para raspar algún pedazo de plástico.

<figure><img src="../../.gitbook/assets/WhatsApp Image 2023-10-29 at 12.00.16.jpeg" alt=""><figcaption><p>Limpieza de la plataforma.</p></figcaption></figure>

Si no vamos a reemplazar el color del filamento podemos proceder directamente a Print.

<div>

<figure><img src="../../.gitbook/assets/WhatsApp Image 2023-10-29 at 12.00.26 (2) (2).jpeg" alt=""><figcaption><p>Seleccionar Print.</p></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/WhatsApp Image 2023-10-29 at 12.00.26 (3).jpeg" alt=""><figcaption><p>Seleccionar el ícono de Tarjeta MicroSD.</p></figcaption></figure>

</div>

<div>

<figure><img src="../../.gitbook/assets/WhatsApp Image 2023-10-26 at 14.58.40 (1).jpeg" alt=""><figcaption><p>Seleccionar el objeto a imprimir.</p></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/WhatsApp Image 2023-10-30 at 03.09.54.jpeg" alt=""><figcaption><p>Confirmar la impresión con Print.</p></figcaption></figure>

</div>

La máquina comenzará su proceso y esperaremos hasta obtener el objeto impreso.

Las vistas del objeto final son las siguientes.

<figure><img src="../../.gitbook/assets/WhatsApp Image 2023-10-29 at 12.00.18 (1).jpeg" alt=""><figcaption><p>Resultado satisfactorio en relación a la apariencia del filamento.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/WhatsApp Image 2023-10-29 at 12.00.19.jpeg" alt=""><figcaption><p>El agujero inferior se encuentra obstruido y debemos perforarlo para terminar el proyecto como fue planteado.</p></figcaption></figure>

¡Gracias por seguir este tutorial!

¡Espero que este tutorial te haya sido de utilidad! Si tienes alguna pregunta o necesitas más ayuda, no dudes en contactarnos. ¡Gracias por leer y buena suerte en tus proyectos futuros!
