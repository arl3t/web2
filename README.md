# LegacyHunt — sitio corporativo (web2)

Sitio estatico de **LegacyHunt**, plataforma SOC/MDR on-premise sobre lakehouse.
Publicado en GitHub Pages: https://arl3t.github.io/web2/

`index.html` es autocontenido: todo el CSS y JS van inline y las fuentes son
self-hosted en `fonts/` (sin Google Fonts ni terceros). No hay build ni backend.

## Marca corporativa (nexus-dark)

Derivada de la propia plataforma. Tokens en `:root` de `index.html`:

- **Base:** `#0A1428` fondo · `#0F1F3A` tarjeta · `#1E2F52` borde
- **Texto:** `#FFFFFF` · `#A3B8D9` atenuado
- **Acentos:** `#7CFF4D` lime (primario, caza/confirmado) · `#14E9C8` cyan (analisis) ·
  `#6FA8FF` azul (datos) · `#BFA3FF` violeta (IA) · `#FF4D6E` rojo (amenaza) · `#FFB74D` ambar
- **Tipografia:** DM Sans (texto) + JetBrains Mono (dato/codigo), self-hosted en `fonts/`
- **Logotipo:** radar/mira concentrica con punto lime — wordmark "Legacy**Hunt**"
- **Voz:** tecnica y directa, en castellano. Detectar · Priorizar · Cazar · Responder · Aprender

## Estructura

- `index.html` — landing: hero, pipeline, capacidades, integraciones, arquitectura, gobernanza
- `informe-muestra.html` — informe de incidente de ejemplo
- `fonts/` — DM Sans + JetBrains Mono (woff2)

## Montaje

GitHub Pages: Settings → Pages → Deploy from branch (`main`, `/root`).
Prueba local: `python3 -m http.server 8080` → http://localhost:8080

Los enlaces internos son anclas, funciona igual en la raiz o bajo `/web2/`.
