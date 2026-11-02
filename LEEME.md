# Bubbles Studio

A phone app (installable web app) for making vertical promo videos scene by scene. One version for **iPhone and Android**.

## What's inside

- `index.html`, `manifest.webmanifest`, `sw.js`, `icons/`: the app
- `music/`: four calm music loops (Calma, Brisa, Agua, Jardín) that repeat without a seam

About 23 MB in total. Nothing private is uploaded: photos, videos, recordings and projects stay on her phone.

## 1. Put it online (Netlify, free)

1. Log in at https://app.netlify.com (an account is required, otherwise the site is deleted after an hour).
2. **First time:** Add new site → Deploy manually → drag this folder in. Then Site configuration → Change site name (e.g. `bubbles-studio` → `https://bubbles-studio.netlify.app`). Rename *before* she installs.
3. **Updates:** open the same site → Deploys → drag the new folder onto "Need to update your site?". Same address, her app updates itself.
4. If you change anything besides `index.html` (music, icons), bump `VERSION` in `sw.js` (e.g. `bubbles-studio-v4` → `v5`).

## 2. Instalar en el teléfono (para ella)

**iPhone**
1. Abre el enlace en **Safari**.
2. Toca **Compartir** (cuadro con flecha hacia arriba) → **Agregar a inicio** → **Agregar**.

**Android**
1. Abre el enlace en **Chrome**.
2. Toca **Instalar Bubbles Studio** en la pantalla de inicio de la app, o el menú **⋮** → **Instalar app** (o **Agregar a la pantalla principal**).

Después, ábrela **siempre desde el ícono**.

## Cómo se usa (para ella)

- **Escenas:** foto o video, título, subtítulo, texto y cuánto tiempo se ve.
- **Voz en off (opcional):** en cada escena toca **Grabar**; el texto de la escena aparece grande para leerlo. Toca **Listo** al terminar. También puedes **Subir audio** (por ejemplo una nota de voz). La app quita los silencios del inicio y del final, y si tu voz dura más que la escena, la escena se alarga sola.
- **Música:** Escenas → Música de fondo → **Elegir**: cuatro piezas tranquilas que se repiten sin cortes, o sube tu canción. La música baja sola mientras hablas.
- **Diseño:** texto encima, caja flotante o pantalla dividida; arrastra en la vista previa para moverlo.
- **Exportar → Crear video.** Mantén la pantalla encendida mientras se crea.
- **Guardar:** en iPhone, **Guardar o compartir** → **Guardar video** (queda en Fotos). En Android, **Guardar en el teléfono** (queda en Descargas y en la galería) o **Compartir** a WhatsApp o Instagram.

## Good to know

- **The first time she records, the phone asks for microphone permission.** If she says no by accident: iPhone Settings → Safari → Microphone; Android: long-press the app icon → App info → Permissions.
- **Always use the icon.** The installed app and a browser tab keep separate storage.
- **Projects live only on her phone.** Uninstalling the app or clearing browser data deletes them; finished videos should be saved to the gallery.
- **Making a video plays it once in real time** (a 40-second video takes about 40 seconds).
