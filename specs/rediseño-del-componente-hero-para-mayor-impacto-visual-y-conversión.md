# Rediseño del Componente Hero para Mayor Impacto Visual y Conversión

## Objetivo
Rediseñar el componente Hero principal para aumentar su impacto visual, comunicar autoridad y especialización técnica de manera clara, y mejorar las tasas de conversión mediante una jerarquía visual mejorada y llamados a la acción (CTAs) más efectivos.

## Alcance
- Reescritura del texto del subtítulo según la nueva copia proporcionada.
- Implementación de un diseño con doble CTA ("Ver proyectos" y "Agendar reunión").
- Integración de un nuevo elemento visual (foto profesional o avatar minimalista).
- Aplicación de un fondo sutil (gradiente o textura) para mayor profundidad visual.
- Refactorización de los estilos CSS para mejorar el contraste, la jerarquía tipográfica y el espaciado.
- Asegurar que el componente sea completamente responsivo.

## Fuera de alcance
- Cambios en la estructura de navegación principal del sitio.
- Modificaciones en el contenido o diseño de otras secciones de la página.
- Implementación de funcionalidad backend para el CTA "Agendar reunión" (solo se implementará el enlace estático).
- Optimización de imágenes o assets fuera del componente Hero.
- Pruebas A/B o integración con herramientas de analítica (solo implementación visual).

## Archivos impactados
- src/components/Hero/Hero.jsx (o .tsx)
- src/components/Hero/Hero.module.css (o .scss/.styled.js)
- src/assets/images/ (para añadir la nueva foto/avatar)
- public/ (si la imagen se sirve estáticamente)

## Subtareas
- Analizar y copiar los assets de imagen (foto/avatar) a la carpeta correspondiente del proyecto.
- Actualizar el archivo del componente Hero (JSX/TSX) para incluir la nueva estructura con la imagen y los dos botones de CTA.
- Reescribir el texto del subtítulo con la nueva copia: "Especialista en construir plataformas SaaS escalables, seguras y listas para producción.".
- Refactorizar el archivo de estilos (CSS/SCSS) para implementar el fondo sutil (gradiente/textura), mejorar el contraste de color y la jerarquía tipográfica (tamaños, pesos, espaciado).
- Aplicar estilos específicos para los nuevos botones de CTA, asegurando un diseño claro y atractivo.
- Ajustar el layout para integrar la foto/avatar de forma responsiva (ej., en desktop a la derecha del texto, en móvil arriba o abajo).
- Realizar pruebas de visualización en diferentes viewports (mobile, tablet, desktop).
- Realizar una revisión de accesibilidad (contraste de colores, etiquetas ARIA, orden de tabulación).

## Criterios de aceptación
- El subtítulo muestra exactamente el texto: "Especialista en construir plataformas SaaS escalables, seguras y listas para producción.".
- Se muestran dos botones o enlaces de CTA claramente visibles y con los textos "Ver proyectos" y "Agendar reunión".
- La foto profesional o avatar minimalista es visible, de alta calidad y bien integrada en el diseño.
- El componente tiene un fondo sutil (gradiente o textura) que no interfiere con la legibilidad del texto.
- Existe un claro contraste visual entre el título, subtítulo y el cuerpo del texto, logrado mediante tamaño, peso y color.
- El diseño es consistente y atractivo en las tres vistas principales (mobile, tablet, desktop).
- Los CTAs son los elementos más destacados visualmente después del título principal.
- El código cumple con los estándares de calidad del proyecto y no introduce errores en la consola.

## Riesgos
- La nueva imagen/avatar podría no ajustarse bien a todos los tamaños de pantalla, requiriendo ajustes de recorte (object-fit) o múltiples resoluciones.
- El gradiente o textura de fondo podría no renderizar de manera consistente en todos los navegadores.
- Los cambios en la jerarquía tipográfica podrían desalinearse con la guía de estilos global del sitio, requiriendo ajustes adicionales.
- Añadir un segundo CTA podría saturar visualmente el espacio en vista móvil si no se diseña cuidadosamente.
- El tiempo de carga podría incrementarse ligeramente debido a la nueva imagen de fondo y/o avatar.
