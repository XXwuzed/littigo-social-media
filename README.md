# Littigo · Social media
Estructura: `posts/AAAA/MM/AAAA-MM-DD_tema/` con `slides/`, PDF, `copy-<red>.md` y `meta.json` (canal, fecha, estado, id de Buffer).
Estados: borrador-local → listo → programado → publicado.
Repo público: no subir nada que no esté aprobado.

## Campos de análisis en meta.json

Para que el circuito de corrección de `mkt-littigo` (skill `littigo-analisis`) mida cada parte de la pieza, cada `meta.json` lleva también:

- `embudo`: `MOFU` o `BOFU` (`TOFU` solo en casos excepcionales).
- `formato` (`reel`, `carrusel`, `imagen`, `historia`), `origen` (`organico` o `pauta`) y `duracion_s` en reels.
- `hook`, `cuerpo`, `cierre`: IDs del banco `context/funnel-content-system.md` de `mkt-littigo` (por ejemplo `M23`, `MC04`, `MF01`).
- `hipotesis` y `variante`: solo si la pieza es parte de una prueba (por ejemplo `H05` y `A`).
- `metrica_principal`: `hook_pauta`, `cuerpo_pauta`, `acciones_cta`, `mensajes`, `conversaciones`, `envios`, `guardados`, `calificados` o `demos`.
- `anuncioMetaId` (conjunto de anuncios si se pauta) y `mensajePrellenado` (texto de WhatsApp por variante).
- `idsRetroactivos` y `notaIds`: solo en publicaciones anteriores al banco, cuando los IDs se asignaron después.

