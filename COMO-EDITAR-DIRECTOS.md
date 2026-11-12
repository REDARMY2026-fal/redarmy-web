# Cómo editar los directos de REDARMY

Este archivo permite publicar o actualizar el anuncio de los próximos directos sin tocar el diseño de la web.

## Pasos

1. Entrá a [GitHub](https://github.com/REDARMY2026-fal/redarmy-web).
2. Abrí el archivo `directos.json`.
3. Tocá el lápiz (**Edit this file**).
4. Cambiá los valores que necesites, sin borrar las comillas ni las comas.
5. Tocá **Commit changes** para guardar.
6. Esperá un momento y actualizá la página de REDARMY.

**No compartas tu contraseña, códigos de verificación ni tokens.** Para editar este archivo, iniciá sesión directamente en GitHub.

## Estados disponibles

- `none`: todavía no hay fecha confirmada.
- `scheduled`: hay un directo anunciado.
- `cancelled`: el directo fue cancelado.
- `finished`: el directo ya terminó.

## Ejemplo: anunciar un directo

Cambiá el contenido de `directos.json` por algo como esto y completá los datos:

```json
{
  "status": "scheduled",
  "title": "Directo de Brawl Stars",
  "game": "Brawl Stars",
  "date": "Sábado 21 de noviembre",
  "time": "22:00",
  "timezone": "Argentina (UTC-3)",
  "platform": "YouTube",
  "message": "¡Nos vemos en vivo! Activá el recordatorio en el canal.",
  "url": "https://www.youtube.com/@REDARMYGAMER2027"
}
```

## Qué significa cada campo

- `status`: estado del anuncio.
- `title`: título principal que verá la gente.
- `game`: juego o tema del directo.
- `date`: fecha escrita como quieras mostrarla.
- `time`: horario local del directo.
- `timezone`: zona horaria; conviene indicar Argentina (UTC-3).
- `platform`: plataforma donde será el directo.
- `message`: mensaje breve para la comunidad.
- `url`: enlace https al canal o al directo.

Para volver al estado inicial, poné `status` en `none`. Los campos pueden quedar vacíos cuando no correspondan.
