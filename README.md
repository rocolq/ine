# LeeINE

Sitio estático para leer texto de imágenes de una credencial para votar INE. Está preparado para publicarse gratis con GitHub Pages.

## Publicar en GitHub Pages

1. Crea un repositorio en GitHub y sube todos los archivos de esta carpeta, conservando la carpeta `.github/workflows`.
2. En el repositorio, abre **Settings → Pages**.
3. En **Build and deployment**, elige **GitHub Actions** como fuente.
4. Sube un cambio a la rama `main`. El flujo publicará el sitio automáticamente.
5. En **Actions**, espera a que termine el flujo `Publicar LeeINE en GitHub Pages`. GitHub mostrará la dirección del sitio en el resumen del despliegue.

## Privacidad

- La imagen y el texto reconocido se procesan en el navegador; la app no tiene backend ni guarda esos datos.
- En celular, marca el consentimiento y toca **Tomar foto con la cámara del celular**. El navegador solicitará permiso al abrir la cámara trasera; el marco adapta la captura a la proporción de la credencial. Para usar la cámara, abre el sitio publicado por HTTPS.
- Para cargar la biblioteca OCR y las fuentes se requiere conexión a Internet. El navegador descarga Tesseract.js desde jsDelivr y las fuentes desde Google Fonts; la imagen de la INE no se envía a esos servicios.
- GitHub Pages sirve el código públicamente. No incluyas fotos reales de identificaciones en este repositorio.
- El OCR puede equivocarse. Revisa cada campo antes de usarlo.

## Archivos

- `index.html`: aplicación web.
- `.github/workflows/pages.yml`: publicación automática con GitHub Pages.
