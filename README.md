# Transformador de imágenes estilo C64

Convierte imágenes a la **paleta de 16 colores del Commodore 64** (320×200), con **dithering**, **ajustes de brillo/contraste/saturación** y modos creativos (contorno “a pincel” y tramas B/N). Todo se ejecuta **localmente** en tu navegador (sin subir nada a servidores).

## Demo (GitHub Pages)
➡️ **https://chesvoc.github.io/transformador_imagenes_a_estilo_c64/**

> Si ves 404, espera unos segundos a que GitHub Pages despliegue y recarga con `Ctrl+F5`.

## Características
- Redimensionado a **320×200** con aspect ratio conservado.
- **Paleta C64 (Pepto) — 16 colores** + cuantización por distancia RGB.
- **Floyd–Steinberg Dithering** (activable/desactivable).
- Ajustes: **Brillo**, **Contraste**, **Saturación** con **Live Preview**.
- **Modo Outline**: detección simple del sujeto + contorno “a pincel” (grosor variable por sombras); re-cuantiza a 16 colores.
- **Modo B/N Tramas**: patrones de puntos/líneas/cross-hatch para sombreado a 320×200.
- **Download** siempre disponible (descarga el canvas actual como PNG).

## Uso
1. Abre la demo (enlace arriba) o abre `index.html` localmente (doble clic).  
2. **Selecciona una imagen** (JPG/PNG).  
3. Ajusta **Brillo/Contraste/Saturación**, Dithering y/o cambia de **modo**.  
4. Pulsa **Download** para guardar el resultado (PNG 320×200).

> Si pulsas acciones sin imagen cargada, se abrirá el selector de archivo automáticamente.

## Requisitos
- Navegador moderno (Chrome/Edge/Brave/Firefox).  
- No requiere internet una vez abierto el HTML (todo es local).

## Estructura
- Proyecto de **archivo único**: `index.html` (incluye CSS/JS inline).  
- Sin dependencias externas, ni CDNs, ni Web Workers.

## Desarrollo
- Para publicar en GitHub Pages:
  1) **Settings → Pages → Build and deployment**  
     Source: *Deploy from a branch* → Branch: `main` / Folder: `/ (root)` → Save  
  2) Asegúrate de que el archivo principal se llama **`index.html`** en la raíz.  
  3) (Opcional) añade un archivo vacío **`.nojekyll`** en la raíz.
- Para probar localmente: abre `index.html` en el navegador (doble clic).

## Licencia
Indica aquí la licencia que prefieras (p. ej. MIT).
