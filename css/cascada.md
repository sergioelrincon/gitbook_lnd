# Cascada

## Concepto de cascada

El concepto de "cascada" en CSS (Cascading Style Sheets) es fundamental para entender cómo se aplican los estilos a los elementos en una página web. La palabra "cascada" se refiere al proceso por el cual se determina el estilo final de un elemento HTML, considerando múltiples reglas de estilo que podrían aplicarse a ese elemento. Este proceso se rige por tres factores principales:

1. **Origen de la regla de estilo**: Las reglas de estilo pueden provenir de diferentes orígenes, como el navegador (estilos predeterminados), el usuario (estilos definidos por el usuario en su navegador) y el desarrollador (estilos definidos en hojas de estilo externas, internas o en línea).\
   Los estilos definidos por el usuario en su navegador son un conjunto de reglas de CSS que un usuario puede especificar para que se apliquen a todas las páginas web que visita. Los navegadores modernos generalmente permiten a los usuarios especificar estos estilos a través de sus opciones de configuración, aunque el método exacto puede variar de un navegador a otro.  Es importante destacar que los estilos definidos por el usuario tienen una alta prioridad en la cascada de CSS. Esto significa que, a menos que una regla de estilo definida por el desarrollador sea marcada como `!important`, los estilos del usuario pueden sobrescribir los estilos definidos en las hojas de estilo de las páginas web.
2. **Especificidad**: La especificidad es un sistema de puntuación que determina qué reglas de estilo se aplican a un elemento. Esta puntuación se calcula en base a los tipos de selectores utilizados en una regla CSS. Por ejemplo, los selectores de ID tienen una especificidad mayor que los selectores de clase, que a su vez tienen una especificidad mayor que los selectores de etiquetas.
3. **Orden de las declaraciones**: Si dos reglas tienen la misma especificidad, la última regla declarada en el código será la que se aplique. Esto es especialmente relevante cuando se utilizan múltiples hojas de estilo o cuando se incluyen estilos en diferentes partes de un documento HTML.

El proceso de cascada garantiza que se apliquen los estilos más relevantes y específicos a cada elemento, permitiendo una gran flexibilidad y control en el diseño de páginas web. Es importante entender este concepto para escribir CSS eficaz y para diagnosticar y resolver problemas relacionados con la aplicación de estilos.

