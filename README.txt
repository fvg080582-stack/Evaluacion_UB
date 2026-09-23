# Clínica Integrada de Adultos — PWA completa

Versión: 2026.09.23.2

Incluye:
- instalación como app en iPhone/iPad;
- iconos de aplicación;
- pantalla de carga;
- Service Worker;
- caché offline del shell de la aplicación;
- actualización automática al publicar una nueva versión.

## Publicación

Sube TODO el contenido de esta carpeta a la raíz del repositorio de GitHub Pages:
- index.html
- manifest.webmanifest
- sw.js
- carpeta icons/

Después abre la URL publicada en Safari del iPhone:
Compartir → Añadir a pantalla de inicio.

## Actualizaciones

Para publicar una nueva versión, sustituye `index.html` y los archivos modificados.
Si quieres forzar una actualización del Service Worker de forma inequívoca, cambia APP_VERSION en `index.html` y `sw.js`.

## Importante

La PWA no convierte el backend en offline. Si la aplicación usa Google Sheets/Apps Script, las operaciones que dependen de ese backend seguirán necesitando Internet y sus permisos.
