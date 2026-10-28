# Guía para principiantes

## 1. ¿Qué archivos son importantes?

- `index.html`: página principal y código de la aplicación.
- `README.md`: descripción y pasos de publicación.
- `netlify.toml`: configuración para que Netlify publique la carpeta raíz.
- `docs/content-validation.md`: comprobación de la estructura conceptual.
- `docs/testing-checklist.md`: pruebas que deben hacerse antes de considerar final el sitio.

## 2. Editar el contenido

Abre `index.html` con un editor de texto o de código. Dentro del bloque JavaScript encontrarás tres estructuras:

- `nodes`: define cada concepto, su título, categoría, explicación, ejemplos y posición.
- `links`: relaciona dos identificadores y escribe una palabra o frase de enlace.
- `guidedOrder`: define el orden del recorrido guiado.

Cada `id` debe ser único. Si agregas un concepto, añade sus relaciones y decide en qué punto debe aparecer en el recorrido.

## 3. Editar colores y diseño

Los colores principales están al principio del bloque CSS como variables: `--blue`, `--green`, `--violet` y `--ink`. Las reglas al final del CSS controlan el diseño móvil, la preferencia de movimiento reducido y la impresión.

## 4. Probar localmente

Abre `index.html` en un navegador moderno. Revisa que puedas seleccionar cada concepto, recorrer todos los pasos, cambiar el zoom y abrir el diálogo de impresión. Para una prueba más parecida a un sitio publicado, puedes iniciar un servidor estático desde esta carpeta con:

```bash
python3 -m http.server 8000
```

Después visita `http://localhost:8000`.

## 5. Publicar con Netlify

La forma más sencilla es conectar el repositorio GitHub en Netlify y desplegar la rama `main`. La configuración incluida publica la raíz del repositorio; no hace falta ejecutar una compilación ni instalar paquetes.

También puedes usar el método manual: en Netlify, elige la opción de desplegar manualmente y arrastra la carpeta del proyecto que contiene `index.html` y `netlify.toml`. Si haces cambios después, vuelve a desplegar la carpeta o sube los cambios a GitHub para activar un nuevo despliegue conectado.

## 6. Guardar como PDF

Usa el botón «Guardar como PDF». Se abrirá el diálogo de impresión del navegador. Selecciona «Guardar como PDF» y orientación horizontal. La vista de impresión oculta los controles interactivos y añade campos para nombre, curso y fecha. La composición exacta depende del navegador y sus márgenes de impresión.

## 7. Limitaciones conocidas

La aplicación es estática: no guarda progreso entre sesiones, no requiere cuenta y no envía datos a un servidor. El mapa se representa en SVG y los textos del modelo son editables. Antes de entregar, sigue la lista de pruebas y verifica el resultado desplegado en escritorio y móvil.
