---
description: >-
  En la siguiente documentación se realiza un diseño paramétrico en base a una
  imagen en Grasshopper.
cover: ../.gitbook/assets/imagen_2023-11-04_201920028.png
coverY: 76.8508682328907
layout:
  cover:
    visible: true
    size: full
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

# Crear un diseño con Grasshopper

Grasshopper es un plugin de Rhino, como descargamos la versión completa no será necesario descargar el plugin aparte, en caso de serlo se debe dirigir al siguiente enlace:

{% embed url="https://www.food4rhino.com/en" %}
Enlace a Food4Rhino.
{% endembed %}

{% hint style="info" %}
En Food4Rhino puede encontrar plugins y materiales para Rhino.
{% endhint %}

Una vez descargado de ser necesario podemos comenzar con el tema que nos compete, primero abrimos el programa Rhino 7, y seleccionamos ¨Tools¨ en el cual encontraremos en las opciones ¨Grasshopper¨.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_191459406.png" alt=""><figcaption><p>Inicio de la interfaz de Rhino 7.</p></figcaption></figure>

En el menú seleccionamos Grasshopper, a continuación se ejecutará el plugin en otra pestaña a la par de la interfaz de Rhino.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_191536479.png" alt=""><figcaption><p>Pestaña de Tools</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_191551648.png" alt=""><figcaption><p>Inicio de Grasshopper.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_191607588.png" alt=""><figcaption><p>La primera vez que se inicie Grasshopper se nos proporcionará indicaciones iniciales y tutoriales.</p></figcaption></figure>

Crear un nuevo documento en Grasshopper para iniciar.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_191622454.png" alt=""><figcaption><p>Interfaz inicial de Grasshopper.</p></figcaption></figure>

Para crear nuestra imagen paramétrica nuestro nodo clave será el **Image Sampler**.

Podemos encontrarlo en el menú de **Paramans** y luego en **Util**.

<details>

<summary>Cómo ingresar un nodo en la mesa de trabajo en Grasshopper.</summary>

Contamos con dos opciones, la primera es seleccionar desde el menú.&#x20;

<img src="broken-reference" alt="" data-size="original">

Y la segunda es hacer doble click izquierdo para abrir un buscador directamente.

<img src="broken-reference" alt="" data-size="original">

</details>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_191718634.png" alt=""><figcaption><p>Ubicación de Image Sampler en el menú.</p></figcaption></figure>

Necesitaremos cargar una imagen al nodo.

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption><p>Nodo sin archivo de Imagen.</p></figcaption></figure>

Al hacer doble click en Image Sampler se observa esta pestaña emergente.

En los parametrosde X e Y domain ingresamos las dimensiones de nuestra imagen, de 0 a 230px por ejemplo.

En channel podemos seleccionar de que información extraeremos de la imagen para utilizar, con solo el rojo, verde, azul, alpha, hue, blanco y negro.Para seleccionar una imagen debemos abrir File path y así seleccionamos desde nuestra galería. Podemos tachar Auto Update y Save in file.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_192135520.png" alt=""><figcaption><p>Pantalla emergente.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_192144770.png" alt=""><figcaption><p>Seleccionar imagen a utilizar en File path.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_192157080.png" alt=""><figcaption><p>Seleccionar una imagen desde la galería y abrir.</p></figcaption></figure>

Supongo que no es la imagen ideal pero vamos a probar mientras tanto con la siguiente imagen .JPG.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_192247577.png" alt=""><figcaption><p>Image Sampler con la imagen ya seleccionada.</p></figcaption></figure>

La configuración a utilizar serán las siguientes.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_192304390.png" alt=""><figcaption><p>Menú de completo Image Sampler.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_192320042.png" alt=""><figcaption><p>Channel de RBGA Colours.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_192351722.png" alt=""><figcaption><p>Dimensiones de X e Y Domain.</p></figcaption></figure>

Ingresaremos un nodo de Square, se trata de ingresar un cuadro 2D con celdas.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_192407252.png" alt=""><figcaption></figcaption></figure>

También un Number Slider para ingresar un valor numérico conectándolo a otro nodo.

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption><p>Vista de un Number Slider con un valor 0.250, el cual es el valor por default.</p></figcaption></figure>

{% hint style="info" %}
Podemos hacer doble click para abrir el buscador y simplemente escribir el valor numérico a utilizar para crear un Number Slider con el valor que queremos más rápido.

<img src="../.gitbook/assets/imagen_2023-11-04_192551474.png" alt="" data-size="original"><img src="../.gitbook/assets/imagen_2023-11-04_192603588.png" alt="" data-size="original">
{% endhint %}

