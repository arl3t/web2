# LegacyHunt — Landing comercial (web2)

Sitio estático de una sola página. `index.html` es **autocontenido**: todo el
CSS y JS van inline; las únicas referencias externas son Google Fonts
(`fonts.googleapis.com`) y enlaces `mailto:`. No hay build, dependencias ni
backend — funciona en cualquier servidor web tal cual.

## Montaje

Copiar `index.html` al docroot del servidor y listo. Ejemplos:

**Apache / cualquier hosting con docroot**
```
cp index.html /var/www/html/
```

**GitHub Pages** — Settings → Pages → Deploy from branch (`main`, `/root`).
La página queda en `https://<usuario>.github.io/web2/`.

**Prueba local rápida**
```
python3 -m http.server 8080
# → http://localhost:8080
```

Funciona igual en la raíz del dominio o bajo un subpath (`/web2/`): los enlaces
internos son anclas (`#modulos`, `#demo`, …), sin rutas absolutas.

## Actualizar

Editar `index.html` y volver a copiar/pushear. Sin pasos de build.

## Contacto

Los CTA apuntan a `info@legacy-roots.net` (enlaces `mailto:` con asunto
prellenado). Para cambiar el destinatario, buscar `mailto:` en `index.html`.
