Ya revisaste las propiedades para realizar transformaciones en 2D, si te fijaste bien, habrás notado que cuando se realiza una transformación en un solo eje (por ejemplo rotateX) el elemento permanece en un solo plano.

Con las transformaciones 3D observaremos el elemento transformarse en diferentes planos.

Por lo tanto, es momento para aplicar transformaciones en 3D. Las propiedades CSS para esto serán: transform-style y perspective.

Transform style para transformaciones en 3D
La propiedad transform-style de CSS establece si un elemento hijo está en el plano 2D (flat) o 3D (preserve-3d). Por defecto, el elemento está con valor flat.

selector {
    transform-style: preserve-3d;
}
Perspective para transformaciones en 3D
La propiedad perspective se utiliza para proveer de profundidad a un elemento con respecto al usuario y dar la sensación de 3D.

El valor que recibe la propiedad es una longitud (px, rem, etc.) que representa la profundidad del plano para construir la perspectiva.

Animación de la propiedad perspective
Por defecto, el origen para las transformaciones 3D está en el centro, pero se puede modificar con la propiedad perpective-origin.

Ejemplo empleando transformaciones 3D.
Cambiar el origen de la perspectiva.
La propiedad perspective-origin es la encargada de cambiar el origen de la perspectiva, por lo que el usuario percibirá de diferente forma el elemento.

animationland09.PNG
Ejemplo cambiando la perspectiva.
Contribución creada por Andrés Guano.

Archivos de la clase
transform-style.html
Lecturas recomendadas

transform - CSS: Cascading Style Sheets | MDN

https://developer.mozilla.org/en-US/docs/Web/CSS/transform