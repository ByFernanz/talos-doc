---
title: Metadatos
author: Billy Y. Fernández
date: 2022-03-18
category: Jekyll
layout: post
---

Aunque no es estricamente necesario, el documento debe aperturar con un bloque de metadatos, delimitado por lineas de tres guiones y cada clave separada de su valor por dos puntos y espacio.

~~~yaml
---
title: El nombre del librojuego
author: Billy Y. Fernández
description: Un dragón ataca una aldea, debes salvarla.
lang: es
publisher: Textagames
output: docx
turn_to: ve a la sección
tags: [terror, fantasia]
---
~~~

Los metadatos que actualmente usa talos son: **title, author, lang, publisher, description, output, tags y turn_to**. Ninguno es obligatorio pero se recomienda por lo menos especificar el título, el autor y el formato de salida del documento.

- **output:** Los formatos de salida soportados por talos son: *html*, *epub*, *docx* y *pdf*.
- **turn_to:** Para especificar qué texto va a preceder a cada enlace, es decir el clásico "ve a la sección X".
- **lang:** Especifica la lengua que usará el documento, por ahora Talos solo soporta: español (**es**), inglés (**en**), hindi (**hi**) y vietnamita (**vi**) para todos los formatos de salida.