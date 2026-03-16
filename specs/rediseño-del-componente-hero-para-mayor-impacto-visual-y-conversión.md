# Rediseño del Componente Hero para Mayor Impacto Visual y Conversión

## Objetivo
Rediseñar el componente Hero principal de la página de inicio para aumentar su impacto visual, comunicar autoridad y especialización técnica de manera clara, y mejorar las tasas de conversión mediante una jerarquía visual mejorada y llamados a la acción (CTAs) más efectivos.

## Alcance
- Reescritura del texto del subtítulo en el componente Hero.
- Implementación de un doble CTA ('Ver proyectos', 'Agendar reunión') con estilos claros y diferenciados.
- Integración de un elemento visual (foto profesional o avatar minimalista) alineado con la marca.
- Diseño e implementación de un fondo sutil (gradiente o textura) para añadir profundidad visual.
- Refactorización de los estilos CSS para mejorar el contraste, la jerarquía tipográfica y el espaciado.
- Asegurar que el componente sea totalmente responsivo en todos los viewports.

## Fuera de alcance
- Cambios en el sistema de diseño (design tokens, componentes base) fuera del componente Hero.
- Modificaciones en la navegación principal (header) o el pie de página (footer).
- Integración con sistemas de calendario para el CTA 'Agendar reunión' (solo se implementará el enlace estático).
- Optimización de imágenes o assets fuera del elemento visual principal del Hero.
- Cambios en el contenido o estructura de otras secciones de la página.

## Archivos impactados
- src/components/Hero/Hero.jsx (o .tsx)
- src/components/Hero/Hero.module.css (o .scss/.styled.js)
- src/assets/images/ (para añadir la nueva foto/avatar y fondo)
- src/pages/index.jsx (o la página principal que contiene el Hero)

## Subtareas
- 1. Analizar y documentar la estructura HTML/CSS actual del componente Hero.
- 2. Reescribir el subtítulo en el archivo del componente con el texto: 'Especialista en construir plataformas SaaS escalables, seguras y listas para producción.'.
- 3. Diseñar y generar los assets visuales: foto/avatar y patrón/gradiente de fondo (en coordinación con diseño).
- 4. Implementar la nueva estructura con doble CTA, imagen y fondo en el archivo del componente.
- 5. Refactorizar los estilos CSS: aumentar tamaño/weight del título, ajustar contraste de colores, mejorar espaciado (padding/margin).
- 6. Asegurar la correcta visualización y alineación de los nuevos elementos en versión escritorio y móvil.
- 7. Realizar pruebas de usabilidad y contraste (WCAG) en los nuevos textos y botones.
- 8. Realizar prueba de integración para verificar que no se hayan roto funcionalidades existentes.

## Criterios de aceptación
- El subtítulo muestra exactamente el texto: 'Especialista en construir plataformas SaaS escalables, seguras y listas para producción.'.
- Se muestran dos botones CTAs primarios con los textos 'Ver proyectos' y 'Agendar reunión', con estilos diferenciados y visualmente prominentes.
- La foto profesional o avatar minimalista es visible, de alta calidad y correctamente alineada con el texto.
- El fondo sutil (gradiente o textura) es visible, no interfiere con la legibilidad y añade profundidad al diseño.
- Existe un claro contraste visual entre el título, subtítulo y cuerpo, cumpliendo con estándares WCAG 2.1 AA.
- El diseño es consistente y funcional en los viewports más comunes (mobile, tablet, desktop).
- Los botones CTAs son completamente clickeables y enlazan a las páginas correctas (/proyectos y /contacto).
- El tiempo de carga del componente no se ve afectado significativamente (optimización de imágenes).

## Riesgos
- La nueva foto/avatar puede no alinearse con la percepción de marca deseada; requiere aprobación de diseño.
- El gradiente o textura de fondo puede afectar la legibilidad en algunos monitores o modos de visualización.
- Los cambios tipográficos podrían desalinear el balance visual con otras secciones de la página.
- Añadir múltiples CTAs podría diluir la tasa de conversión si no están jerarquizados correctamente.
- Posible incremento en el tamaño del bundle por la adición de nuevas imágenes/assets.
