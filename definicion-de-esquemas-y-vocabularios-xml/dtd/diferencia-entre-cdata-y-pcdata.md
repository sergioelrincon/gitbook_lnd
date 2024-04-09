# Diferencia entre CDATA y PCDATA

En XML, los tipos de datos `CDATA` y `PCDATA` se utilizan para especificar el tipo de contenido permitido en los elementos y atributos.

`CDATA` significa "datos de caracteres" (character data) y se utiliza para permitir cualquier tipo de contenido en un atributo o elemento, incluyendo caracteres especiales de XML como `<`, `>`, `&`, `'` o `"`. Los datos `CDATA` no se analizan ni se interpretan como parte del marcado XML, sino que se tratan simplemente como texto.

`PCDATA` significa "datos de caracteres de texto analizable" (parsed character data) y se utiliza para permitir sólo contenido de texto en un elemento. El contenido de `PCDATA` se analiza y se interpreta como parte del marcado XML y, por lo tanto, no puede contener caracteres especiales de XML sin ser escapados o codificados correctamente.
