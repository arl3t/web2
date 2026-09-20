# LegacyHunt — sitio corporativo (web2)

Sitio estatico de **LegacyHunt**, SOC on-premise sobre lakehouse.
Publicado en GitHub Pages: https://arl3t.github.io/web2/

`index.html` es autocontenido: CSS y JS inline, fuente self-hosted en `fonts/`
(sin Google Fonts ni terceros). Sin build ni backend.

## Marca corporativa — sistema "void"

- **Fondo:** `#000000` negro absoluto (el vacio es el diseno; sin tarjetas, bordes ni sombras)
- **Texto:** `#ffffff` · `#9a9a9a` (atenuado) · `#bdbdbd` (terciario)
- **Accion:** `#8052ff` Electric Iris — unico boton relleno y color de marca
- **Enfasis:** `#ffb829` Saffron Spark — etiquetas y resaltados
- **Gradiente de logo:** `#8052ff` → `#15846e`
- **Tipografia:** DM Sans (self-hosted, sustituto de PPNeueMontreal). Jerarquia por
  ESCALA, no por peso: titulares en peso 400 a gran tamano; cuerpo en peso 200 (ultra-light)
- **Logotipo:** marca triangular (gradiente violeta→teal + chispa ambar) + wordmark "LegacyHunt"
- **Imagen de marca:** constelacion de particulas triangulares multicolor (forma organica
  de cerebro) renderizada en canvas + campo ambiente de fondo

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
- `fonts/` — DM Sans (woff2)

## Montaje

GitHub Pages: Settings → Pages → Deploy from branch (`main`, `/root`).
Prueba local: `python3 -m http.server 8080` → http://localhost:8080
