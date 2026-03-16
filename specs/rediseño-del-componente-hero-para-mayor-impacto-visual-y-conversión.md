# Rediseño del Componente Hero para Mayor Impacto Visual y Conversión

## Objetivo
Rediseñar el componente Hero principal de la página de inicio para aumentar su impacto visual, comunicar autoridad y especialización técnica de manera clara, y mejorar las tasas de conversión mediante una jerarquía visual mejorada y llamados a la acción (CTAs) más efectivos.

## Alcance
- Modificación del archivo del componente Hero principal (ej: `components/Hero.jsx`, `sections/HeroSection.vue`).
- Actualización del texto del subtítulo según la nueva copy proporcionada.
- Implementación de dos CTAs principales con estilos diferenciados.
- Integración de un nuevo elemento visual (foto profesional o avatar minimalista).
- Implementación de un fondo sutil (gradiente o textura) para añadir profundidad.
- Refactorización de los estilos CSS/Tailwind para mejorar contraste, jerarquía tipográfica y espaciado.

## Fuera de alcance
- Cambios en la navegación principal o el footer del sitio.
- Rediseño de otras secciones de la página de inicio.
- Implementación de funcionalidades complejas para los CTAs (ej: calendario embebido). Los enlaces pueden ser estáticos por ahora.
- Optimización de imágenes para rendimiento (se asume que la imagen proporcionada ya está optimizada).
- Cambios en la estrategia de SEO o metaetiquetas.
- Adaptaciones responsivas extremas más allá de las estándar (se mantendrá la responsividad actual).

## Archivos impactados
- El archivo principal del componente Hero (ej: `src/components/Hero.vue`, `app/components/Hero.tsx`).
- El archivo de estilos asociado al Hero (ej: `src/components/Hero.module.css`, estilos en `tailwind.config.js` si se añaden colores personalizados).
- El archivo de assets/imágenes para la nueva foto/avatar (ej: `public/images/avatar-profesional.jpg`).
- Posible actualización en un archivo de constantes para los textos (ej: `src/data/copy.js`).

## Subtareas
- Analizar el código actual del componente Hero y su estructura de estilos.
- Crear una copia de seguridad del estado actual del componente.
- Reescribir el texto del subtítulo con la nueva copy: 'Especialista en construir plataformas SaaS escalables, seguras y listas para producción.'.
- Diseñar e implementar el contenedor para los dos CTAs ('Ver proyectos' y 'Agendar reunión') con estilos visualmente diferenciados (primario/secundario).
- Integrar la nueva imagen (foto/avatar) en el layout, asegurando una visualización correcta en todos los breakpoints.
- Implementar el fondo sutil (definir y aplicar gradiente lineal o textura SVG sutil).
- Refactorizar la jerarquía tipográfica: Aumentar tamaño/peso del título, ajustar contraste de colores entre texto y fondo, mejorar el espaciado (padding/margin).
- Realizar pruebas de visualización en diferentes viewports (móvil, tablet, escritorio).
- Realizar una revisión de contraste de colores (WCAG) para asegurar accesibilidad.
- Solicitar revisión de diseño y merge a la rama principal.

## Criterios de aceptación
- El subtítulo muestra exactamente el texto: 'Especialista en construir plataformas SaaS escalables, seguras y listas para producción.'.
- Se visualizan dos botones/CTAs claramente diferenciados con los textos 'Ver proyectos' y 'Agendar reunión'.
- La nueva imagen (foto o avatar) se muestra correctamente, es proporcional y de alta calidad.
- El fondo tiene un gradiente o textura sutil que no interfiere con la legibilidad del texto.
- Existe un claro contraste visual entre el título, subtítulo y el cuerpo, con una jerarquía tipográfica evidente.
- El componente es totalmente responsivo y se visualiza correctamente en dispositivos móviles, tabletas y escritorio.
- Los enlaces de los CTAs son funcionales (pueden apuntar a un placeholder por el momento).
- El código cumple con los estándares de calidad y no introduce errores en la consola.

## Riesgos
- La nueva imagen podría no estar optimizada para web, afectando el performance de carga.
- Los colores del gradiente de fondo podrían no tener suficiente contraste con el texto, afectando la accesibilidad.
- La adición de nuevos elementos podría romper el layout en algunos breakpoints no probados.
- Los estilos de los nuevos CTAs podrían no estar alineados con el sistema de diseño existente.
- El tiempo de implementación podría extenderse si la integración de la imagen y el fondo requiere ajustes complejos de CSS.
