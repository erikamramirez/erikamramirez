---
description: >-
  Descargaremos e imprimiremos un objeto o modelo 3D diseñado específicamente
  para probar y calibrar la impresora 3D, o para evaluar la calidad de impresión
  de la máquina.
cover: ../.gitbook/assets/WhatsApp Image 2023-10-29 at 12.26.48 (2).jpeg
coverY: -58
---

# Descarga e Impresión de un test de impresión.

{% embed url="https://www.printables.com/en/model/159768-bat-cali-cat-man/files" %}
Link del modelo que utilizaremos.
{% endembed %}

Descargaremos el test de impresión en este caso de Printables, en este caso seleccioné el test BatCaliCat-Man realizado por Alex Ronda.

Es una versión de CaliCat muy llamativo y ciertamente tierno.

<figure><img src="../.gitbook/assets/image (64).png" alt=""><figcaption><p>Vista de la interface del enlace.</p></figcaption></figure>

El modelo consta de múltiples piezas.

* El modelo del gato
* Una capa
* Un casco
* El símbolo de Batman&#x20;

<figure><img src="../.gitbook/assets/image (62).png" alt=""><figcaption><p>Vista de los modelos por separado.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (63).png" alt=""><figcaption><p>Lista de modelos descargables en el enlace.</p></figcaption></figure>

El modelo ya está preparado para imprimirlo, no le realizaremos cambios, ni aumentaremos los polígonos.

A continuación exportaremos el archivo de BatCaliCat-man que descargamos, para ellos entramos en **Archivo**, **Cargar Archivo** y seleccionamos.

<figure><img src="../.gitbook/assets/image (83).png" alt=""><figcaption><p>Vista de la interface de Flashprint.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (84).png" alt=""><figcaption><p>Archivo ya exportado en Flashprint.</p></figcaption></figure>

Seleccionamos **Iniciar corte** y nos abrirá un menú emergente.&#x20;

<figure><img src="../.gitbook/assets/image (73).png" alt=""><figcaption><p>Seleccionar <strong>Iniciar Corte</strong>.</p></figcaption></figure>

Al abrir por primera vez el menú nos aparecerá las opciones simplificadas, debemos seleccionar el **Modo Experto** para continuar.

<figure><img src="../.gitbook/assets/image (85).png" alt=""><figcaption><p>Vista del menú emergente.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (74).png" alt=""><figcaption><p>Menú emergente <strong>Modo Experto.</strong></p></figcaption></figure>

Prestaremos especial atención a la temperatura de la extrusora que utilizaremos (en este caso la derecha) y la temperatura de la plataforma, estos parámetros se tienen en cuenta según la etiqueta del filamento que poseemos.

<figure><img src="../.gitbook/assets/WhatsApp Image 2023-10-29 at 12.00.19 (1) (1).jpeg" alt=""><figcaption><p> Vista de Filamentos varios.</p></figcaption></figure>

{% tabs %}
{% tab title="Filamento de PLA" %}
<figure><img src="../.gitbook/assets/image (75).png" alt=""><figcaption><p>Filamento Blanco PLA.</p></figcaption></figure>

Extrusor: 183-238.

Plataforma:28-68.
{% endtab %}

{% tab title="Filamento de PLA " %}
<figure><img src="../.gitbook/assets/WhatsApp Image 2023-10-29 at 12.26.55 (1).jpeg" alt=""><figcaption><p>Vista del filamento azul.</p></figcaption></figure>

Extrusor: 190-230.

Plataforma: 50.
{% endtab %}

{% tab title="Filamento ABS." %}
<figure><img src="../.gitbook/assets/WhatsApp Image 2023-10-29 at 12.26.55.jpeg" alt=""><figcaption><p>Filamento ABS.</p></figcaption></figure>

Extrusor: 220.
{% endtab %}

{% tab title="Filamento PETG" %}

{% endtab %}
{% endtabs %}

Configuraremos la temperatura con los siguientes parámetros.

<figure><img src="../.gitbook/assets/image (76).png" alt=""><figcaption><p>Parámetros de temperatura utilizados en el tutorial.</p></figcaption></figure>

Nos dirigiremos al menú lateral izquierdo y nos vamos a la pestaña de **Estructuras**.&#x20;

<figure><img src="../.gitbook/assets/image (27) (1).png" alt=""><figcaption><p>Vista del menú lateral.</p></figcaption></figure>

La razón es para poder empezar la impresión de **Interior a Exterior** en **Orden de impresión de la carcasa**, de esta manera si el filamento sale de manera indeseada al principio, no perjudicará el resultado final, por que la temperatura se estabilizará al imprimir el exterior.

