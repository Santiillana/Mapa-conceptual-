# Guía para principiantes

## 1. Ejecutar el proyecto

1. Descarga el repositorio o abre su página en GitHub.
2. Abre index.html en Firefox, Chrome, Edge u otro navegador moderno.
3. No se necesita Node.js, instalar paquetes ni compilar.
4. Si el navegador bloquea alguna función al abrir un archivo local, sirve la carpeta con cualquier servidor estático sencillo; la aplicación no requiere backend.

## 2. Explorar el mapa

- Vista general muestra el mapa completo.
- Seleccionar un nodo actualiza la ficha y resalta las conexiones directas.
- Recorrido guiado presenta los conceptos en orden pedagógico.
- Auto avanza periódicamente; el botón cambia a Pausar y detiene el temporizador al volver a pulsarlo.
- Zoom + / − modifica el encuadre; Centrar mapa restablece la vista general.
- Exportar PDF abre el diálogo de impresión del navegador.

## 3. Editar el contenido

En index.html, busca const nodes. Cada objeto define identificador, título, categoría, tipo visual, posición, dimensiones, definición, utilidad, ejemplo, criterios, relaciones, ejemplos y diagrama.

Busca const links para editar conexiones. Cada enlace contiene identificador de origen, identificador de destino, palabra de enlace y color. Los identificadores deben coincidir exactamente con los de nodes.

Busca const guidedOrder para modificar el recorrido. Usa identificadores existentes. Si agregas nodos, actualiza también las relaciones y el orden del recorrido.

Los conceptos se dibujan en un lienzo SVG de 1400 × 760 unidades. x e y indican el centro del nodo; w y h, sus dimensiones. Mantén los nodos dentro del lienzo y comprueba que las etiquetas no se superpongan.

## 4. Comprender el código

- HTML organiza página, controles, mapa y ficha.
- CSS define paleta, distribución, estados visuales, adaptación e impresión.
- JavaScript administra datos, dibuja nodos y relaciones, cambia la selección y coordina el recorrido.
- SVG representa conexiones y nodos como elementos vectoriales interactivos.

Los diagramas de las fichas son esquemáticos: resumen una secuencia didáctica, no ejecutan una simulación física.

## 5. Publicar en Netlify

Importa Santiillana/Mapa-conceptual- desde GitHub. Usa main, deja vacío el comando de compilación y publica el directorio raíz. Después abre la URL pública, recorre la lista de pruebas y registra los problemas observados.

## 6. Exportar e imprimir

Selecciona Exportar PDF y elige guardar como PDF en orientación horizontal. Los controles se ocultan al imprimir. Los campos para nombre, curso y fecha aparecen en la esquina inferior derecha.

El resultado depende del motor de impresión y del tamaño de papel. Revisa el PDF final para comprobar que las etiquetas sean legibles y que el mapa no se recorte.