# KML

## Descripción

El lenguaje de marcas KML (Keyhole Markup Language) es un lenguajes de marcas basado en XML, ampliamente  utilizado para representar datos geográficos. KML es especialmente valioso en el contexto de aplicaciones de mapas, ya que permite describir de manera detallada la ubicación de puntos de interés, rutas, polígonos, imágenes y otra información geoespacial. Su principal utilidad radica en la representación y el intercambio de datos geográficos, lo que lo convierte en un formato esencial para la creación de mapas interactivos y la visualización de información espacial en aplicaciones como Google Earth y Google Maps. KML permite definir elementos como marcadores, líneas, polígonos, estilos de visualización, descripciones y enlaces multimedia asociados con ubicaciones geográficas. También admite animaciones, lo que hace que sea posible mostrar cambios en el tiempo y eventos geoespaciales a lo largo de un período.

## Ejemplo

```xml
<?xml version="1.0" encoding="UTF-8"?>
<kml xmlns="http://www.opengis.net/kml/2.2">
  <Placemark>
    <name>Oficina Central</name>
    <description>Estamos aquí.</description>
    <Point>
      <coordinates>-122.084143, 37.422006, 0</coordinates>
    </Point>
  </Placemark>
</kml>
```

* `<kml>` define el elemento raíz del documento KML.
* `<Placemark>` representa un marcador en una ubicación geográfica y contiene información sobre el nombre, descripción y coordenadas del lugar.
* `<name>` proporciona un nombre para el marcador.
* `<description>` ofrece una descripción adicional.
* `<Point>` indica que se trata de un punto geográfico.
* `<coordinates>` especifica las coordenadas de longitud, latitud y altitud del lugar.
