# CORNER (“L”) JOINTS

<figure><img src="../../../.gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure>

Esta disposición de lengüetas y ranuras entrelazadas en un ángulo de noventa grados es, por supuesto, antigua y rudimentaria. La mayoría de las personas la llaman "unión de caja". También puede ser mejorada al romper la simetría.

<figure><img src="../../../.gitbook/assets/image (1) (2).png" alt=""><figcaption><p>Es adaptable a la disposición de tuerca empotrada atornillada.</p></figcaption></figure>

El material a utilizar es el MDF

<details>

<summary><mark style="color:purple;">Qué es el MDF</mark></summary>

El fibropanel de densidad media o MDF (por sus siglas en inglés medium density fibreboard o también llamado DM, Trupán​ o Fibrofácil) es un producto de madera reconstituida que se obtiene descomponiendo residuos de madera dura o blanda en fibras de madera, a menudo en un desfibrador, combinándolo con cera y un aglutinante de resina, y formando paneles mediante la aplicación de alta temperatura y presión. El MDF es por lo general más denso que el contrachapado. El MDF es más fuerte y denso que el aglomerado.

</details>

L a dimensión del grosor del MDF es de 12 mm, para nuestro corte en MDF debemos crear un archivo 2D y enviarlo al programa como .dxf

Utilizaremos un material de dimensiones de 300x300x120 mm

## <mark style="color:purple;">Diseñar el encastre</mark>

{% file src="../../../.gitbook/assets/encastres.3dm" %}
Archivo de Rhino descargable.
{% endfile %}

{% file src="../../../.gitbook/assets/Prueba encastre Erika.dxf" %}
Archivo de Rhino descargable.
{% endfile %}

<figure><img src="../../../.gitbook/assets/image (176).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_112008552.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_112054837.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (177).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_112214651.png" alt=""><figcaption></figcaption></figure>

## <mark style="color:purple;">Preparar el material</mark>

#### Cortar el material a utilizar

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_013659881 (1).png" alt="" width="188"><figcaption></figcaption></figure>

## <mark style="color:purple;">Prender la máquina</mark>

Para comenzar debemos girar la llave del compresor de aire y subimos el interruptor. Luego debemos dirigirnos al lateral izquierdo de la máquina para girar la perilla y la llave.

<div>

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_014819171.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_014913189.png" alt=""><figcaption></figcaption></figure>

</div>

Una vez funcionando el sistema de aire comprimido podemos retirar la pila de madera ya que la máquina ya puede estabilizarse sola, con la máquina apagada la fresa se terminaría rompiendo porque todo el conjunto del cabezal se caería con su propio peso.

<div>

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_015539007.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_015713917.png" alt=""><figcaption></figcaption></figure>

</div>

#### Medir las dimensiones

Debemos dimensionar los ejes en la CNC debemos considerar el larga de la mesa como X y el ancho como Y.

<div>

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_012158645.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_012458221.png" alt="" width="375"><figcaption><p>Dimensionar los ejes desde esta vista, en este caso el eje sería el X.</p></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_012431922.png" alt="" width="328"><figcaption><p>Pensar esta dirección como el eje Y.</p></figcaption></figure>

</div>

Para medir el material utilizaremos el calibre y la cinta métrica.

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_015003341.png" alt=""><figcaption><p>Utilizaremos el calibre y una cinta métrica.</p></figcaption></figure>

Dimensiones en el eje X&#x20;

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_012039117.png" alt=""><figcaption></figcaption></figure>

Dimensiones del eje Y

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_012017847.png" alt=""><figcaption></figcaption></figure>

Dimension en el eje Z

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_011945582.png" alt=""><figcaption></figcaption></figure>

#### Fijar el material a la mesa con un taladro y tornillos

<div>

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_004739436.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_004723650.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_014029112.png" alt=""><figcaption></figcaption></figure>

</div>

Podemos cambiar las brocas del taladro de acuerdo a las necesidades

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_014231542.png" alt=""><figcaption></figcaption></figure>

Debemos tener en cuenta que la distancia que utilizaremos se enuentra dentro del espacio que delimitan los tornillos que fijamos, debemos tener en cuenta la distancia de este margen.

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_014329472.png" alt=""><figcaption></figcaption></figure>