También cambiaremos el **Modo** a usar **puntos de inicio aleatorios**, de esta manera evitamos que nuestro modelo tenga un aspecto de zipper o de cierre visible en el punto de inicio.

<figure><img src="../.gitbook/assets/image (28) (1).png" alt=""><figcaption><p>Vista de parámetros cambiados en la pestaña de <strong>Estructuras</strong>.</p></figcaption></figure>

En el menú lateral derecho nos encontramos con diversas opciones, seleccioné **Guardar Configuración** para imprimir con los parámetros establecidos próximos objetos, teniendo en cuenta si utilizaremos el mismo filamento.

Finalmente seleccionamos **Corte**.

<figure><img src="../.gitbook/assets/image (29) (1).png" alt=""><figcaption><p>Vista del menú lateral derecho.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (32).png" alt=""><figcaption><p>Se procesará hasta obtener un resultado exportable.</p></figcaption></figure>

Al seleccionar Vista previa de corte podremos ver el objeto laminado, los tipos de rellenos categorizados por colores automáticamente, la duración de tiempo que tomará la impresión.

<figure><img src="../.gitbook/assets/image (33).png" alt=""><figcaption><p>Vista del menú superior después del corte.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (34).png" alt=""><figcaption><p>Vista de la interface luego de seleccionar <strong>Vista previa de corte.</strong></p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (35).png" alt=""><figcaption><p>Podemos ver dónde se utilizará cada tipo de relleno señalizado según colores automáticamente.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (36).png" alt=""><figcaption><p>Es un dato importante la estimación de impresión que tomará el modelo en la máquina.</p></figcaption></figure>

A continuación seleccionamos **Guardar en local** para descargar el archivo en un formato aceptable por la impresora 3D, el formato \*.gx, y con los parámetros que establecimos.

<figure><img src="../.gitbook/assets/image (37).png" alt=""><figcaption><p>Debemos seleccionar el ícono de <strong>Guardar en local.</strong></p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (90).png" alt=""><figcaption><p>Se guardará en formato *.gx</p></figcaption></figure>

Ahora debemos exportar el documento .gx a la memoria SD de la impresora.

<figure><img src="../.gitbook/assets/image (38).png" alt=""><figcaption><p>Entrada MicroSD en una notebook.</p></figcaption></figure>

{% hint style="info" %}
<img src="../.gitbook/assets/image (39).png" alt="" data-size="original">

Hay que tener en cuenta que las notebooks más actuales no suelen contar con esta entrada, en caso de necesitarlo existen adaptadores en el mercado.
{% endhint %}

Prender la máquina e ingresar de nuevo la tarjeta SD.

<div>

<figure><img src="../.gitbook/assets/47e8ebd4-dfdf-4ef2-87bc-a5a20dabdd4a (1).jpg" alt=""><figcaption><p>Entrada de la tarjeta MicroSD en la impresora 3D.</p></figcaption></figure>

 

<figure><img src="../.gitbook/assets/93acadf1-2d2a-4ec8-baa1-879eb382897e (1).jpg" alt=""><figcaption><p>Tarjeta MicroSD.</p></figcaption></figure>

</div>

Como está conectado el plástico azul, y quiero reemplazar el filamento a otro color debemos calentar primero el extrusor derecho para poder extraer el anterior.

Los pasos a realizar son:

<figure><img src="../.gitbook/assets/imagen_2023-11-11_022323787.png" alt=""><figcaption><p>Este es el menú principal al que accederemos constantemente. Seleccionamos Preheat.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-11_022456549 (2).png" alt=""><figcaption><p>Desactivamos (off) lo que no queremos que se caliente, y activamos (on) lo que sí queremos calentar, en este caso el Extrusor derecho/ R Extruder.</p></figcaption></figure>

<div>

<figure><img src="../.gitbook/assets/imagen_2023-11-11_022520275.png" alt=""><figcaption><p>Debemos calentar el extrusor derecho, los parámetros serán los establecidos en Flashprint.</p></figcaption></figure>

 

<figure><img src="../.gitbook/assets/imagen_2023-11-11_022535160.png" alt=""><figcaption></figcaption></figure>

</div>

Una vez que se termina de calentar el extrusor. Apretamos la palanca que se encuentra al lateral del extrusor, y a la par empujamos el filamento. Una vez expulsado los restos del filamento anterior, podemos abrir la rejilla y quitar los restos.

