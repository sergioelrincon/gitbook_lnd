# A-FRAME

## Descripción

A-Frame es un framework o marco de trabajo de código abierto diseñado para la creación de experiencias de realidad virtual (RV) y realidad aumentada (RA) en la web. Se basa en HTML y es una extensión de HTML que permite a los desarrolladores web crear contenido de RV y RA de forma fácil y accesible. La utilidad principal de A-Frame radica en su capacidad para democratizar el desarrollo de experiencias inmersivas, ya que utiliza una sintaxis HTML declarativa que es familiar para los desarrolladores web. Esto facilita la creación de escenas tridimensionales y objetos interactivos, lo que anteriormente requería conocimientos más profundos en programación 3D.

A-Frame proporciona una serie de componentes y primitivas que permiten a los desarrolladores agregar gráficos en 3D, interactividad, seguimiento de movimiento y características de RV y RA a sus aplicaciones web. Esto hace que sea más accesible para una amplia gama de profesionales, desde desarrolladores web experimentados hasta diseñadores y creadores de contenido. Además, A-Frame es compatible con múltiples plataformas y dispositivos, lo que significa que las experiencias de RV y RA creadas con A-Frame se pueden ejecutar en una variedad de navegadores y dispositivos, incluyendo gafas de RV, smartphones y computadoras de escritorio.

## Ejemplo

```html
<!DOCTYPE html>
<html>
  <head>
    <script src="https://aframe.io/releases/1.2.0/aframe.min.js"></script>
  </head>
  <body>
    <a-scene>
      <a-box position="0 1.6 -4" rotation="0 45 0" color="red"></a-box>
      <a-sky color="#222"></a-sky>
    </a-scene>
  </body>
</html>
```

* Se incluye la biblioteca A-Frame a través del script en el encabezado del documento HTML.
* Dentro del cuerpo del documento, `<a-scene>` define la escena de A-Frame.
* `<a-box>` crea un cubo en la posición (0, 1.6, -4) con una rotación de 45 grados y un color rojo.
* `<a-sky>` agrega un fondo de color al entorno de la escena.
