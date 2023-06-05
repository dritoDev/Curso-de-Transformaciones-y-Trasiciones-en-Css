La propiedad backface-visibility de CSS permite mostrar la cara posterior de un elemento. Esta propiedad recibe dos valores: visible (visible) y hidden (oculto); por defecto, su valor es visible.

selector {
    backface-visibility: visible;
    backface-visibility: hidden;
}
La cara posterior de un elemento siempre tiene un fondo transparente, por lo que al ser visible y realizar una transformación en un solo eje, mostrará un efecto de imagen espejo. Mira la siguiente imagen y observa cómo Alicia cambia de lugar.

Representación de la propiedad backfase-visibility
En cambio, si el valor es hidden no mostrará contenido. Con esto podemos realizar que un elemento se muestre al ocultarse otro, como un efecto de voltear una carta.

Crea el efecto de voltear una carta con backface-visibility
Como punto inicial, necesitarás un elemento padre con dos elementos hijos, los cuales representarán la cara frontal y posterior de la carta. Te dejo este código para que empieces, aunque no es obligatorio, ya que se hablará de manera general en la explicación.

Punto de partida
Ahora sigamos los siguientes pasos:

Al elemento padre agrega una posición relativa; y a los hijos, una posición absoluta. Esto provocará que los elementos hijos estén uno sobre el otro con respecto al eje Z dentro del elemento padre.
.padre {
    position: relative;
}

.hijos{
    position: absolute;
}
Al elemento padre agrega la propiedad para que la transformación sea en 3D.
.padre {
    transform-style: preserve3d;
}
Al elemento que deba estar en la vista posterior, rótalo 180 grados sobre el eje X o Y dependiendo de lo que esperes. Observarás el efecto espejo, pero aún no está listo.
.cara-posterior  {
    transform: rotateY(180deg);
}
A los elementos hijos, agrega la propiedad backface-visibility con el valor hidden. Observarás que el contenido frontal y posterior se han situado como una tarjeta. Solo faltaría añadir un accionador para la animación.
.hijos {
    backface-visibility: hidden;
}
Al elemento padre, agrega un accionador para la animación que consista en rotar todo el contenido para mostrar la vista posterior al usuario.
.padre:hover {
  transform: rotateY(180deg);
}
Y listo, tienes el efecto de voltear una tarjeta mediante la propiedad backface-visibility.

Ejercicio completo del efecto de voltear una tarjeta.
Contribución creada por Andrés Guano.

Archivos de la clase
backface-visibility.html
Lecturas recomendadas

transform - CSS: Cascading Style Sheets | MDN

https://developer.mozilla.org/en-US/docs/Web/CSS/transform


backface-visibility - CSS | MDN

https://developer.mozilla.org/es/docs/Web/CSS/backface-visibility