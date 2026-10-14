                localStorage.setItem('sb_cart_v1', JSON.stringify(cart));# Sweet Bites — Sitio listo para GitHub Pages

Este repositorio contiene una página estática (HTML/CSS/JS) para "Sweet Bites" preparada para desplegar en GitHub Pages.

¿Cómo publicar en GitHub Pages?
1. Crea un nuevo repositorio en tu cuenta de GitHub o sube estos archivos a uno existente.
2. Añade los archivos tal cual están:
   - Coloca `index.html` y otros recursos dentro de la carpeta `docs/` (ya está preparado como `docs/index.html` en este paquete).
   - Alternativamente, puedes colocar `index.html` en la raíz y usar la opción `main` branch / `root` folder para Pages.
3. En la configuración del repositorio (Settings → Pages):
   - Fuente (Source): selecciona "Deploy from a branch".
   - Branch: `main` (o `master` según tu caso).
   - Folder: selecciona `/docs` si usaste la carpeta `docs/`, o `/ (root)` si pusiste `index.html` en la raíz.
4. Guarda la configuración. GitHub procesará el sitio y en unos minutos te dará una URL `https://<tu-usuario>.github.io/<repo>/` (o `https://<tu-usuario>.github.io/` para repositorios con nombre `<usuario>.github.io`).

Notas y recomendaciones
- El formulario de checkout actualmente muestra un alert y no envía a ningún servicio externo. Para producción conecta `finalizeOrder()` a tu backend, a un servicio de mensajería (WhatsApp API) o a un procesador de pagos (Stripe, PayPal).
- Si quieres separar los assets (CSS/JS) en archivos estáticos, muévelos a `docs/assets/` y actualiza las referencias en `index.html`.
- Si prefieres usar la rama `gh-pages`, crea la rama `gh-pages` y pon `index.html` en la raíz, y luego selecciona `gh-pages` como fuente en Settings → Pages.

¿Quieres que lo suba yo al repo y lo publique?
Puedo:
- Generar la estructura del repo y crear los archivos allí (si me das permiso para crear el repo).
- O guiarte paso a paso para que lo subas desde tu máquina usando git.

¡Listo! Si quieres, hago la versión con CSS/JS en archivos separados y añado un simple backend (GitHub Actions + Google Sheets, o un endpoint mock) para que los pedidos se almacenen.
