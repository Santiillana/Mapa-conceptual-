# Guía para principiantes

## Explorar el mapa

- **Vista general** devuelve el encuadre panorámico.
- **Seleccionar un concepto** abre su ficha y resalta sus relaciones.
- **Recorrido guiado** entra en modo inmersivo a pantalla completa.
- Dentro del recorrido, usa **← / →** o **↑ / ↓** para avanzar y retroceder.
- Pulsa **Esc** o **Salir del recorrido** para regresar a la vista general.
- **Exportar PDF** abre el diálogo de impresión del navegador.

En el recorrido, el mapa sigue visible: la cámara se acerca al concepto activo, se iluminan las conexiones pertinentes y la ficha explica el concepto y la palabra de enlace. Los diagramas de las fichas son esquemas educativos animados.

## Ejecutar localmente

Abre index.html en un navegador moderno. No requiere Node.js, instalar paquetes ni compilar. Si necesitas un servidor local, sirve la carpeta con cualquier servidor estático sencillo.

## Editar conceptos

En index.html busca const nodes para editar títulos, definiciones, utilidad, ejemplo, criterios, relación y etiquetas de los diagramas. Busca const links para cambiar origen, destino y palabra de enlace. Busca const guidedOrder para ajustar el orden pedagógico. Los identificadores deben coincidir entre los tres arreglos.

Al editar, conserva la distinción entre equipos físicos, software y servicios de Internet. El software de sistema, aplicación y programación se clasifica por función; la licencia es una dimensión distinta. Software libre no significa necesariamente gratuito.

## Publicar en Netlify

Importa Santiillana/Mapa-conceptual- desde GitHub. Selecciona main, deja vacío el comando de compilación y usa la raíz como directorio de publicación. Después prueba la URL pública y registra los resultados.

## Impresión

Pulsa Exportar PDF, elige guardar como PDF y orientación horizontal. Revisa el documento final para confirmar que el mapa y los campos personales sean legibles y no estén recortados.