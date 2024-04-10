# Diferencia entre CDATA y PCDATA

En XML, los tipos de datos `CDATA` y `PCDATA` se utilizan para especificar el tipo de contenido permitido en los elementos y atributos.

`CDATA` significa "datos de caracteres" (character data) y se utiliza para permitir cualquier tipo de contenido en un atributo o elemento, incluyendo caracteres especiales de XML como `<`, `>`, `&`, `'` o `"`. Los datos `CDATA` no se analizan ni se interpretan como parte del marcado XML, sino que se tratan simplemente como texto.

`PCDATA` significa "datos de caracteres de texto analizable" (parsed character data) y se utiliza para permitir sólo contenido de texto en un elemento. El contenido de `PCDATA` se analiza y se interpreta como parte del marcado XML y, por lo tanto, no puede contener caracteres especiales de XML sin ser escapados o codificados correctamente.

#### Ejemplo

Imaginemos que estamos definiendo un documento XML para libros y queremos incluir tanto descripciones (que pueden contener entidades como `&lt;` para `<`) como fragmentos de código (que deberían ser interpretados literalmente). Podríamos tener un DTD como el siguiente:

```xml
xmlCopy code<!DOCTYPE libro [
<!ELEMENT libro (titulo, descripcion, codigo)>
<!ELEMENT titulo (#PCDATA)>
<!ELEMENT descripcion (#PCDATA)>
<!ELEMENT codigo (#CDATA)>
]>
```

Y un documento XML correspondiente podría ser:

```xml
xmlCopy code<libro>
    <titulo>Ejemplo de PCDATA y CDATA</titulo>
    <descripcion>Este es un ejemplo de cómo utilizar &lt;PCDATA&gt; y &lt;CDATA&gt;.</descripcion>
    <codigo><![CDATA[function ejemplo() { return "<esto es código>"; }]]></codigo>
</libro>
```

En este ejemplo, la descripción utiliza `&lt;` para representar el símbolo `<` literalmente, ya que está definida como PCDATA y por lo tanto el analizador intentará interpretar cualquier entidad o marcado. Por otro lado, el contenido dentro de `<![CDATA[ ... ]]>` en el elemento `codigo` es interpretado como texto literal, permitiendo que el código JavaScript contenga `<` y `>` sin ser malinterpretado como marcado XML.
