# QR Dinámicos en GitHub Pages

## Publicar en GitHub Pages
1. Crea un repo (por ej. `qr-dinamico`) y sube estos archivos.
2. En **Settings → Pages**: Source = `Deploy from branch`, Branch `main`, Folder `/root`.
3. Tu sitio quedará en `https://TU_USUARIO.github.io/qr-dinamico/`.

## Cómo generar tus QRs
- Abre `https://TU_USUARIO.github.io/qr-dinamico/generator.html`.
- Elige **k=android** para el QR de Android (temporal → luego Play) o **k=ios** para iOS.
- Ajusta color, logo y título, y pulsa **Generar → Descargar PNG**.
- Ese PNG ya es tu QR “permanente” porque apunta a `redirect.html?k=...`.

## Cómo cambiar destinos sin cambiar el QR
- Edita `target.json` en GitHub:
  - `android`: URL de Play (o temporal hasta publicar)
  - `ios`: URL de App Store
  - `web`/`default`: lo que prefieras
- Guarda (*Commit changes*). ¡Listo!
