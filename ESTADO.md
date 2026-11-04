# Budines by Sofi — estado

## Qué es
Tienda de budines artesanales. Node/Express sin build step, HTML + JS vanilla en `public/`, Google Sheets como base.
Corre en Render detrás de Cloudflare en budines-by-sofi.com.ar y despliega `main`.

## Mapa de páginas
- `/` — landing (`public/landing.html`)
- `/catalogo` — catálogo con carrito y pedido por WhatsApp (`public/index.html`)
- `/admin.html` — panel de administración

## 2026-11-04 — Landing con hero nuevo, sin restricción San Isidro
Hecho:
- Landing: hero full-bleed con foto real, header solo logo transparente, tiles con flecha, franja "Cómo pedir" (3 pasos), sin banner ni sección de zona. Un solo CTA ("Ver catálogo"); WhatsApp queda en el botón flotante ("Hola! Quiero hacer un pedido.").
- Catálogo: fuera banner y bloque de zona; subtítulo "Budines artesanales, horneados a pedido."; header sticky en top:0; el número de WhatsApp del carrito tiene fallback fijo si /config-publico no responde.
- Textos de meta/schema/`seo.js`/`/llms.txt`/checkout-exito/pendiente sin "solo en San Isidro" ni lista de barrios. San Isidro queda como ubicación en title y areaServed.
Diferido:
- El checkout oculto (`#pantallaCheckout`) y la validación de zona en `server.js` siguen limitados a San Isidro.
