# TIC Explorer

Mapa conceptual interactivo sobre las Tecnologías de la Información y la Comunicación (TIC), construido con HTML, CSS y JavaScript nativos.

## Abrir localmente

1. Descarga o clona este repositorio.
2. Abre index.html en un navegador moderno.
3. Selecciona un nodo para consultar su ficha y explorar sus conexiones.
4. Pulsa **Recorrido guiado** para entrar en el modo inmersivo a pantalla completa.
5. En el recorrido, usa **← / →** (también ↑ / ↓) para avanzar y retroceder. Pulsa **Esc** o **Salir del recorrido** para volver al mapa.
6. Usa **Vista general** para restablecer el mapa y **Exportar PDF** para imprimir o guardar como PDF.

## Cómo funciona el recorrido

El mapa conceptual permanece visible durante el recorrido. Cada paso selecciona un concepto, destaca sus conexiones, encuadra el nodo, actualiza la ficha y explica la palabra de enlace que lo conecta con el mapa. Las ilustraciones son diagramas educativos animados basados en el concepto; no son simulaciones físicas.

La navegación del recorrido es deliberadamente sencilla: flechas del teclado para cambiar de paso y Esc para salir. No hay puntos, cuestionarios ni gamificación.

## Desplegar en Netlify

1. En Netlify, elige Add new site → Import an existing project.
2. Conecta GitHub y selecciona Santiillana/Mapa-conceptual-.
3. Usa la rama main, sin comando de compilación, y directorio de publicación raíz (.).
4. Publica y prueba la URL pública con la lista de verificación.

## Estructura

- index.html: datos conceptuales, SVG, estilos e interacciones.
- netlify.toml: configuración de publicación estática.
- docs/beginner-guide.md: guía de edición y funcionamiento.
- docs/content-validation.md: validación conceptual.
- docs/testing-checklist.md: pruebas y estado de validación.

## Contenido y mantenimiento

Los arreglos nodes, links y guidedOrder dentro de index.html definen conceptos, relaciones y orden pedagógico. Conserva los identificadores y revisa cada palabra de enlace al modificar el mapa. La clasificación por función del software es independiente de sus licencias; software libre no significa necesariamente gratuito.

## Estado de las pruebas

Se comprobaron estáticamente los identificadores de los conceptos y los extremos de las relaciones en el repositorio. Las pruebas funcionales en navegador, dispositivos móviles, impresión y despliegue público deben registrarse en docs/testing-checklist.md antes de considerar el proyecto validado.

## Tecnologías y atribución

HTML, CSS, JavaScript y SVG nativos. Las ilustraciones son esquemas educativos propios del proyecto y no se presentan como fuentes académicas.