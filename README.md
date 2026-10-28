# TIC Explorer

Mapa conceptual interactivo educativo sobre las Tecnologías de la Información y la Comunicación (TIC).

## Abrir y desplegar

La aplicación no requiere dependencias, compilación ni backend. Abre `index.html` en un navegador moderno para probarla localmente.

**Despliegue recomendado en Netlify:**
1. Entra en Netlify y elige **Add new site → Import an existing project**.
2. Conecta GitHub y selecciona `Santiillana/Mapa-conceptual-`.
3. Selecciona la rama `main`.
4. Usa la configuración de `netlify.toml`: directorio de publicación `.` (raíz) y sin comando de build.
5. Pulsa **Deploy site**. Netlify te dará la URL del sitio; ábrela y comprueba los pasos de la lista de pruebas.

También puedes desplegar manualmente arrastrando a Netlify la carpeta que contiene `index.html`.

## Qué incluye

- Tres ramas: equipos y herramientas TIC, tipos de software y servicios de Internet.
- Conceptos seleccionables con definiciones y ejemplos.
- Relaciones explícitas con palabras de enlace.
- Recorrido guiado con anterior/siguiente y progreso.
- Vista general, zoom y reinicio.
- Adaptación a pantallas pequeñas, foco visible, navegación por teclado y respeto por la preferencia de movimiento reducido.
- Impresión apaisada con campos para nombre, curso y fecha; «Guardar como PDF» abre el diálogo de impresión del navegador.
- Atribución tecnológica visible: HTML, CSS y JavaScript.

## Criterios conceptuales

El mapa diferencia hardware, software y servicios de Internet. El software se clasifica por función en sistema, aplicación y programación. Las licencias aparecen como una dimensión transversal, independiente de la función. **Software libre no significa necesariamente gratuito**: las libertades de uso, estudio, modificación y redistribución son distintas del precio.

## Personalizar

Consulta [la guía para principiantes](docs/beginner-guide.md). El modelo de conceptos se encuentra en el arreglo `nodes` del JavaScript dentro de `index.html`; las relaciones están en `links` y el orden del recorrido en `guidedOrder`.

## Verificación y limitaciones

La integridad del contenido se documenta en [la validación conceptual](docs/content-validation.md). Antes de declarar el sitio listo, completa [la lista de pruebas](docs/testing-checklist.md), especialmente la comprobación visual en el navegador, los controles de teclado, el diseño móvil y la impresión real. No se declara verificada la publicación de Netlify hasta que se abra y revise la URL generada.

## Tecnología y privacidad

Proyecto estático con HTML, CSS y JavaScript, sin dependencias externas, analítica, formularios, cuentas ni envío de datos personales a un servidor. Netlify aloja los archivos estáticos cuando se despliega el sitio.
