Recapitulando, una timing function es la representación de la progresión en función del tiempo de cada ciclo de una animación. Representa la aceleración del elemento desde un punto A hasta un punto B.

linear: El elemento se mueve a una aceleración constante.
ease: Es el valor predeterminado si no se especifica. El elemento acelera inicialmente, pero presenta mucha desaceleración.
ease-in: El elemento empieza lento pero termina rápido.
ease-out: El elemento empieza rápido pero termina lento.
ease-in-out: Es la combinación de ease-in y ease-out. El elemento empieza lento, a medida que avanza va acelerándose, pero termina lento.
cubic-bezier: Se necesitan cuatro números, que representan dos puntos de control para formar la curva de aceleración deseada.
Propiedades opcionales para una transición
transition-timing-function: propiedad que establece una timing function para especificar una forma de aceleración de la transición.

transition-delay: propiedad que establece un intervalo de tiempo desde la acción que desencadena la animación hasta su inicio.

Ejemplo usando transition-timing-fuction.

Ejemplo usando transition-delay.

Contribución creada por Andrés Guano.

Archivos de la clase
transition-timing-function-delay.html
Lecturas recomendadas

transition - CSS: Cascading Style Sheets | MDN

https://developer.mozilla.org/en-US/docs/Web/CSS/transition