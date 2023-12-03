# Black Frost y Jack Frost en FlashPrint

Para empezar debemos importar el modelo ya editado en Meshmixer abriendo en **Archivo**, luego **importar**, y seleccionar el modelo en nuestra galería.

Podemos proceder a añadir soportes dirigiéndonos al menú lateral derecho, seleccionar el ícono de soportes.

En las opciones de soporte seleccionaos el diámetro del soporte que creamos conveniente y luego **Autosoporte**. También podemos seleccionar manualmente

<figure><img src="../../.gitbook/assets/imagen_2023-11-13_051556403 (3).png" alt=""><figcaption></figcaption></figure>

Una vez obtenidos los soportes seleccionamos atrás y volvemos al menú inicial.&#x20;

&#x20;Nos dirigimos a calcular el corte con ahora los autosoportes incluidos

{% hint style="info" %}
Para el primer intento conservé los parámetros ya establecidos para las pruebas del Test de BatCaliCat-man.
{% endhint %}

Establecemos los parámetros de impresión de la temperatura de la extrusora derecha y la temperatura de la plataforma en el menú de **Impresora**.

<figure><img src="../../.gitbook/assets/image (172).png" alt=""><figcaption></figcaption></figure>

Una vez ejecutado Corte, podemos descargar nuestro archivo en formato .gx para luego procesarlo en la impresora 3D.

Los resultados en el primer intento no fueron satisfactorios.

***

## <mark style="color:purple;">Cambios</mark>

Observando los principales defectos del modelo original se realizaron cambios en los parámetros de Flashprint con la intensión de mejorar la impresión.

Este nuevo modelo tiene algunos fragmentos del **Black Frost** que no me pude deshacer en **Meshmixer**, para eliminarlo debemos empezar por seleccionar la herramienta de corte, seleccionar el formato vertical y ubicar el plano a la mitad de los fragmentos y la figura de Jack Frost y seleccionar **Iniciar Corte.**&#x20;

<div>

<figure><img src="../../.gitbook/assets/imagen_2023-11-13_051958696.png" alt=""><figcaption><p>Herramienta de Cortar.</p></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/imagen_2023-11-13_052009168.png" alt=""><figcaption><p>Plano de Corte entre las figuras a separar en objetos diferentes.</p></figcaption></figure>

</div>

Luego de seguir los pasos anteriores obtenemos dos objetos en la interface, lo cual podemos corroborar observando el menú, seleccionamos los fragmentos y lo eliminamos con el botón **Delete.**

<figure><img src="../../.gitbook/assets/imagen_2023-11-13_052031879.png" alt=""><figcaption><p>Se observa dos modelos en la lista del menú.</p></figcaption></figure>

Podemos centrar la pieza en la plataforma automáticamente seleccionando los botones **En plataforma** y **Centrar** que se encuentran en la ventana de Mover dentro del menú lateral derecho.

<figure><img src="../../.gitbook/assets/imagen_2023-11-13_052114347.png" alt=""><figcaption><p>Botones descritos ubicados en la ventana de Mover.</p></figcaption></figure>

Procedemos a escalar el objeto para no obtener un resultado tan pequeño como en el intento 1. Utilizamos la herramienta de Escalar ubicada en el menú lateral derecho.

<figure><img src="../../.gitbook/assets/imagen_2023-11-13_052101122.png" alt=""><figcaption><p>Escalado del modelo.</p></figcaption></figure>

Para establecer los parámetros para imprimir debemos seleccionar **Iniciar Corte**.

<figure><img src="../../.gitbook/assets/imagen_2023-11-13_052134294.png" alt=""><figcaption></figcaption></figure>

Una vez vista los problemas del intento 1 de Jack Frost en cuanto a la plataforma, se decidió aumentar la cantidad de capas de relleno.

Se realizó cambios en el alto de capa al parámetro de 0.10mm el cual consume más material pero nos ayudará para evitar que nuestra base no se vea quebradiza como en el primer intento.

<figure><img src="../../.gitbook/assets/imagen_2023-11-13_052220624.png" alt=""><figcaption></figcaption></figure>

Si bien el parámetro del primer intento ya es bajo de por sí (0.15mm) ahora será reemplazado por altura de capa 0.10mm.

<figure><img src="../../.gitbook/assets/imagen_2023-11-13_051922497.png" alt=""><figcaption><p>Alto de capa original</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (173).png" alt=""><figcaption><p>Nuevo parámetro.</p></figcaption></figure>

En el parámetro de Densidad de relleno será cambiado a 30% el cual es un relleno medio-bajo.

Para entender mejor sobre los parámetros de alto de capa, densidad de relleno y la influencia del tipo de relleno se puede visitar la siguiente página en esta documentación:&#x20;

{% content-ref url="../../test-de-impresiones/" %}
[test-de-impresiones](../../test-de-impresiones/)
{% endcontent-ref %}

<figure><img src="../../.gitbook/assets/imagen_2023-11-13_051803280.png" alt=""><figcaption><p>Nuevos parámetros establecidos.</p></figcaption></figure>

Los parámetros de temperatura de la extrusora derecha y la plataforma son las siguientes.

<figure><img src="../../.gitbook/assets/imagen_2023-11-13_052242798.png" alt=""><figcaption><p>Parámetros de temperatura de la extrusora derecha y plataforma.</p></figcaption></figure>

Seleccionamos el ícono para descargar el archivo compatible con la impresora en formato .gx y continuamos con el proceso habitual descrito en las siguiente documentaciones:

{% content-ref url="../diseno-3d-editando-con-meshmixer./diseno-3d-e-impresion-de-una-vasija..md" %}
[diseno-3d-e-impresion-de-una-vasija..md](../diseno-3d-editando-con-meshmixer./diseno-3d-e-impresion-de-una-vasija..md)
{% endcontent-ref %}

{% content-ref url="../descarga-e-impresion-de-un-test-de-impresion..md" %}
[descarga-e-impresion-de-un-test-de-impresion..md](../descarga-e-impresion-de-un-test-de-impresion..md)
{% endcontent-ref %}

<figure><img src="../../.gitbook/assets/imagen_2023-11-13_052329210.png" alt=""><figcaption></figcaption></figure>

