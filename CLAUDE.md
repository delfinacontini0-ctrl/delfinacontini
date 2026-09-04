# Portfolio — Delfina Contini

## Stack
- HTML, CSS y JavaScript puro (vanilla). SIN frameworks (no React, no Vue, no Tailwind, no build tools).
- Sitio estático: cada página es un archivo .html que se abre directo en el navegador.

## Estructura de archivos
- `index.html` — home (página principal).
- `styles.css` — estilos compartidos por TODAS las páginas (incluye las @font-face, el cursor personalizado y el menú mobile).
- Páginas adicionales: `projects.html`, `about.html`, `contact.html` (a crear).

## Reglas de estilo (importantes)
- Las fuentes (Switzer y DM Mono) están embebidas en base64 dentro de styles.css. NO duplicarlas en cada página: van una sola vez en styles.css y todas las páginas lo enlazan con `<link rel="stylesheet" href="styles.css">`.
- Estética: minimalista, blanco y negro. Tipografía DM Mono para textos, Switzer para el nombre/títulos.
- Las proporciones y tamaños se ajustan vía las variables de `:root` (ej. `--pad`) y las funciones `clamp()` repartidas en el CSS. Cuando haya que cambiar tamaños o espaciados, tocar ahí.
- Mantener las animaciones existentes (firma animada, reveal de entrada, hover del cursor) y el comportamiento del menú mobile.

## Convenciones
- Toda página nueva reutiliza el mismo header (nav), el cursor personalizado y el menú mobile que el index.
- No cambiar colores, fuentes ni animaciones sin que se pida explícitamente.
- Mantener el HTML semántico y accesible (aria-labels como ya están en el index).