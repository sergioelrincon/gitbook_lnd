# YAML

## Descripción

YAML (acrónimo de "YAML Ain't Markup Language" o "YAML Ain't a Markup Language") es un lenguaje que se utiliza para representar información de manera estructurada y legible por humanos. Aunque YAML comparte similitudes con lenguajes de marcas como XML y JSON, se diferencia en su enfoque en la legibilidad y simplicidad. YAML se utiliza comúnmente para la configuración de software, archivos de datos y otras aplicaciones donde la estructura de los datos es importante.

La utilidad principal de YAML radica en su capacidad para describir datos en un formato que es fácil de entender y editar para los humanos, sin requerir etiquetas o caracteres especiales excesivos. Esto hace que YAML sea especialmente útil en la configuración de aplicaciones, ya que permite a los desarrolladores y administradores definir parámetros y valores de configuración de una manera más natural y legible.

Un ejemplo común de uso de YAML es en archivos de configuración de aplicaciones, como archivos de configuración de servidores web, sistemas de automatización, contenedores Docker y más. La claridad y la estructura de YAML facilitan la comprensión y la modificación de las configuraciones, lo que lo convierte en una elección popular en el mundo de la administración de sistemas y el desarrollo de software.

## Ejemplo

```yaml
# Configuración de una aplicación
nombre: Mi Aplicación
entorno: desarrollo
servidor:
  direccion: ejemplo.com
  puerto: 8080
base_de_datos:
  motor: MySQL
  usuario: usuario_db
  contraseña: secreto123
```

* `nombre`, `entorno`, `servidor`, y `base_de_datos` son claves que representan diferentes aspectos de la configuración de la aplicación.
* Los valores pueden ser cadenas de texto, números o incluso estructuras anidadas, como el objeto `servidor` y `base_de_datos`.
* El uso de espacios y la indentación determinan la estructura jerárquica de los datos. Por ejemplo, `direccion` y `puerto` están anidados dentro del objeto `servidor`.
* Los comentarios se indican con el símbolo `#`.

