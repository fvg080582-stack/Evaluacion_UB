# Clínica Integrada de Adultos — PWA completa

Incluye lector de alumnos mediante cámara:
- QR
- códigos de barras 1D habituales (por ejemplo Code 128, Code 39, EAN, UPC, ITF)
- algunos formatos 2D adicionales

El lector utiliza ZXing en navegador como primera opción y BarcodeDetector como alternativa cuando está disponible.

## Publicación

Sube TODO el contenido de esta carpeta a la raíz del repositorio de GitHub Pages:
- index.html
- manifest.webmanifest
- sw.js
- carpeta icons/

Después abre la URL publicada en Safari del iPhone.

Para que la cámara funcione, la aplicación debe abrirse desde HTTPS, como la URL de GitHub Pages. No funcionará correctamente abriendo el HTML directamente desde Archivos.

## Uso

En «1 · Identificar alumno»:
1. Pulsa «Escanear QR / código de barras».
2. Autoriza el acceso a la cámara la primera vez.
3. Enfoca el QR o código de barras del alumno.
4. La aplicación lee el contenido.
5. Si el código contiene o es el NIUB, selecciona automáticamente al alumno y continúa con su ficha.

También se mantiene la búsqueda manual por NIUB o nombre.

## Actualizaciones

Versión PWA: 2026.09.23.3

Al publicar una versión nueva, cambia APP_VERSION en index.html y sw.js si quieres forzar la actualización del Service Worker.

## Importante

La PWA no convierte el backend en offline. Si la aplicación usa Google Sheets/Apps Script, las operaciones que dependen de ese backend seguirán necesitando Internet y sus permisos.
