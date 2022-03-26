---
title: Secciones
author: Billy Y. Fernández
date: 2022-03-22
category: Jekyll
layout: post
---

Las secciones son las partes en las que se divide un librojuego. Una sección inicia con *#*, seguido de un espacio y luego el nombre de la sección.

~~~markdown
# esto_es_una_seccion "Este es el título de la sección"
Y esto es el contenido de la seccion.

Una linea en blanco indica la separacion entre párrafos.
~~~

- Si el nombre de la sección inicia con mayúscula, la sección aparecera tal cual fue redactada y se quedará en su sitio.
- Si el nombre está todo en minúscula separado por guiones bajos, esto quiere decir que a esta sección se le asignará un número aleatorio al producir el librojuego.
- Si el nombre es un número, se mantendrá tal cual en la salida y se pondrá en el lugar que le corresponde al ordenar las secciones de forma secuencial.
- El título de la sección solo será visible si en la cabecera del documento si está definido **titled_sections** en true. *Esta opción no es compatible con Pangamebook/Pandoc*.

## Metadatos locales

Las secciones también pueden tener un bloque de parámetros. Ejemplo:

~~~markdown
# otra_seccion
---
title: Una sección
description: Un nodo más
---
Y esto es el contenido de la seccion.
~~~

- **title:** Sirve para asignarle un nombre de la sección, hace lo mismo que los títulos en línea descritos anteriormente. Si ambos títulos están definidos, el que acompaña al nombre de la sección tendrá mayor prioridad.
- **description:** Puede usarse para hacer una pequeña descripción de lo que ocurre en la sección. Esta información será visible en el diagrama de flujo cuando el mouse repose sobre un nodo, en forma de tooltip.