Conectaremos los valores numéricos de los Number Slider a Ex (extender en el eje x) y a Ey (extender en el eje y).

Conectamos estos valores numéricos al Cuadro 2D para determinar las dimensiones de la grilla 2D.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_192634951.png" alt=""><figcaption><p>Nodos de valores numéricos conectados al nodo de la grilla 2D.</p></figcaption></figure>

{% hint style="info" %}
Si el nodo se ve en rojo y con una advertencia en la zona superior será necesario cambiar algún valor que sea incompatible para poder procesar nuestro trabajo luego.
{% endhint %}

<figure><img src="../.gitbook/assets/imagen_2023-11-04_192739408.png" alt=""><figcaption><p>Nuevos valores en cada Number Slider.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_192752177.png" alt=""><figcaption><p>Relación de los números en Image Sampler con los nuevos Number Slider.</p></figcaption></figure>

Nos dirigimos al nodo de la grilla 2D y en la salida ¨P¨ de points, hacemos click derecho y seleccionamos Flatten.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_192808939.png" alt=""><figcaption><p>Ícono de Flatten en el menú.</p></figcaption></figure>

Nuestra Grilla 2D se ve de la siguiente manera mientras tanto.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_192829817.png" alt=""><figcaption><p>Grilla 2D en el viewport de Rhino.</p></figcaption></figure>

Teniendo en cuenta que el resultado saldrá mejor si la imagen es blanco y negro, decidí editar la imagen en Photoshop.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_192921748.png" alt=""><figcaption><p>Edición en Photoshop.</p></figcaption></figure>

También decidí desenfocar levemente la imagen. Seleccioné Desenfoque Gaussiano.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_192937817.png" alt=""><figcaption><p>Filtros de desenfoque en Photoshop.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_192950672.png" alt=""><figcaption><p>Desenfoque Gaussiano de 1.0 píxeles.</p></figcaption></figure>

Al momento de exportar la imagen para guardarlo, cambié las dimensiones em X e Y, y lo guardé como .png

<figure><img src="../.gitbook/assets/imagen_2023-11-04_193131649.png" alt=""><figcaption><p>Vista de <strong>Exportar como.</strong></p></figcaption></figure>

La imagen final a utilizar será la siguiente.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_193152204.png" alt=""><figcaption><p>Imagen editada.</p></figcaption></figure>

Reemplacé la imagen y los valores en X e Y.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_193203247.png" alt=""><figcaption><p>Imagen reemplazada en Image Sampler.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_193219301.png" alt=""><figcaption><p>Nuevos valores para extender en X e Y en la grilla cuadrada 2D.</p></figcaption></figure>

Los puntos de la grilla 2D a un nodo de círculo y a nodo de Image Sampler.

<figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption><p>Nodos de círculo y la Image Sampler.</p></figcaption></figure>

Al conectar los puntos de la grilla al nodo de círculo y el Image Sampler se ve de la siguiente manera en el viewport.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_193350840.png" alt=""><figcaption><p>Vista en el viewport.</p></figcaption></figure>

Conectamos un panel al image sampler y se nos presentaran los puntos y sus coordenadas.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_193404604.png" alt=""><figcaption><p>Nodo de panel.</p></figcaption></figure>

Insertamos un nodo de ReMap Numbers al grupo para cambiar los valores de los dominios de la dimensión.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_193418573.png" alt=""><figcaption><p>Descripción de ReMap Numbers.</p></figcaption></figure>

También un no matemático "Round" para redondear el valor.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_193554870.png" alt=""><figcaption><p>Nodo matemático para redondear.</p></figcaption></figure>

Conectamos los nodos de Round y ReMap al panel, que a su vez el panel al Image Sampler.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_193606622.png" alt=""><figcaption><p>Conectar los nodos de Round y ReMap. </p></figcaption></figure>

Los nodos de entrada y salida son los siguientes:

La salida F de Floor en el Round es conectado al Source de ReMap.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_193650302.png" alt=""><figcaption><p>Salida de Floor en Round.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_193702633.png" alt=""><figcaption><p>Entrada Source en ReMap.</p></figcaption></figure>

Value en ReMap se conecta al panel.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_193832246.png" alt=""><figcaption><p>Salida de value conectado en el panel.</p></figcaption></figure>

Añadimos un nodo de Construct Mesh para crear malla de superficie a partir de vértices.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_193844973.png" alt=""><figcaption><p>Nodo de Construct Mesh.</p></figcaption></figure>

