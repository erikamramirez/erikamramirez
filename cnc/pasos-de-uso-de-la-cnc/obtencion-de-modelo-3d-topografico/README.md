---
description: >-
  Crearemos un modelo 3d y realizaremos el fresado en una máquina CNC de un
  terreno seleccionado de Google Maps.
---

# Obtención de modelo 3D topográfico

{% embed url="https://jthatch.com/Terrain2STL/" %}
Página para crear un archivo .stl de cualquier lugar del mapa de Google Maps.
{% endembed %}

{% embed url="https://www.youtube.com/watch?v=H9oFvuCNeIQ" %}
Tutorial de Terrain2STL.
{% endembed %}

Antes de empezar entenderemos los parámetros de la página.&#x20;

<figure><img src="../../../.gitbook/assets/image (14) (1) (1) (1).png" alt=""><figcaption><p>Vista de la página del enlace.</p></figcaption></figure>

En el menú lateral derecho podemos observar los siguientes parámetros.

## <mark style="color:purple;">**Ubicación**</mark>

Coordenadas de la esquina noroeste.

&#x20;Latitud y Longitud.

&#x20;Y en botón de centrar vista.

<figure><img src="../../../.gitbook/assets/image (15) (1) (1) (1).png" alt=""><figcaption><p>Vista del menú de ubicación.</p></figcaption></figure>

## <mark style="color:purple;">**Detalles del modelo**</mark>

* Ancho de la caja.
* Altura de la caja.
* Factor de escala de la caja.
* Rotación de la caja (grados).
* Escala vertical

<figure><img src="../../../.gitbook/assets/image (16) (1) (1) (1).png" alt=""><figcaption><p>Vista del menú de detalles del modelo.</p></figcaption></figure>

## <mark style="color:purple;">**Configuraciones de base y agua.**</mark>

* Gota de agua (mm).
* Altura de la base (mm).

<figure><img src="../../../.gitbook/assets/image (17) (1) (1) (1).png" alt=""><figcaption><p>Vista del menú de Configuraciones de Base y Agua.</p></figcaption></figure>

## <mark style="color:purple;">Instrucciones</mark>

<figure><img src="../../../.gitbook/assets/image (7) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

1. Selecciona el área de la que deseas obtener un archivo STL utilizando el recuadro rojo.
2. Centrar en vista' moverá el recuadro. También es arrastrable.
3. Gira y ajusta el tamaño del recuadro según sea necesario.
4. La escala Z exagera la escala vertical de los modelos.
5. La gota de agua disminuye la altura de los océanos para resaltar.
6. No te preocupes por que el recuadro se distorsione con las rotaciones; el modelo será preciso en relación al terreno real.

