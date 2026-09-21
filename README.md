# LegacyHunt — sitio corporativo (web2)

Sitio estatico de **LegacyHunt**, SOC on-premise sobre lakehouse.
Publicado en GitHub Pages: https://arl3t.github.io/web2/

`index.html` es autocontenido: CSS y JS inline, fuente self-hosted en `fonts/`
(sin Google Fonts ni terceros). Sin build ni backend.

## Marca corporativa — identidad real de LegacyHunt

- **Fondo:** `#0a0e14` slate oscuro (el del isotipo oficial)
- **Texto:** `#ffffff` · `#c4d0dd` · `#9fb0c3` (atenuado) · `#6b7a8d` (faint)
- **Primario:** `#4ade80` verde neon (marca, CTA, escudo del logo)
- **Secundario:** `#5eead4` teal (etiquetas, isotipo, detalles)
- **Tipografia:** DM Sans (self-hosted). Titulares peso 700 a tamano CONTENIDO
  (hero ~48px max, secciones 30-38px); cuerpo peso 400 a 16.5px, legible
- **Logotipo oficial:** `logo-legacyhunt.png` (escudo tech + wordmark + tagline
  "Threat Monitoring & Response"), usado en el footer
- **Isotipo:** `favicon.svg` real (triangulo teal sobre slate) en nav y favicon
- **Imagen de marca:** constelacion de particulas triangulares en tonos verde/teal
  (forma organica de cerebro) en canvas + campo ambiente sutil de fondo

## Arlet — asistente SOC

Asistente client-side (sin backend) que guia al visitante: interpreta lo que escribe
o las pistas que toca, responde y lo lleva a la seccion relevante. Se abre desde el FAB
inferior derecho o desde los botones "Preguntar a Arlet".

## Stack anonimizado

El sitio describe la plataforma por **categorias genericas** (cortafuegos, SIEM, EDR,
object storage, motor SQL, base relacional, servidor de modelos local...), sin nombrar
proveedores ni productos concretos — ni en el texto ni en las palabras clave del asistente.

## Estructura

- `index.html` — landing: hero + constelacion, disciplinas, pipeline, capacidades, arquitectura, gobernanza, Arlet
- `informe-muestra.html` — informe de incidente de ejemplo
- `logo-legacyhunt.png` — logotipo horizontal oficial
- `favicon.svg` — isotipo oficial (triangulo teal)
- `fonts/` — DM Sans (woff2)

## Montaje

GitHub Pages: Settings → Pages → Deploy from branch (`main`, `/root`).
Prueba local: `python3 -m http.server 8080` → http://localhost:8080
