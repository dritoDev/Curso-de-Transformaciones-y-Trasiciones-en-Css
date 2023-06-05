## Propiedades para crear animaciones con CSS y propiedades animables

Al principio de nuestra historia, Alicia cae en una cueva dirigiéndose un salón donde observa una bebida con una frase: “Bébeme”. Esta bebida provoca que Alicia disminuya su estatura para que pueda accede al mundo de las animaciones.

Esa bebida representa tres propiedades fundamentales: transform, transition y animation. Cada propiedad contiene elementos que nos ayudarán en la construcción de animaciones, revísalas en la Cheat Sheet de cada una.

# Transform
La propiedad transform sirve para transformar un elemento HTML mediante funciones. Estas funciones permitirán trasladar, escalar, rotar o torcer a lo largo, ancho y profundidad del elemento.

Sin embargo, el usuario mira el resultado final de esta transformación. Por ejemplo, todos mirarán a Alicia pequeña, y no sabrán que realmente era grande. Por eso, esta propiedad está relacionada con transition para crear una animación.

> Transform Cheat Sheet

## Transition

La propiedad transition sirve para agregar un intervalo de tiempo a un elemento HTML para visualizar los cambios de un punto inicial A, a un punto final B.

Animación de las propiedades transition y transform
Cabe recalcar, con transform y transition solamente podemos manipular la posición inicial y la final, no las posiciones intermedias. Si se requiere crear una animación manipulando las posiciones intermedias, es necesario usar animation.

> Transition Cheat Sheet

## Animation

La propiedad animation sirve para cambiar estilos CSS a lo largo de un intervalo, consiste en reglas para un estado inicial, final e intermedios que conformarán una animación.

> Animation Cheat Sheet

En este curso nos enfocaremos solamente en transition y transform, después seguir con el Curso de Animaciones con CSS, en el cual se abarcará la propiedad “animation”.


Básicamente la propiedad transform() nos permité modificar cualquier elemento que tengamos, podemos agrandarla, achicarla, escalarla, moverla, girarla, etc. Solo con esta propiedad ya tenemos las suficiente herramientas para manipular nuestro elemento, es decir, con ella ya podemos hacer que nuestro elemento se mueva a X posición, o que gire X grados 😄.
.
Sin embargo, únicamente con esta propiedad no lograremos ver ninguna animación, es decir, si tu usas la propiedad, verás que al cargar la página, el elemento aparecerá ya con la propiedad apicada, por ejemplo, si lo moviste 6 pixeles a la derecha entonces el elemento ya aparecerá movido, y es aquí donde entra transition. Esta propiedad permite generar ese movimiento, pero para ello necesita un punto inicial y un punto final.
.
Imagina que quieres mover un elemento 6 píxeles a la derecha, entonces, tu estado inicial va a ser 0 píxeles (cuando aún no se ha movido) y tu estado final va a ser 6 píxeles (cuando ya se movió), y la propiedad transition se encargará se que ese movimiento se vea suave, es decir, lo animará 👇