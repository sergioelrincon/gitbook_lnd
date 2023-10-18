# vCard

## Descripción

El lenguaje de marcas vCard es un estándar ampliamente utilizado para representar y compartir información de contacto de una persona o entidad en un formato estructurado y legible por máquinas. Cada "vCard" se compone de una serie de campos que describen datos personales como el nombre, dirección, número de teléfono, dirección de correo electrónico, sitio web y mucho más. Estas tarjetas de contacto son especialmente útiles en la gestión de contactos en aplicaciones de correo electrónico, libretas de direcciones electrónicas y otras aplicaciones relacionadas con la comunicación. vCard facilita la transferencia y el intercambio de información de contacto de una manera estandarizada, lo que significa que los usuarios pueden compartir sus datos de contacto con facilidad, independientemente de la plataforma o la aplicación que utilicen. Además, las vCards también pueden incluir imágenes de perfil, lo que las hace ideales para la identificación visual de contactos en aplicaciones de mensajería y redes sociales.

## Ejemplo

```
BEGIN:VCARD
VERSION:3.0
FN:Sergio Ramos
ORG:IES El Rincón
TEL:123-456-7890
EMAIL:sergioramos@ieselrincon.es
END:VCARD
```

* `BEGIN:VCARD` y `END:VCARD` delimitan el inicio y el final de la vCard.
* `VERSION` especifica la versión de la vCard (en este caso, 3.0).
* `FN` representa el nombre completo de la persona (Sergio Ramos).
* `ORG` describe la organización a la que pertenece la persona (IES El Rincón).
* `TEL` proporciona un número de teléfono de contacto (123-456-7890).
* `EMAIL` incluye una dirección de correo electrónico (sergioramos@ieselrincon.es)
