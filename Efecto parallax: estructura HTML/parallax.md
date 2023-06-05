El efecto de paralaje o parallax es una técnica en la que el fondo se mueve a una velocidad distinta que la del contenido. El resultado es un ligero efecto de profundidad, dejando ver partes que antes no podías visualizar. Te ayuda a sumergirte totalmente en el contenido, similar al efecto 3D.

30 Webs con efecto Parallax
Estructura HTML para el efecto parallax
Crea un contenedor con elementos hijos, estos serán las capas del contenedor para crear el efecto. En este caso, agrega tres elementos que representen la capa del fondo (background), del medio (middle) y de primer plano (foreground). Cada elemento debe tener una clase general y una que las diferencie.

<div class="parallax-container">
  <div class="image image_background"></div>
  <div class="image image_middle"></div>
  <div class="image image_foreground"></div>
</div>
En la capa del medio, crea tres elementos hijos que representen tres cartas.

<div class="image image_middle">
    <div class="card one"></div>
    <div class="card two"></div>
    <div class="card three"></div>
</div>
Para las demás capas, agrega una imagen de fondo y una en primer plano de Alicia. Te dejo los enlaces de las imagenes, utiliza una etiqueta de imagen con su respectivo atributo alt.

* [Alicia](https://i.ibb.co/vJdbRkj/Alice.png)
* [Imagen de fondo](https://i.ibb.co/jbLKgvX/Background.png)
Y listo, ya tienes la estructura del efecto parallax, no importa si las imágenes están sobredimensionadas. Ahora utilizaremos CSS para dar estilos a las capas.

Estructura HTML completa
Contribución creada por Andrés Guano, con aportes de Carlos Mazzaroli.

Archivos de la clase
parallax-1.html
Lecturas recomendadas

https://i.ibb.co/vJdbRkj/Alice.png

https://i.ibb.co/vJdbRkj/Alice.png


https://i.ibb.co/jbLKgvX/Background.png

https://i.ibb.co/jbLKgvX/Background.png

Ahora que ya está la estructura HTML para el efecto parallax, es momento de agregar los estilos CSS.

Estilos CSS para el efecto parallax
Quita el margin que está por defecto establecido por el navegador.

body {
  margin: 0;
}
Dimensiona las imágenes para que ocupen el espacio del contenedor.

img{
  max-width: 100%;
  height: auto;
}
En el elemento contenedor (parallax-container) agrega:

Medidas para que ocupe el ancho y alto de la pantalla.
Perspectiva de 8 píxeles (recuerda este valor).
Posición relativa para que las capas puedan posicionarse con respecto al contenedor del efecto.
En este caso, el exceso de contenido deberá estar oculto para el eje X y desplazable para el eje Y, pero lo puedes cambiar a tu gusto.
.parallax-container {
  width: 100%;
  height: 100vh;
  perspective: 8px;
  overflow-x: hidden;
  overflow-y: scroll;
  position: relative;
}
Agrega la posición absoluta a todos los elementos hijos o capas del efecto.

.image{
  position: absolute;
} 
Para las cada capa del efecto vamos a realizar lo siguiente:

Medidas según sean necesarias.
Trasladar la capa en eje Z, desde 0 hasta el valor de la perspectiva (8px).
Escalar el elemento según su profundidad. Para calcular este valor utiliza la siguiente fórmula: $(perspective - translateZ) / perspective$, por ejemplo para la capa del medio, $(8-5)/8 = 0.375$.
Modificar el origen según sea necesario.
Algunos valores no son necesarios colocar, pero es recomendable tener un control del código y de las propiedades CSS.

.image_background{
  width: 100%;
  height: auto;
  transform: translateZ(0px) scale(1);
  transform-origin: 0 50%;
}

.image_middle{
  width: 100%;
  height: 100%;
  transform: translateZ(5px) scale(0.375);
  transform-origin: 50%;
}

.image_foreground{
  width: 100%;
  height: auto;
  transform: translateZ(2px) scale(0.75);
  transform-origin: top;
}
Para las cartas de la segunda capa agrega dos estilos importantes: las medidas y la posición absoluta.

.card {
  width: 80px;
  height: 100px;
  position: absolute;
  /* Estilos propios de la carta */
  background: white;
  border-radius: 8px;
  transform: rotate(-20deg);
}
La posición sirve para posicionar cada carta como deseemos.

> Valores al azar, modificálos a tu gusto. 
.one {
  left: 30%;
}

.two{
  right: 20%;
  top: 200px;

}

.three{
  right: 20%;
  bottom: -700px;
}

¡Y listo! Ya está construido el efecto parallax.

Efecto Parrallax.
Contribución creada por Andrés Guano.

Clases relacionadas

Lecturas recomendadas

https://i.ibb.co/vJdbRkj/Alice.png

https://i.ibb.co/vJdbRkj/Alice.png


https://i.ibb.co/jbLKgvX/Background.png

https://i.ibb.co/jbLKgvX/Background.png