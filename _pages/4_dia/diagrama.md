---
title: Diagrama de flujo
author: Billy Y. Fernández
date: 2022-03-23
category: Jekyll
layout: post
---

Cuando se abre el editor, encontraremos una pantalla divida en dos partes. A la izquierda el editor de texto, y a la derecha el diagrama de flujo. Solo aparecerán en el diagrama las secciones fijas y las que van a ser numeradas posteriormente en la salida. 

El diagrama cuenta con botones en la barra de herramientas para hacer zoom, alejarse y realizar una captura de los nodos visibles en formato SVG.

Podemos agrupar nodos en clústers, encerrando en el editor de texto las secciones que queremos juntar entre tres dos puntos o más (:::). Así:

```
::::::::::::: titulo_del_cluster :::::::::::
# sec1
ve a la [sec2]

# sec2
ve a la [sec1]
::::::::::::::::::::::::::::::::::::::::::::
```