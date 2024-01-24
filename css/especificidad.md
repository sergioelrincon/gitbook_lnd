# Especificidad

## ¿Qué es la especificidad?

La especificidad en CSS es una forma de determinar qué regla se aplica a un elemento cuando hay varias reglas que lo afectan. La especificidad se basa en el tipo y el número de selectores que componen cada regla. Cuanto más específico sea el selector, más prioridad tendrá sobre los demás. La especificidad se puede entender como una medida de la fuerza o el peso de una regla CSS.

## ¿Cómo se calcula la especificidad?

La especificidad de una regla CSS se puede calcular siguiendo un sistema de puntos que asigna un valor a cada tipo de selector. Los tipos de selectores son, de menor a mayor especificidad:

* Selectores de tipo o etiqueta: por ejemplo, `p`, `div`, `h1`, etc. Tienen un valor de **1 punto**.
* Selectores de clase, atributo o pseudo-clase: por ejemplo, `.clase`, `[href]`, `:hover`, etc. Tienen un valor de **10 puntos**.
* Selectores de id o pseudo-elemento: por ejemplo, `#id`, `::before`, `::after`, etc. Tienen un valor de **100 puntos**.
* Estilos en línea: por ejemplo, `style="color: red;"`. Tienen un valor de **1000 puntos**.
* La palabra clave `!important`: por ejemplo, `color: red !important;`. Tiene un valor de **infinito** y siempre sobrescribe cualquier otra regla.

Para calcular la especificidad de una regla CSS, se suman los puntos de cada selector que la compone. Por ejemplo, la regla `div#id.clase p::first-line` tiene una especificidad de **112 puntos**, porque tiene un selector de tipo (1), un selector de id (100), un selector de clase (10) y un selector de pseudo-elemento (1). La regla que tenga mayor especificidad será la que se aplique al elemento. En caso de empate, se aplica la regla que esté más abajo en el código.
