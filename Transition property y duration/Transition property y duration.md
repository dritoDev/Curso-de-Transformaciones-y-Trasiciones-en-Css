Recapitulando, las transformaciones ocurren instantáneamente, sin embargo, estos cambios son no permiten crear una animación. La propiedad transition de CSS sirve para agregar un intervalo de tiempo a un elemento HTML para visualizar los cambios de una transformación.

transition: [property] [duration] [timing-function] [delay];
transition-property (obligatoria)
transition-duration (obligatoria)
transition-timing-function (opcional)
transition-delay (opcional)
Propiedades obligatorias para una transición
transition-property: esta propiedad sirve para especificar el elemento HTML de la transición. Si la transición es para todos los elementos, su valor es all.
transition-duration: esta propiedad sirve para agregar un intervalo de tiempo en segundos o milisegundos (1s = 1000ms).

selector {
    transition: transform 100ms;
    transition: all 2s;
}

Ejemplo sin transiciones.
Archivos de la clase
transition-property-duration.html
transiciones.pdf
Lecturas recomendadas

HTML Color Codes

http://htmlcolorcodes.com/


transition - CSS: Cascading Style Sheets | MDN

https://developer.mozilla.org/en-US/docs/Web/CSS/transition