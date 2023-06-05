Los tips de UX son recomendaciones para que tus animaciones sean mejores para la experiencia de usuario. Estudiaremos tres, los cuales son:

Movimiento impulsado por la acción.
Tiempos de espera.
Problemas de parpadeo.
Movimiento impulsado por la acción
Al momento de crear una transición, el tiempo del punto A al punto B es el mismo. El movimiento impulsado por la acción consiste en modificar los tiempos de la transición, para que el tiempo de regreso (de B a A) sea mayor, para que la animación repose y no exista un movimiento abrupto.

Esto se consigue añadiendo la transición en el accionador de la animación y en el elemento, pero con diferentes tiempos. Ten en cuenta que la animación primero sucede con el evento.

/* De A a B */
selector:hover {
    transition: transform 1s;
}

/* De B a A */
selector {
    transition: transform 1.5s;
}
Ejemplo empleando el movimiento impulsado por la acción.
Contribución creada por Andrés Guano.

Archivos de la clase
ux-movimiento-impulsado-por-la-accion.html
Lecturas recomendadas

transition - CSS: Cascading Style Sheets | MDN

https://developer.mozilla.org/en-US/docs/Web/CSS/transition