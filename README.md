# Apuntes Curso Desarrollo Fullstack Javascript
---


## INDICE

0. [AYUDA](#---)
1. [Módulo 1 - Fundamentos del Desarrollo de Páginas Web](#modulo-1)
2. [Módulo 2 - Programación básica en Javascript](#modulo-2)
- [Acceso al DOM](#acceso-al-dom)
3. [Módulo 3 - Programación avanzada en Javascript](#modulo-3)
4. [Módulo 4 - Desarrollo de Aplicaciones Web Frontend](#modulo-4)
5. [Módulo 5 - Lenguaje de Consultas a una Base de Datos Postgres](#modulo-5)
6. [Módulo 6 - Desarrollo de Backend en Node](#modulo-6)
7. [Módulo 7 - Acceso a base de datos con Node](#modulo-7)
8. [Módulo 8 - Framework Express](#modulo-8)


---


## Modulo 1
## Fundamentos del Desarrollo de Páginas Web

Aquí debería ir algún apunte del módulo 1.
Procure seguir las ayudas para formatear el texto con títulos, subtítulos, enlaces, etc.

---


## Modulo 2
## Programación básica en Javascript

### Acceso al DOM

En Javascript se puede acceder a elementos existentes en el documento HTML, almacenarlos en variables (const o let), obtener sus atributos y cambiarlos.

Esto se hace a través del DOM (Modelo del Objeto Documento), que es una interfaz definida para representar e interactuar con el documento HTML. Así, hay ciertas funciones o métodos definidos en Javascript que nos permiten hacer esto.

Uno de los objetos más importantes es el objeto documento, que representa al documento HTML completo. Con diversos métodos o funciones se pueden extraer porciones más acotadas y específicas a partir de document.

Ejemplos:


```

index.html --------------------------

...
<body>
    <div id="formulario">
        <div class="name"></div>
        <div class="email"></div>
        <div class="password"></div>
        <div class="resultado"></div>
    </div>
</body>
...

script.js ---------------------------

let formu = document.querySelector('#formulario');
let nam = document.querySelector('.name');
let email = document.querySelector('.email');
let pwd = document.querySelector('.password');
let resul = document.querySelector('.resultado');


```

En el ejemplo anterior se aprecia el uso del método querySelector, perteneciente al objeto document. Este método recibe como parámetro un string conteniendo un identificador en la misma notación que CSS, un # para referirse a un id y un . para referirse a una clase. Para seleccionar un tag (como div, body ...) no se debe anteceder nada ('div', 'img', 'p').

Al consultar en la consola del navegador por el valor de las variables almacenadas, nos devolverá la estructura html que le corresponde, o sea, el nivel que se seleccionó y sus hijas.

---


## Modulo 3
## Programación avanzada en Javascript

Aquí debería ir algún apunte del módulo 3.
Procure seguir las ayudas para formatear el texto con títulos, subtítulos, enlaces, etc.

---


## Modulo 4
## Desarrollo de Aplicaciones Web Frontend

Aquí debería ir algún apunte del módulo 4.
Procure seguir las ayudas para formatear el texto con títulos, subtítulos, enlaces, etc.

---


## Modulo 5
## Lenguaje de Consultas a una Base de Datos Postgres

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
## Desarrollo de Backend en Node

Aquí debería ir algún apunte del módulo 6.
Procure seguir las ayudas para formatear el texto con títulos, subtítulos, enlaces, etc.

---


## Modulo 7
## Acceso a Base de Datos con Node

Aquí debería ir algún apunte del módulo 7.
Procure seguir las ayudas para formatear el texto con títulos, subtítulos, enlaces, etc.

---


## Modulo 8
## Framework Express

Aquí debería ir algún apunte del módulo 8.
Procure seguir las ayudas para formatear el texto con títulos, subtítulos, enlaces, etc.

---


## - -
## Ayuda: Cómo escribo en este documento de tipo Markdown?


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

