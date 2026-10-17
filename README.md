# Ahora

Agenda, cine y gym en una sola app instalable. Se abre a pantalla completa desde la pantalla de inicio, funciona sin conexión y guarda los datos en el propio móvil.

- **Agenda** (negro): días deslizables, línea de la hora actual, pendientes y notas. Se escribe como se habla: "dentista el martes a las 10", "llamar al taller mañana", "nota: regalos, libro, auriculares".
- **Cine** (rojo): películas vistas en sala, con nota, foto opcional y resumen del año.
- **Gym** (blanco): días entrenados, racha semanal, peso con media de 7 días y checklist diario.

Hecho con HTML, CSS y JavaScript sin dependencias. PWA con manifest y service worker.

## Publicarla en GitHub Pages

1. Crea un repositorio nuevo en GitHub, por ejemplo `ahora`.
2. Sube todo el contenido de esta carpeta (`index.html`, `manifest.webmanifest`, `sw.js`, `icons/` y este README) a la raíz del repositorio.
3. En el repositorio: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, rama `main`, carpeta `/ (root)`. Guarda.
4. En un minuto estará en `https://TU-USUARIO.github.io/ahora/`.

## Instalarla en el iPhone

1. Abre esa dirección en **Safari**.
2. **Compartir → Añadir a pantalla de inicio**. Saldrá con el nombre Ahora y su icono.
3. Ábrela siempre desde el icono: así va a pantalla completa y sin barras.

## Datos y copias

Los datos viven en el móvil, dentro de la app instalada (no se comparten con Safari ni con otros dispositivos). En **Gym → Ajustes** tienes **Exportar copia** e **Importar copia**: guarda una de vez en cuando en Archivos o iCloud.

## Actualizar

Cambia `index.html`, sube `VERSION` en `sw.js` (por ejemplo `ahora-v2`) y haz commit. La app cogerá la versión nueva la próxima vez que la abras con conexión.
