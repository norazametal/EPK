# NO RAZA · EPK oficial

Sitio estático (HTML, sin build) con el EPK de la banda y el rider técnico.

| Ruta | Qué es |
|---|---|
| `/` | EPK: bio, Tyrona, prensa, discografía, videos, festivales y giras, line-up, endorsements, booking |
| `/rider/` | Rider técnico en versión web |
| `/rider/pdf/` | Rider imprimible (5 páginas carta). Botón **Save as PDF / Print** para bajarlo en PDF |
| `assets/` | Fotos, portadas, logos y el video del hero (versiones optimizadas para web) |

Las fotos y logos en alta resolución **no** van en el repo: el botón "Hi-res photos & logos" del EPK abre la carpeta de Drive **NO RAZA – Press Kit**.

## Subir a GitHub

**Opción fácil (desde el navegador):**
1. En github.com → **New repository** → nombre `no-raza-epk` → Create.
2. En el repo vacío: **uploading an existing file** → arrastra **todo el contenido** de esta carpeta (no la carpeta, lo que hay dentro: `index.html`, `rider/`, `assets/`, `vercel.json`…).
3. **Commit changes**.

**Opción con terminal:**
```bash
cd no-raza-epk
git init
git add .
git commit -m "EPK NO RAZA"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/no-raza-epk.git
git push -u origin main
```

## Publicar en Vercel

1. vercel.com → **Add New… → Project** → importa el repo `no-raza-epk`.
2. Framework Preset: **Other**. Build Command: vacío. Output Directory: vacío (la raíz).
3. **Deploy**. Cada vez que subas cambios a GitHub, Vercel publica solo.
4. Dominio propio: Project → **Settings → Domains** → agrega `noraza.net` y sigue las instrucciones de DNS.

## Notas

- En celular la página se ve como la de escritorio, escalada al ancho de la pantalla.
- Las fuentes (Cinzel, Barlow, Barlow Condensed) cargan desde Google Fonts.
- El video del hero pesa ~8.5 MB y va en silencio y en loop.
- Para cambiar textos, edita `index.html`, o pide que lo regeneren desde el diseño del EPK.
