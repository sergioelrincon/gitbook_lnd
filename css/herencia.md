# Herencia

La herencia en CSS es un mecanismo que permite a los elementos HTML recibir los valores de algunas propiedades CSS de sus elementos padres. Esto facilita la creación de estilos consistentes y evita la repetición de código. Por ejemplo, si defines el color de la fuente de un elemento `<body>` como negro, todos los elementos dentro del `<body>` heredarán ese color, a menos que se especifique otro diferente.

Sin embargo, no todas las propiedades CSS son heredables. Algunas propiedades solo afectan al elemento al que se aplican, y no se transmiten a sus descendientes. Por ejemplo, el ancho y el alto de un elemento no se heredan, sino que se calculan en función del contenido y el diseño del elemento. [Para saber si una propiedad es heredable o no, puedes consultar la documentación de CSS](https://developer.mozilla.org/es/docs/Learn/CSS/Building\_blocks/Cascade\_and\_inheritance)[1](https://developer.mozilla.org/es/docs/Learn/CSS/Building\_blocks/Cascade\_and\_inheritance)[2](https://developer.mozilla.org/es/docs/Web/CSS/inheritance) o usar herramientas como el inspector de elementos del navegador.

La herencia en CSS está relacionada con la cascada, ya que las reglas que se aplican a un elemento pueden afectar a los valores que heredan sus hijos. Por ejemplo, si hay una regla que cambia el color de la fuente de un elemento `<div>` que contiene un párrafo, el párrafo heredará el nuevo color, a menos que tenga una regla propia que lo sobrescriba. Por eso, es importante entender cómo funciona la especificidad y el orden de las reglas en CSS, para evitar conflictos o inconsistencias en los estilos.

Puedes encontrar más información sobre herencia y ejemplos [en la siguiente web](https://codigofacilito.com/articulos/la-herencia-en-css).
