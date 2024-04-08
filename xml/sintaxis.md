# Sintaxis

## Recursos

* [Validador XML](https://www.xmlvalidation.com)

## Contenidos

* [Estructura de árbol](https://www.w3schools.com/xml/xml\_tree.asp)
* [Reglas sintácticas](https://www.w3schools.com/xml/xml\_syntax.asp)
* [Elementos](https://www.w3schools.com/xml/xml\_elements.asp)
* [Atributos](https://www.w3schools.com/xml/xml\_attributes.asp)
* [Espacios de nombres](https://www.w3schools.com/xml/xml\_namespaces.asp)

{% code title="ejemplo.xml" overflow="wrap" %}
```xml
<!-- Datos de Contacto -->
<contacto xmlns:c="http://www.ejemplo.com/contactos">
    <c:nombre>Juan Pérez</c:nombre>
    <c:email>juan.perez@example.com</c:email>
</contacto>

<!-- Datos del Evento -->
<evento xmlns:e="http://www.ejemplo.com/eventos">
    <e:nombre>Taller de Seguridad Informática</e:nombre>
    <!-- Integrando información de contacto -->
    <e:participante xmlns:c="http://www.ejemplo.com/contactos">
        <c:nombre>Maria López</c:nombre>
        <c:email>maria.lopez@example.com</c:email>
    </e:participante>
</evento>

```
{% endcode %}

* [Validación de documentos XML bien formados](https://www.w3schools.com/xml/xml\_validator.asp)
