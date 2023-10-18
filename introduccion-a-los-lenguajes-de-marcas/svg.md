# SVG

## Descripción

SVG, que significa Scalable Vector Graphics (Gráficos Vectoriales Escalables), es un lenguaje de marcas ampliamente utilizado en la creación de gráficos vectoriales en la web. A diferencia de los formatos de imagen tradicionales, como JPEG o PNG, SVG se basa en descripciones matemáticas de formas y objetos en lugar de píxeles, lo que significa que las imágenes SVG son escalables sin pérdida de calidad, lo que las hace ideales para gráficos, iconos, mapas y gráficos en línea. SVG es compatible con animaciones y efectos interactivos, lo que permite a los desarrolladores web crear experiencias visuales dinámicas y atractivas. Además, al ser un lenguaje de marcas, SVG se integra perfectamente con HTML, lo que facilita su uso en páginas web y aplicaciones.&#x20;

## Ejemplo

```svg
<svg width="150" height="150">
  <circle cx="50" cy="50" r="40" fill="red" />
  <rect x="20" y="20" width="60" height="40" fill="blue" />
  <line x1="10" y1="90" x2="90" y2="10" stroke="green" stroke-width="4" />
</svg>
```

* `<rect>` crea un rectángulo con la esquina superior izquierda en (20, 20), un ancho de 60 unidades y una altura de 40 unidades, y lo llena de color azul.
* `<line>` crea una línea que conecta los puntos (10, 90) y (90, 10), con un grosor de trazo de 4 unidades y de color verde gracias a las propiedades `x1`, `y1`, `x2`, `y2`, `stroke` y `stroke-width`.
