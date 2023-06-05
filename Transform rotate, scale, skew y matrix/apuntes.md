Además de translate, existen otras funciones que permiten transformar el elemento HTML para iniciar una animaci

Rotate para transformaciones
Rotate es una función de la propiedad transform que te permite rotar un elemento HTML a través de los ejes del navegador. El valor que recibe es un ángulo, por ejemplo, “45deg” (45 grados) o “2rad” (2 radianes). Los ángulos positivos están en sentido horario, y los negativos en sentido antihorario.

selector {
    transform: rotate(45deg);
}

Dependiendo del eje en el que rotes el elemento, existe una función.

Tipo	Valor con los argumentos que recibe
Eje X y Y	rotate(angle)
Eje X	rotateX(angle)
Eje Y	rotateY(angle)
Eje Z	rotateZ(angle)
Múltiple	rotate3d(x,y,z,angle)

Ejemplo usando rotate
Scale para transformaciones
Scale es una función de la propiedad transform que te permite escalar un elemento HTML a través de sus ejes. El valor que recibe es un número multiplicador al elemento original.

Si el elemento es igual a 1 entonces sigue como el original; mayor a 1 aumenta de tamaño; y, menor a 1 disminuye de tamaño.

selector {
    transform: scale(0.8);
}

Dependiendo del eje en el que escales el elemento, existe una función.

Tipo	Valor con los argumentos que recibe
Eje X y Y	scale(x)
Eje X	scaleX(x)
Eje Y	scaleY(y)
Eje Z	scaleZ(z)
Múltiple	scale3d(x,y,z)


Ejemplo usando scale
Skew para transformaciones
Skew es una función de la propiedad transform que te permite torcer un elemento HTML a través de sus ejes en dos dimensiones. El valor que recibe es un ángulo para cada eje en el que el elemento se distorsionará.

selector {
    transform: skew(45deg, 45deg);
}

Dependiendo del eje en el que tuerzas el elemento, existe una función.

Tipo	Valor con los argumentos que recibe
Eje X y Y	skew(angleX, angleY)
Eje X	skewX(angle)
Eje Y	skewY(angle)
Ejemplo usando scale
Matrix para transformaciones
Matrix es una función de la propiedad transform que te permite realizar varios efectos en uno solo.

Documentación de matrix
Orden en el código para transformaciones
Solamente puede existir una sola propiedad transform en el código de CSS, por lo que si escribimos otra regla CSS con otra transformación, esta se sobreescribirá y solo ejecutará la última. Por ende, utiliza varias funciones en la misma propiedad transform para realizar varias transformaciones.

/*Mal (solo rotará el elemento)*/

selector {
    transform: translate(100px,  100px);
    transform: rotate(45deg);
 }

 /*Bien (realizará ambas transformaciones)*/

selector {
    transform: translate(100px, 100px) rotate(45deg);
}
Contribución con aportes de: Andrés Guano.

Archivos de la clase

transform-rotate.html
transform-scale.html
transform-skew.html

Lecturas recomendadas

transform - CSS: Cascading Style Sheets | MDN

https://developer.mozilla.org/en-US/docs/Web/CSS/transform


Gradient Backgrounds – 🌈 The Best Gradient Sites All in One Place

https://cssgradient.io/gradient-backgrounds/