<figure><img src="../.gitbook/assets/image (42).png" alt=""><figcaption><p>Vista del filamento ingresado en el extrusor derecho, y a su costado la palanca mencionada.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (43).png" alt=""><figcaption><p>Zoom a la palanca a apretar con fuerza mientras empujamos el filamento.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/WhatsApp Image 2023-10-26 at 16.16.51 (1).jpeg" alt=""><figcaption><p>Podemos utilizar herramientas para cortar el resto de filamento o extraerlo de la plataforma en caso de quedarse pegado.</p></figcaption></figure>

Una vez que se haya terminado el proceso anterior y haber cambiado el filamento de haber sido necesario, podemos continuar.

**Mover la plataforma para acercarlo al extrusor.**

Para mover la plataforma debemos seleccionar tools en el menú principal, luego move, y mover la plataforma en el eje Z para acercalo al extrusor.

<figure><img src="../.gitbook/assets/imagen_2023-11-11_022230973.png" alt=""><figcaption><p>Seleccionar Tools en el menú principal.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/WhatsApp Image 2023-10-29 at 12.26.54.jpeg" alt=""><figcaption><p>Menú Tools.</p></figcaption></figure>

{% hint style="info" %}
Podemos seleccionar **Level** para nivelar la plataforma en relación al extrusor y luego mover la plataforma para **alejarlo** del extrusor.

<img src="../.gitbook/assets/imagen_2023-11-11_023052475.png" alt="" data-size="original">
{% endhint %}

Seleccionar Manual para mover la plataforma, movemos en el eje z para alejar o acercar al extrusor. Establecemos una distancia aceptable entre ambos y luego retrocedemos.

<figure><img src="../.gitbook/assets/imagen_2023-11-11_022300603.png" alt=""><figcaption><p>Vista del menú de <strong>Manual</strong>.</p></figcaption></figure>

Cuando queremos empezar la impresión volvemos en el menú principal y seleccionamos Print.

<figure><img src="../.gitbook/assets/imagen_2023-11-11_022323787.png" alt=""><figcaption><p>Seleccionar <strong>Print</strong>.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-11_022204905.png" alt=""><figcaption><p>Seleccionar el ícono de la tarjeta Micro SD.</p></figcaption></figure>

<div>

<figure><img src="../.gitbook/assets/imagen_2023-11-11_022743576.png" alt=""><figcaption><p>Seleccionar el modelo que queremos imprimir.</p></figcaption></figure>

 

<figure><img src="../.gitbook/assets/imagen_2023-11-11_022801346.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/imagen_2023-11-11_022818866.png" alt=""><figcaption></figcaption></figure>

</div>

Una vez seleccionado nos aparece una última confirmación, aceptamos y la máquina comienza su proceso.

<figure><img src="../.gitbook/assets/WhatsApp Image 2023-10-27 at 16.47.42 (1).jpeg" alt=""><figcaption><p>Proceso del BatCaliCat-man.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/WhatsApp Image 2023-10-29 at 12.00.24.jpeg" alt=""><figcaption><p>BatCaliCat-man terminado.</p></figcaption></figure>

Una vez terminado podemos extraer el objeto, limpiar los excesos de filamento incrustados en la plataforma y analizar el resultado.

<figure><img src="../.gitbook/assets/WhatsApp Image 2023-10-29 at 12.00.16.jpeg" alt="" width="188"><figcaption><p>Limpieza del exceso de filamento con ayuda de la herramienta.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/WhatsApp Image 2023-10-29 at 12.26.52.jpeg" alt="" width="188"><figcaption><p>Podemos abrir la rejilla para acceder a la plataforma con facilidad.</p></figcaption></figure>

**Resultado Final**

<figure><img src="../.gitbook/assets/WhatsApp Image 2023-10-30 at 13.18.56 (1).jpeg" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/WhatsApp Image 2023-10-30 at 13.18.56.jpeg" alt=""><figcaption><p>Desperfectos en el lateral.</p></figcaption></figure>

A pesar de utilizar los parámetros de temperatura especificados en la etiqueta del producto, no salió como se esperaba.

Se debe realizar nuevas pruebas con otros parámetros de temperatura.

| Nuevos Intentos |   |
| --------------- | - |
|                 |   |
|                 |   |
|                 |   |



¡Gracias por seguir este tutorial!

¡Espero que este tutorial te haya sido de utilidad! Si tienes alguna pregunta o necesitas más ayuda, no dudes en contactarnos. ¡Gracias por leer y buena suerte en tus proyectos futuros!
