# Apuntes Curso Desarrollo Fullstack Javascript
---


## INDICE

0. [AYUDA](#ayuda-formato)
1. [Módulo 1](#modulo-1)
2. [Módulo 2](#modulo-2)
3. [Módulo 3](#modulo-3)
4. [Módulo 4](#modulo-4)
5. [Módulo 5](#modulo-5-bases-de-datos)
6. [Módulo 6](#modulo-6)
7. [Módulo 7](#modulo-7-acceso-a-base-de-datos-con-node)
8. [Módulo 8](#modulo-8)


---


## Modulo 1

Aquí debería ir algún apunte del módulo 1.
Procure seguir las ayudas para formatear el texto con títulos, subtítulos, enlaces, etc.

---


## Modulo 2

Aquí debería ir algún apunte del módulo 2.
Procure seguir las ayudas para formatear el texto con títulos, subtítulos, enlaces, etc.

---


## Modulo 3

Aquí debería ir algún apunte del módulo 3.
Procure seguir las ayudas para formatear el texto con títulos, subtítulos, enlaces, etc.

---


## Modulo 4

Aquí debería ir algún apunte del módulo 4.
Procure seguir las ayudas para formatear el texto con títulos, subtítulos, enlaces, etc.

---


## Modulo 5 Bases de Datos

Aquí debería ir algún apunte del módulo 5.
Procure seguir las ayudas para formatear el texto con títulos, subtítulos, enlaces, etc.

#### Cómo hacer una consulta anidada con dos join

A continuación se da un ejemplo para realizar una consulta a través de psql, donde se hace una primera consulta a través de un join de dos tablas. El resultado de esa consulta es una tabla que será usada para realizar un segundo join (o sea, es como una tabla "virtual").

```
select TABLA4.COLUMNA, TABLA4.COLUMNA2 from
(select TABLA1.COLUMNA, TABLA2.COLUMNA from prestamos
join TABLA2 on TABLA1.COL-JOIN = TABLA2.COL-JOIN) as TABLA3
join TABLA4 on TABLA4.COL-JOIN = TABLA3.COL-JOIN;
```

En el ejemplo anterior, lo que está entre paréntesis es la primera consulta, cuyo resultado se ha llamado con el apodo de TABLA3. Es decir es como decir "select columnaX... from TABLA3".

Lo que va antes y después de los paréntesis es la segunda consulta. En este caso las dos consultas utilizan un join, pero el join puede hacerse sólo en una o en ninguna.



---


## Modulo 6

Aquí debería ir algún apunte del módulo 6.
Procure seguir las ayudas para formatear el texto con títulos, subtítulos, enlaces, etc.

---


## Modulo 7 Acceso a Base de Datos con Node

Aquí debería ir algún apunte del módulo 7.
Procure seguir las ayudas para formatear el texto con títulos, subtítulos, enlaces, etc.

---


## Modulo 8

Aquí debería ir algún apunte del módulo 8.
Procure seguir las ayudas para formatear el texto con títulos, subtítulos, enlaces, etc.

---



## Ayuda Formato


Los títulos (como el de arriba que dice "Módulo 1") se escriben con "#" en el comienzo de la línea seguido de un espacio y el título. La cantidad de "#" definen el nivel del título, en este caso 1 "#" se usó para el título del documento y 2 "#"s para el título de cada módulo.
Así:

```
# Título mayor
## Título menor
## Subtítulo
etc...

Párrafo
```

Para hacer un enlace se debe escribir esto el texto a mostrar entre corchetes seguido de un espacio y el url del enlace entre paréntesis así:


`[Esto es texto] (este-es-un-enlace)`


Para referenciar un título dentro del mismo documento se hace así:


`[Texto] (#este-es-un-titulo-en-minusculas-y-con-guiones)`


Nótese que todo el enlace se escribe en minúsculas, y los espacios son guiones. Además, sólo se ocupa un solo "#", independiente de cuántos "#" tenga el título referenciado.


Para insertar código en una sola línea se debe incluir así:

\`código dentro de estos dos tildes hacia atrás\`


Para insertar código en varias líneas:

\`\`\`
Se debe insertar

dentro

de seis tildes hacia atrás.

Tres antes y tres después.
\`\`\`

[Más ayuda] (https://www.markdownguide.org/cheat-sheet)

[Volver al Índice](#indice)

---

