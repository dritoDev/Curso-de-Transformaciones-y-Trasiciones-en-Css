Un trigger es un accionador de animaciones, es decir, el evento inicial que desencadena una animación. Algunos ejemplos son:

Pasar el mouse sobre un elemento.
Dar clic a un elemento.
Al deslizar la pantalla.
Al recargar la página web.
Las pseudo-clases y pseudo-elementos ayudan a activar las animaciones.

Pseudo-clases
Una pseudo-clase define el estilo de un estado especial de un elemento.

Índice de pseudo-clases estándar{target="_blank"}.
Sintaxis
selector:pseudo-clase { propiedad: valor; }
:link
La pseudo-clase :link representa el estado de un elemento que no ha sido visitado.

Ejemplo usando :link{target="_blank"}
:visited
La pseudo-clase :visited representa el estado de un elemento que ya ha sido visitado.

Ejemplo usando :visited{target="_blank"}
:hover
La pseudo-clase :hover representa el estado en el cual el cursor está encima del elemento.

Ejemplo usando :hover{target="_blank"}
:not()
La pseudo-clase :not() representa el estado en el cual no coinciden los selectores que se indiquen.

Ejemplo usando :not(){target="_blank"}
:nth-child()
La pseudo-clase :nth-child() representa el estado en el cual coinciden los hijos del elemento según el valor indicado.

Valores de palabras clave:

odd: Los elementos hijos en posiciones impares.
even: Los elementos hijos en posiciones pares.
Fórmula matemática: An+B donde A y B son números enteros.

Ejemplo usando :nth-child(){target="_blank"}
Pseudos-elementos
Un pseudo-elemento define el estilo de una parte específica de un elemento.

Lista de pseudo-elementos{target="_blank"}.
Sintaxis
selector::pseudo-elemento { propiedad: valor; }
::before
La pseudo-elemento ::before sirve para agregar un contenido antes del elemento. El contenido es agregado mediante la propiedad CSS content.

Ejemplo usando ::before{target="_blank"}
::after
La pseudo-elemento ::after sirve para agregar un contenido después del elemento. El contenido es agregado mediante la propiedad CSS content.

Ejemplo usando ::after{target="_blank"}
Contribución creada por Andrés Guano.

Archivos de la clase
pseudo-classes.html
pseudo-elements.html
Lecturas recomendadas

HTML Color Codes

https://htmlcolorcodes.com/


:hover - CSS: Cascading Style Sheets | MDN

https://developer.mozilla.org/en-US/docs/Web/CSS/:hover


:focus - CSS: Cascading Style Sheets | MDN

https://developer.mozilla.org/en-US/docs/Web/CSS/:focus


:active - CSS: Cascading Style Sheets | MDN

https://developer.mozilla.org/en-US/docs/Web/CSS/:active


:disabled - CSS: Cascading Style Sheets | MDN

https://developer.mozilla.org/en-US/docs/Web/CSS/:disabled