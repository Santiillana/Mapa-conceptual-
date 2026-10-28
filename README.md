# TIC Explorer

Mapa conceptual interactivo sobre las Tecnologías de la Información y la Comunicación (TIC). Está construido con HTML, CSS y JavaScript nativos; no requiere dependencias ni compilación.

## Abrir localmente

1. Descarga o clona este repositorio.
2. Abre el archivo index.html en un navegador moderno.
3. Selecciona nodos para ver su ficha contextual.
4. Usa Vista general, Recorrido guiado, Auto, zoom y Centrar mapa.
5. Usa Exportar PDF para abrir el diálogo de impresión y elegir Guardar como PDF.

## Desplegar en Netlify

1. Entra en Netlify y elige Add new site → Import an existing project.
2. Conecta GitHub y selecciona Santiillana/Mapa-conceptual-.
3. Selecciona la rama main.
4. Deja vacío el comando de compilación y usa el directorio de publicación . (raíz); la configuración está en netlify.toml.
5. Pulsa Deploy site y abre la URL publicada para ejecutar las pruebas.

El despliegue no se considera validado hasta que la URL pública se abra y se pruebe en un navegador.

## Funcionalidades

- Tres ramas cromáticas: hardware (cian), software (violeta) y servicios de Internet (naranja).
- Nodos seleccionables, palabras de enlace, relaciones resaltadas y encuadre del concepto activo.
- Fichas contextuales con definición, utilidad, ejemplo, criterios, relación y diagrama esquemático.
- Recorrido educativo con progreso, anterior/siguiente y reproducción automática pausables.
- Zoom, restablecimiento de vista y navegación por teclado.
- Diseño adaptable, foco visible y respeto por prefers-reduced-motion.
- Impresión horizontal con mapa, ficha seleccionada y campos personales; los controles se ocultan al imprimir.

## Estructura

- index.html: interfaz, estilos, datos, dibujo SVG e interacciones.
- netlify.toml: configuración de publicación estática y cabeceras.
- docs/beginner-guide.md: guía de edición y ejecución.
- docs/content-validation.md: revisión conceptual.
- docs/testing-checklist.md: criterios de prueba y estado conocido.

## Editar conceptos

En index.html, el arreglo nodes contiene los conceptos y las fichas. El arreglo links define las conexiones y sus palabras de enlace; guidedOrder define el recorrido pedagógico. Mantén identificadores únicos y comprueba que cada relación apunte a conceptos existentes.

Los diagramas de las fichas son esquemáticos, no mediciones científicas ni fuentes externas. Revisa el contenido con la especificación maestra y, cuando corresponda, con el docente.

## Pruebas y limitaciones

Se verificó que los archivos principales y la configuración están presentes en el repositorio. La implementación se actualizó, pero las pruebas funcionales en navegador, móvil y la URL de Netlify deben ejecutarse antes de declarar el proyecto validado. Consulta docs/testing-checklist.md y registra los resultados reales.

## Tecnologías y atribución

HTML, CSS, JavaScript y SVG nativos. No se utilizan bibliotecas de terceros ni se atribuyen las ilustraciones esquemáticas a fuentes externas.