## <mark style="color:purple;">Establecer los ejes X, Y, Z</mark>&#x20;

#### Eje X e Y

Para acercar a los ejes X e Y se utiliza Software de **SnapBot** en la PC para guiar a la máquina CNC.

<div>

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_015344338.png" alt=""><figcaption><p>Al abrir debemos seleccionar la figura de aparente botonera amarilla que se encuentra en la ventana roja.</p></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_015400468.png" alt=""><figcaption><p>Utilizamos esta botonera para ubicarnos sobre el tornillo inferior derecho de nuestra pieza.</p></figcaption></figure>

</div>

El primer paso sería pinzar la fresa y colocar la pieza de metal debajo.

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_011733118.png" alt=""><figcaption><p>Intersección de X e Y sobre el tornillo. Desde esta perspectiva se ve un poco desviado.</p></figcaption></figure>

Hasta acá hemos establecido el eje X e Y, ahora podemos actualizar el eje 0 en el SnapBot. Debemos seleccionar el botón de **Zero Axes.**

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_115115938 (1).png" alt=""><figcaption></figcaption></figure>

<div>

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_114613671.png" alt=""><figcaption><p>Vista del la ventana de SnapBot cuando la máquina se encuentra en movimiento.</p></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_114806406.png" alt=""><figcaption></figcaption></figure>

</div>

**Eje Z**

En el caso del eje Z debemos acercar con Snapbot a un lugar específico entre la intersección de X e Y sobre el tornillo del margen inferior derecho, también debemos dejar poca distancia sobre el tornillo para que la operación tarde mucho menos. Y luego extraer las pinza y la pieza de metal para establecer con la ayuda del software SnapBot el eje Z.

<div>

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_011825774.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_015639535.png" alt=""><figcaption><p>Ubicación de guardado de las piezas.</p></figcaption></figure>

</div>

Una vez ubicado los ejes debemos actualizar el eje en el software. Debemos seleccionar el botón del Z que se encuentra a lado del ícono de la botonera amarilla. El proceso de ubicación sobre el eje Z el Bot realiza dos pasadas, durante esta operación debemos sostener la pieza de metal.

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_114806406.png" alt=""><figcaption></figcaption></figure>

## <mark style="color:purple;">**VCarve**</mark>

Para cargar nuestro archivo realizado en Rhino a la CNC debemos utilizar el software VCarve Pro, aquí determinaremos la ubicación sobre el material, el tipo de operación, la profundidad de fresar, ubicar Taps para evitar que vuele el material, etc.

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_115740603.png" alt=""><figcaption><p>Seleccionar la VCarve Pro en el inicio.</p></figcaption></figure>

Seleccionamos New File para crear una nueva mesa de trabajo.

<div>

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_115641483.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_123654308.png" alt=""><figcaption></figcaption></figure>

</div>

Debemos Importar los vectores de la carpeta que previamente se ha copiado en el equipo.

{% hint style="info" %}
&#x20;El archivo diseñado en Rhino lo había guardado en  un pendrive y luego exportado a la PC.
{% endhint %}

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_125031265.png" alt=""><figcaption><p>Debemos seleccionar Import Vectors.</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_125031265.png" alt=""><figcaption></figcaption></figure>



## <mark style="color:purple;">Toolpath</mark>

<div>

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_134706692.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_134946454.png" alt=""><figcaption></figcaption></figure>

</div>



<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_135134802 (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_134452169.png" alt=""><figcaption></figcaption></figure>

{% embed url="https://photos.app.goo.gl/o1vpbTwN4xKBqf218" %}

## <mark style="color:purple;">Resultado</mark>

Al finalizar el corte destornillamos el pedazo de MDF, empujamos las piezas resultantes.

Luego tenemos que lijar

<div>

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_004539546.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_004550464.png" alt=""><figcaption></figcaption></figure>

</div>

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_004604697.png" alt=""><figcaption></figcaption></figure>

<div>

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_004649447.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../../../.gitbook/assets/imagen_2023-11-13_004623758.png" alt=""><figcaption></figcaption></figure>

</div>

