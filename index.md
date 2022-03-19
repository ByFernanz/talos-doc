---
layout: home
---

## ¿Qué es Talos Editor?

​Talos Editor es un entorno de desarrollo de librojuegos construido con tecnologías web, enfocado en la simplicidad y en reducir las frustraciones durante el proceso creativo.

La herramienta toma prestadas  las mecánicas de diseño de Pangamebook​ (un filtro de Pandoc para generar también librojuegos), expande sus características y las envuelve en un entorno moderno, productivo y amigable, sin dependencias externas, todo desde el navegador.

## ¿Qué hace exactamente Talos?

Talos busca todos los encabezados de nivel superior (**#**) que contienen solo letras minúsculas, dígitos y guiones bajos. Los encabezados como *inicio* , *primera_sala* o *encontrando_un_botín_23* se verán afectados, pero los encabezados como *Introducción* , *Cómo jugar* , F*icha de personaje* o *Epílogo* se ignorarán.

Un encabezado de nivel superior que sea un número también se ignorará, ya que ese número se usará tal cual.

Talos mezcla todos los encabezados afectados junto con todo lo que sigue hasta el siguiente encabezado de nivel superior, incluidos los encabezados de nivel inferior y todo el texto, las imágenes y las tablas, etc. Esa colección de cosas que se mueve junto con el encabezado se considera una sección .

Las secciones nunca se moverán de antes de un encabezado de nivel superior *ignorado* a después de ese encabezado, o viceversa. Un efecto importante de esto es que los encabezados que son números, como el 1 , permanecerán donde están , y también dividirán naturalmente el librojuego en partes que evitan que la historia salte demasiado. La mayoría de los libros probablemente tendrán un encabezado 1 para marcar el comienzo de la historia, asi se garantiza que seguirá siendo el primero en la salida también. Si el último encabezado tiene un número suficientemente alto (por ejemplo, 400 ), seguirá siendo el último. Cualquier otro encabezado también puede tener un número para corregirlo en la historia, pero si hay demasiadas secciones para barajar entre encabezados fijos, Talos no estará contento (por ejemplo, si baraja entre 1 y 400 , pero en realidad hay 410 secciones en el libro).

Después de barajar todas las secciones, todos sus encabezados se numeran en secuencia. Es posible que se creen espacios donde hay encabezados a los que se les dio un número fijo. Los encabezados que ya eran números, como se mencionó anteriormente, no se verán afectados.

Todos los enlaces en el documento se actualizarán finalmente para mostrar el número al que se refieren. Si por ejemplo en el documento documento original ponía "ver primera_sala" (donde primera_sala es un enlace válido, no solo texto) se convertirá en algo como "ver 12".

La mejor manera de aprender es probablemente experimentar con los botones y jugar  con el entorno.
