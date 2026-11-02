# Bubbles Studio

A phone app (installable web app) for making vertical promo videos scene by scene. One version for **iPhone and Android**.

## What's inside

- `index.html`, `manifest.webmanifest`, `sw.js`, `icons/`: the app
- `music/`: four calm music loops (Calma, Brisa, Agua, Jardín) that repeat without a seam
- `tts/` + `voices/`: the automatic voice (Piper "Claude", female, Mexican Spanish, Apache-2.0, free for commercial use). The 63 MB voice model is split into 14 MB pieces so every file fits GitHub's 25 MB browser-upload limit; the app joins them itself.

About 112 MB in total. The phone only downloads the voice (about 92 MB) the first time she uses "Voz automática". Nothing private is uploaded: photos, videos, recordings and projects stay on her phone.

## 1. Put it online (GitHub Pages, free)

1. Create a new **public** repository, e.g. `bubbles-studio`.
2. **Add file → Upload files**: drag in everything from *inside* this folder (`index.html`, `manifest.webmanifest`, `sw.js`, `LEEME.md` and the folders `icons`, `music`, `tts`, `voices`). Files must sit at the top of the repo, not inside a `bubbles-studio-app` folder. Commit.
3. **Settings → Pages → Deploy from a branch → `main` / `(root)` → Save.**
4. After a minute or two: `https://<your-username>.github.io/bubbles-studio/`.

**Updates:** upload the new files to the same repo and commit (Upload files replaces files with the same name). Don't rename the repo; that changes the address.
Every build has its own version number (shown in Ajustes → Aplicación, e.g. `2026.11.02-1816`). When the app opens with internet it compares itself with the copy on GitHub; if yours is newer she sees **"Hay una versión nueva · Actualizar ahora"** on the home screen, and Ajustes → Aplicación has a **Buscar actualización** button. Updating keeps her projects, videos and the downloaded voice.
If you ever edit `index.html` yourself, change the `APP_VERSION` line (e.g. add `-b`) so phones notice the update.

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
- **Voz en off (opcional), tres formas en cada escena:**
  - **Grabar:** el texto de la escena aparece grande para leerlo; toca **Listo** al terminar.
  - **Subir audio:** por ejemplo una nota de voz.
  - **Voz automática:** voz femenina en español de México. Escribe lo que dirá, elige la velocidad y toca **Crear voz**. La primera vez se descargan unos 92 MB (usa Wi-Fi); después funciona sin internet.
  - Si la voz dura más que la escena, la escena se alarga sola.
- **Música:** Escenas → Música de fondo → **Elegir**: cuatro piezas tranquilas que se repiten sin cortes, o sube tu canción. La música baja sola mientras hablas.
- **Diseño:** texto encima, caja flotante o pantalla dividida; arrastra en la vista previa para moverlo.
- **Exportar → Crear video.** Mantén la pantalla encendida mientras se crea.
- **Guardar:** en iPhone, **Guardar o compartir** → **Guardar video** (queda en Fotos). En Android, **Guardar en el teléfono** (queda en Descargas y en la galería) o **Compartir** a WhatsApp o Instagram.

## Good to know

- **The first time she records, the phone asks for microphone permission.** If she says no by accident: iPhone Settings → Safari → Microphone; Android: long-press the app icon → App info → Permissions.
- **Automatic voice:** Ajustes → Voz automática has the default speed, a "Probar la voz" button and "Borrar voz descargada" to free the 92 MB.
- **Always use the icon.** The installed app and a browser tab keep separate storage.
- **Projects live only on her phone.** Uninstalling the app or clearing browser data deletes them; finished videos should be saved to the gallery.
- **Making a video plays it once in real time** (a 40-second video takes about 40 seconds).
