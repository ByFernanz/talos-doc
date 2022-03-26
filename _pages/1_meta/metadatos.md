---
title: Metadatos
author: Billy Y. Fernández
date: 2022-03-23
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
titled_sections: false
hide_sections: false
tags: [terror, fantasia]
dia_scale: 8
dia_output: png
dia_book: true
---
~~~

Los metadatos que actualmente usa talos son: **title, author, lang, publisher, description, output, tags y turn_to**. Ninguno es obligatorio pero se recomienda por lo menos especificar el título, el autor y el formato de salida del documento.

- **output:** Los formatos de salida soportados por talos son: *html*, *epub*, *docx* y *pdf*.
- **turn_to:** Se usa para para especificar qué texto va a preceder a cada enlace, es decir el clásico "ve a la sección X".
- **lang:** Especifica la lengua que usará el documento, por ahora Talos solo soporta: español (**es**), inglés (**en**), hindi (**hi**) y vietnamita (**vi**) para todos los formatos de salida.
- **titled_sections:** Si se pone en **true** y se han definido títulos en las secciones, los enlaces y los números de las secciones serán sustuídos por estos nombres. En el caso del formato pdf o docx, se colocan ambos al mismo tiempo.
- **hide_sections:** Si está en **true**, oculta los títulos de las secciones o su número asignado. en el caso del formato pdf o docx, solo se oculta el título, pero se preservan los números.
- **dia_output:** Indica el formato de salida de la captura del diagrama de flujo. Puede estar en **svg** o **png**.
- **dia_scale:** Indica la escala de la captura del diagrama de flujo, si **dia_output** está en **png**.
- **dia_book:** Si está en *true*, junto al librojuego se generará una imagen del diagrama de flujo con todos los nodos numerados.