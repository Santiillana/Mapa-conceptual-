# TIC Explorer

**Mapa conceptual interactivo sobre las Tecnologías de la Información y la Comunicación (TIC).**

## Abrir la aplicación

La página principal está en `index.html`. Puedes abrirla directamente en un navegador o publicarla con GitHub Pages.

- [Abrir el código de la aplicación](./index.html)
- [Ver el repositorio](https://github.com/Santiillana/Mapa-conceptual-)

## Qué incluye

- Tres ramas principales: equipos y herramientas TIC, tipos de software y servicios de Internet.
- Relaciones entre conceptos con palabras de enlace.
- Selección de conceptos para leer sus definiciones y ejemplos.
- Recorrido guiado con pasos anterior/siguiente y barra de progreso.
- Controles de zoom, vista general y reinicio de la vista.
- Diseño adaptable a escritorio y móvil, controles accesibles por teclado y respeto por la preferencia de movimiento reducido.
- Hoja de impresión apaisada con campos para nombre, curso y fecha; el botón «Guardar como PDF» abre el diálogo de impresión del navegador.
- Atribución tecnológica visible: HTML, CSS y JavaScript.

## Criterios conceptuales

El mapa diferencia hardware, software y servicios de Internet. El software se organiza por función (sistema, aplicación y programación), mientras que las licencias se muestran como una dimensión transversal e independiente de esa clasificación. **Software libre no significa necesariamente software gratuito**: la libertad de usar, estudiar, modificar o redistribuir no es lo mismo que el precio.

## Personalización para principiantes

El contenido está en el arreglo `nodes` del bloque JavaScript dentro de `index.html`. Cada concepto incluye identificador, título, categoría, definición, ejemplos y coordenadas. Las relaciones se mantienen en `links` y el orden del recorrido en `guidedOrder`. Los colores, el diseño adaptable y la impresión se configuran en el bloque `style`.

Al añadir un nodo, asígnale un identificador único y asegúrate de que las relaciones y el recorrido guiado usen ese mismo identificador.

## Publicar con GitHub Pages

1. En el repositorio, abre **Settings → Pages**.
2. En **Build and deployment**, selecciona **Deploy from a branch**.
3. Elige la rama `main` y la carpeta `/ (root)`; guarda los cambios.
4. Espera a que GitHub Pages termine el despliegue y usa la URL que muestre esa misma sección.

## Estado de verificación

Se verificó que el archivo `index.html` y este README están en la rama `main`. La revisión funcional en navegador, la impresión real y la publicación de GitHub Pages todavía deben comprobarse en el entorno final. No se declaran esas pruebas como aprobadas hasta ejecutarlas.

## Tecnología y atribución

Proyecto educativo hecho con HTML, CSS y JavaScript sin dependencias externas ni servicios de terceros.
