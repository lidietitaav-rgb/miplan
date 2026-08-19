# Mi Plan — Entreno y Nutrición

PWA personal de entrenamiento y nutrición. Funciona sin conexión y se instala
en el móvil desde el navegador.

## Qué incluye

- **Hoy** — qué toca hoy y checklist diario
- **Entreno** — rutinas, planificador semanal, sesión en vivo serie a serie con
  cronómetro y temporizador de descanso, editor de rutinas y ejercicios con foto
- **Nutrición** — menú semanal, contador de raciones y recetas. El reparto de
  hidratos se recalcula según los días de entreno planificados
- **Progreso** — rachas, sesiones por semana, peso, cintura y récords

## Archivos

| Archivo | Para qué sirve |
|---|---|
| `index.html` | La app entera: estilos, lógica e imágenes |
| `manifest.json` | Nombre, iconos y colores al instalarla |
| `sw.js` | Service worker: hace que funcione sin conexión |
| `icon-192.png` / `icon-512.png` | Iconos de la app instalada |
| `.nojekyll` | Evita que GitHub Pages procese la carpeta |

## Publicar

Repositorio público → Settings → Pages → Source: `main`, carpeta `/ (root)`.

Queda en `https://USUARIO.github.io/REPO/`

## Al actualizar

Cambia la versión de la caché en la primera línea de `sw.js`
(`miplan-v2` → `miplan-v3`) para que los navegadores instalados
recojan la versión nueva.

## Datos

Todo se guarda en el `localStorage` del navegador. No hay servidor ni cuentas.
Haz copias desde Progreso → Descargar copia.