Debemos añadir un nodo Domain/Dominio y dos slider number\`s.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_193859475.png" alt=""><figcaption><p>Nodo Domain.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_193910611.png" alt=""><figcaption><p>Number sliders para A y B en el nodo de dominio.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_193922019.png" alt=""><figcaption><p>Number sliders.</p></figcaption></figure>

Conectamos el nodo de Dominio entre los valores A y B al nodo ReMap en la entrada de Target.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_194000761.png" alt=""><figcaption><p>Target Domain de 1 valor heredado entre de los valores de 0.2 y 0.5.</p></figcaption></figure>

Ahora volvemos a utilizar el nodo de círculo a ReMap, debemos conectar la salida de Remapped number de ReMap a la entrada de Radio al nodo de círculo.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_194015342.png" alt=""><figcaption><p>Vista general de nuestros nodos hasta este paso, acercamos el nodo de círculo a nuestro nodo de ReMap.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_194025693.png" alt=""><figcaption><p>Salida ¨R¨ Remapped number.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption><p>Salida ¨R¨ de radius (radio) del nodo círculo.</p></figcaption></figure>

Vista en el viewport de los círculos en la grilla después del ReMap.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_194146369.png" alt=""><figcaption><p>Vista de los círculos de forma que los bordes coincidan controlando los valores A y B en el Number Slider.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_194157349.png" alt=""><figcaption><p>Al sustituir los valores A y B, se modifica el tamaño de los círculos en la grilla.  </p></figcaption></figure>

{% hint style="info" %}
Me di cuenta de un error en el uso de los nodos más tarde, por lo que tuve que cambiar el nodo 'round' por el nodo 'bound'.
{% endhint %}

<figure><img src="../.gitbook/assets/image (8).png" alt=""><figcaption><p>Reemplazar Round por Bound.</p></figcaption></figure>

El nodo Bound crea un dominio numérico que abarque una lista de números.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_194304618.png" alt=""><figcaption><p>Vista de la descripción del nodo Bound.</p></figcaption></figure>

La salida I del nodo bounds se conectará a la entrada source de ReMap. La salida **I** indica un dominio numérico entre el número más bajo y el número más alto en **N.**

<figure><img src="../.gitbook/assets/imagen_2023-11-04_194315236.png" alt=""><figcaption><p>Vista de la descripción de la salida I del nodo Bound.</p></figcaption></figure>

Añadimos un nodo de panel. Debido a este nodo se evidencia el error del nodo Round y Bound.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_194349484.png" alt=""><figcaption><p>Nodo de panel.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_194359957.png" alt=""><figcaption><p>ReMap con error.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_194410077.png" alt=""><figcaption><p>El error se ve en el panel con el valor nulo.</p></figcaption></figure>

Una vez reemplazado el nodo Round por el de Bound el panel ya no presenta error.

Duplicaremos el grupo que se encuentra resaltado en verde.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_194504049.png" alt=""><figcaption><p>Grupo de nodos duplicados.</p></figcaption></figure>

Añadimos un nodo de división y un solo number slider.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_194515726.png" alt=""><figcaption><p>Nodo de división matemática con dos entradas A y B y una salida para el resultado.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_194527540.png" alt=""><figcaption><p>Number Slider con el valor de 1.</p></figcaption></figure>

El valor 1 se ingresará en la entrada de división A y la salida Remapped Number del nodo de ReMap se ingresará en la entrada B del nodo de división.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_194636046.png" alt=""><figcaption><p>División entre 1 y el Remapped Number.</p></figcaption></figure>

El Remapped number 1 será conectado igualmente en el nodo Bound del nuevo grupo que se había duplicado.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_194645955.png" alt=""><figcaption><p>Salida Remapped Number del nodo ReMap en la entrada de número más alto del nodo Bound.</p></figcaption></figure>

La División resultante se ingresará en la entrada Value en la entrada de ReMap del nuevo grupo duplicado.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_194656475.png" alt=""><figcaption><p>Nodos mencionados conectados al segundo ReMap.</p></figcaption></figure>

El número resultante de ReMap lo conectamos el radio del nodo de círculo duplicado y también conectamos un panel.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_194705422.png" alt=""><figcaption><p>El número resultante de ReMap lo conectamos el radio del nodo de círculo duplicado.</p></figcaption></figure>

La entrada de plane se conecta en la salida de point de la grilla 2D.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_200244530.png" alt=""><figcaption><p>La entrada plane de círculo se conecta a la salida point de la grilla 2D.</p></figcaption></figure>

Conectamos el panel entre la salida de Remapped Number y el Radio del círculo.&#x20;

<figure><img src="../.gitbook/assets/imagen_2023-11-04_200304589.png" alt=""><figcaption><p>Colocar el panel entre la conexión ya existente entre Remapped Number y Radio del Círculo.</p></figcaption></figure>

Vista de lo realizado hasta este nodo desde el viewport.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_200428739.png" alt=""><figcaption><p>Vista desde el viewport.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_200438933.png" alt=""><figcaption><p>Vista más cercana al rostro.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_200450189.png" alt=""><figcaption><p>Zoom a los círculos de la grilla.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_200508891.png" alt=""><figcaption><p>Segunda vista del zoom del viewport.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (9).png" alt=""><figcaption><p>Vista del zoom cercano y lejano.</p></figcaption></figure>

La función principal de este tutorial es generar una extrusión a partir de la imagen creada a partir de los círculos, para generar una imagen tridimensional.

Para generar la extrusión buscamos e insertamos el nodo de Extrude.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_200557759.png" alt=""><figcaption><p>Nodo de extrude.</p></figcaption></figure>

Para extruir en dirección vertical necesitamos indicar el eje Z, para ello buscamos el nodo Unit Z.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_200629268 (1).png" alt=""><figcaption><p>Vista del nodo Unit Z.</p></figcaption></figure>

Conectar de la siguiente manera.

El resultado de círculo se conecta con la entrada Base del nodo Extrude.

La salida Unit Vector de Unit Z se conecta a la entrada Direction del nodo Extrude.

<figure><img src="../.gitbook/assets/image (10).png" alt=""><figcaption><p>Conexiones de los nodos Unit Z y Circle al nodo Extrude.</p></figcaption></figure>

Resultado de la extrusión.

<figure><img src="../.gitbook/assets/image (11).png" alt=""><figcaption><p>Vista de cerca de la imagen con dimensiones en 3D del dibujo.</p></figcaption></figure>

Para aumentar el tamaño de los cilindros seguimos los siguientes pasos.

Agregar un nodo de multiplicación.&#x20;

<figure><img src="../.gitbook/assets/imagen_2023-11-04_200938940.png" alt=""><figcaption><p>Nodo matemático de multiplicación.</p></figcaption></figure>

Conectamos la salida del panel que contiene la información del nodo Remapped Number en A, y un Number Slider en B. A su vez el resultado de la multiplicación se conectará a la entrada de factor del nodo de Unit Z, y la salida de Unit Z a su vez a Dirección del nodo Extrude.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_201016690.png" alt=""><figcaption><p>Vista de los nodos descritos y el number slider con un valor que modifica la altura de los cilindros.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_201026689.png" alt=""><figcaption><p>Vista de la conexión del resultado de la multiplicación al eje Z y éste a la dirección a extruir.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_201039931.png" alt=""><figcaption><p>Vista lejana con las nuevas modificaciones.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_201116751 (2).png" alt=""><figcaption><p>Zoom a los cilindros extruidos.</p></figcaption></figure>

Para tapar los cilindros añadimos el nodo Cap.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_201151093.png" alt=""><figcaption><p>Nodo Cap Holes.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_201201998.png" alt=""><figcaption><p>Vista de los cilindros tapados.\</p></figcaption></figure>

Para finalizar el modelo y luego procesarlo debemos hacer click derecho y seleccionar Bake.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_201230868.png" alt=""><figcaption><p>Seleccionar Bake.</p></figcaption></figure>

Configurar el nombre, seleccionar para renderizar en un solo grupo.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_201430969.png" alt=""><figcaption><p>Configuraciones de Bake.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_201339406.png" alt=""><figcaption><p>Nombre Seleccionado.</p></figcaption></figure>

Ahora debemos esperar a que finalice el bake.

<figure><img src="../.gitbook/assets/imagen_2023-11-04_201517226.png" alt=""><figcaption><p>Vista de creación de mallas.</p></figcaption></figure>

Debido al error de cálculos en el nodo la creación de mallas no se pudo realizar.

{% hint style="info" %}
Posible solución convertir el Circle Curve a Polilíneas.
{% endhint %}

<figure><img src="../.gitbook/assets/image (12).png" alt=""><figcaption><p>Error de creación de malla.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_201618328.png" alt=""><figcaption><p>Vista del relieve.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_201920028.png" alt=""><figcaption><p>Vista del relieve.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/imagen_2023-11-04_201935530.png" alt=""><figcaption><p>Vista del relieve.</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (13).png" alt=""><figcaption><p>Vista dek Relieve.</p></figcaption></figure>
