---
title: Diagrama de flujo
author: Billy Y. Fernández
date: 2022-03-20
category: Jekyll
layout: post
---

Cuando se abre el editor, encontraremos una pantalla divida en dos partes. A la izquierda el editor de texto, y a la derecha el diagrama de flujo. Solo aparecerán en el diagrama las secciones fijas y las que van a ser numeradas posteriormente en la salida. 

El diagrama cuenta con botones en la barra de herramientas para hacer zoom, alejarse y realizar una captura de los nodos visibles en formato SVG.

## Clústers

Podemos agrupar nodos en clústers, encerrando en el editor de texto las secciones que queremos juntar entre tres dos puntos o más (:::). Así:

```
::::::::::::: titulo_del_cluster :::::::::::
# sec1
ve a la [sec2]

# sec2
ve a la [sec1]
::::::::::::::::::::::::::::::::::::::::::::
```

## Clases

Para usar una clase para un nodo, en el bloque de metadatos de la sección debe añadir class, seguido del nombre de la clase. Hay cuatro clases predefinidas: **deadly**, **treasure**, **final** y **fight**. Al usar una de estas cambiara el color del nodo, el borde, la forma y se le añadirá un ícono al lado del nombre.

Puede crear su propia clase usando un bloque de definición como el siguiente:

```
===== deadly =====
fill: yellow
stroke: white
stroke_width: 2px
icon: skull
shape: round
------------------
```

Un bloque de definición usa la misma estructura que un bloque de metadatos, solo que inicia con por lo menos tres `=`, en vez de `-`, y lleva acompañado un nombre, que sigue la mismas reglas que los nombres de la secciones.

- **fill:** Para especificar el color de relleno del nodo. El color puede ser dado en inglés o en código hexadecimal (en ese caso, debe envolver el código hexadecimal entre comillas)
- **stroke:** Para especificar el color del borde.
- **stroke_width:**  Para el grosor del borde.
- **icon:** Para especificar un ícono. Puede buscar el nombre del ícono que desea usar en [esta web](https://fontawesome.com/search?m=free&s=solid).
- **shape:** Especifica la forma del nodo. Puede ser **circle**, **round**, **diamond** y **hexagon**.

Puede usar los bloques de definición que desee, siempre y cuando estén ubicados entre el bloque de metadatos del principio y la primera sección, sea cual sea su tipo.

Puede también sobreescribir clases, por ejemplo algunas de las predeterminadas, con tan solo usar el mismo nombre en un bloque de definición.

