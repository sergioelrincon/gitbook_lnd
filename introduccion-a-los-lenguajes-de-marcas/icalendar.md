# iCalendar

## Descripción

El lenguaje iCalendar, a menudo representado en archivos con la extensión .ics, es un estándar ampliamente utilizado para la creación, distribución y el intercambio de información de calendario en formato de texto. Este lenguaje de marcas se utiliza para describir eventos, tareas, reuniones y recordatorios en un formato estructurado y legible tanto para humanos como para aplicaciones. iCalendar es especialmente valioso en la gestión de calendarios y la programación, ya que permite a los usuarios compartir eventos entre diferentes aplicaciones y plataformas de calendario, como Google Calendar, Outlook, Apple Calendar y muchas otras. Además, iCalendar admite datos como la fecha y hora de inicio y finalización de un evento, ubicación, descripciones, invitados y recordatorios, lo que lo convierte en una herramienta esencial para la organización de agendas personales y eventos compartidos en entornos empresariales.

## Ejemplo

```
BEGIN:VCALENDAR
VERSION:2.0
BEGIN:VEVENT
DTSTART:20231018T100000
DTEND:20231018T120000
SUMMARY:Reunión de equipo
LOCATION:Sala de Conferencias
DESCRIPTION:Una reunión para revisar el progreso del proyecto.
END:VEVENT
END:VCALENDAR
```

* `BEGIN:VCALENDAR` y `END:VCALENDAR` delimitan el inicio y el final del calendario.
* `BEGIN:VEVENT` y `END:VEVENT` delimitan el inicio y el final de un evento.
* `DTSTART` define la fecha y hora de inicio del evento (en este caso, el 18 de octubre de 2023 a las 10:00).
* `DTEND` define la fecha y hora de finalización del evento (el mismo día a las 12:00).
* `SUMMARY` proporciona un resumen o título para el evento.
* `LOCATION` especifica la ubicación del evento.
* `DESCRIPTION` ofrece una descripción más detallada del evento.
