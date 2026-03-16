# Mockups del Nuevo Diseño Hero con Doble CTA y Fondo

## Objetivo
Crear mockups visuales que muestren el nuevo diseño del componente Hero con doble CTA, fondo mejorado y jerarquía visual optimizada.

## Diseño Conceptual

### 1. Layout General (Desktop)
```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│  [Fondo: Gradiente sutil azul/gris con textura geométrica] │
│                                                             │
│  ┌─────────────────────────────────────────────────────┐   │
│  │                                                     │   │
│  │  CONTENIDO PRINCIPAL (Izquierda - 60%)              │   │
│  │                                                     │   │
│  │  H1: Hola, soy Jhonatan Rojas                       │   │
│  │  Subtítulo: Desarrollador Full Stack...             │   │
│  │  Descripción: +5 años experiencia...                │   │
│  │                                                     │   │
│  │  ┌──────────────┐  ┌──────────────┐                │   │
│  │  │  Ver Proyectos │  │  Agendar Reunión │          │   │
│  │  └──────────────┘  └──────────────┘                │   │
│  │                                                     │   │
│  └─────────────────────────────────────────────────────┘   │
│                                                             │
│  ┌─────────────────────────────────────────────────────┐   │
│  │  IMAGEN PROFESIONAL (Derecha - 40%)                 │   │
│  │  [Foto profesional con fondo desenfocado]           │   │
│  │  [Sombra sutil y borde redondeado]                  │   │
│  └─────────────────────────────────────────────────────┘   │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

### 2. Esquema de Colores
- **Fondo principal**: Gradiente `#0f172a` → `#1e293b` con textura geométrica sutil
- **Color primario**: `#3b82f6` (Azul vibrante para acentos y CTAs)
- **Color secundario**: `#8b5cf6` (Púrpura para highlights)
- **Texto principal**: `#f8fafc` (Blanco muy claro)
- **Texto secundario**: `#cbd5e1` (Gris claro)
- **Botón primario**: `#3b82f6` con hover `#2563eb`
- **Botón secundario**: `transparent` con borde blanco, hover `rgba(255,255,255,0.1)`

### 3. Jerarquía Tipográfica
- **H1**: `4.5rem` (72px) - Peso 700 - Inter
- **Subtítulo**: `2rem` (32px) - Peso 600 - Inter
- **Descripción**: `1.125rem` (18px) - Peso 400 - Inter
- **Botones**: `1rem` (16px) - Peso 600 - Inter

### 4. Mockup Visual Desktop
```html
<!-- Estructura HTML/JSX propuesta -->
<section class="hero-section">
  <div class="hero-background">
    <!-- Gradiente + textura geométrica -->
  </div>
  
  <div class="hero-container">
    <div class="hero-content">
      <!-- Badge de especialización -->
      <div class="specialization-badge">
        <span>🚀 Full Stack Developer</span>
      </div>
      
      <!-- Título principal -->
      <h1 class="hero-title">
        Hola, soy <span class="highlight">Jhonatan Rojas</span>
      </h1>
      
      <!-- Subtítulo -->
      <h2 class="hero-subtitle">
        Desarrollador Full Stack especializado en <span class="accent">Laravel</span> y <span class="accent">Vue.js</span>
      </h2>
      
      <!-- Descripción -->
      <p class="hero-description">
        Con más de 5 años de experiencia creando soluciones SaaS escalables para el sector salud. 
        Combino expertise técnico con comprensión profunda de necesidades empresariales.
      </p>
      
      <!-- CTAs -->
      <div class="hero-ctas">
        <a href="#proyectos" class="btn-primary">
          <i class="fas fa-code"></i> Ver Proyectos
        </a>
        <a href="#contacto" class="btn-secondary">
          <i class="fas fa-calendar-check"></i> Agendar Reunión
        </a>
      </div>
      
      <!-- Indicadores de confianza -->
      <div class="trust-indicators">
        <div class="indicator">
          <span class="number">50+</span>
          <span class="label">Proyectos Completados</span>
        </div>
        <div class="indicator">
          <span class="number">5+</span>
          <span class="label">Años Experiencia</span>
        </div>
        <div class="indicator">
          <span class="number">100%</span>
          <span class="label">Satisfacción Clientes</span>
        </div>
      </div>
    </div>
    
    <div class="hero-image">
      <!-- Imagen profesional -->
      <div class="image-container">
        <img src="assets/img/professional-photo.jpg" alt="Jhonatan Rojas - Desarrollador Full Stack">
        <div class="image-decoration"></div>
      </div>
    </div>
  </div>
</section>
```

### 5. Mockup Visual Mobile
```
┌─────────────────────────────────────┐
│                                     │
│  [Fondo gradiente]                  │
│                                     │
│  ┌─────────────────────────────┐   │
│  │                             │   │
│  │  [Imagen profesional]       │   │
│  │  (Circular, centrada)       │   │
│  │                             │   │
│  └─────────────────────────────┘   │
│                                     │
│  H1: Hola, soy Jhonatan Rojas       │
│                                     │
│  Subtítulo: Desarrollador Full...   │
│                                     │
│  Descripción: +5 años...            │
│                                     │
│  ┌──────────────┐                   │
│  │ Ver Proyectos │                  │
│  └──────────────┘                   │
│                                     │
│  ┌──────────────┐                   │
│  │Agendar Reunión│                  │
│  └──────────────┘                   │
│                                     │
│  [Indicadores en fila horizontal]   │
│                                     │
└─────────────────────────────────────┘
```

### 6. Mockup Visual Tablet
- Layout similar a desktop pero con imagen más pequeña
- CTAs en fila horizontal
- Contenido e imagen en proporción 60/40
- Tipografía ligeramente reducida

### 7. Estados Interactivos
- **Hover botón primario**: Escala ligera (1.05) + sombra más intensa
- **Hover botón secundario**: Fondo blanco translúcido + cambio de color de texto
- **Focus estados**: Outline accesible con contraste adecuado
- **Active estados**: Efecto de presión (scale 0.98)

### 8. Elementos Visuales Adicionales
- **Textura de fondo**: Patrón geométrico sutil (líneas/dots en 10% opacity)
- **Efectos de iluminación**: Puntos de luz sutil en esquinas
- **Decoración imagen**: Elemento decorativo abstracto detrás de la foto
- **Animaciones**: Fade-in escalonado para elementos

### 9. Especificaciones Técnicas
- **Breakpoints**: Mobile (<768px), Tablet (768px-1024px), Desktop (>1024px)
- **Performance**: Imagen optimizada WebP + lazy loading
- **Accesibilidad**: Contraste mínimo 4.5:1, navegación por teclado, ARIA labels
- **SEO**: Estructura semántica correcta (h1, h2, p)

### 10. Assets Necesarios
1. **Foto profesional**: Retrato profesional con fondo neutro (800x1000px min)
2. **Textura de fondo**: Patrón geométrico SVG/PNG (1920x1080px)
3. **Iconos**: Font Awesome para CTAs
4. **Gradientes**: Definidos en CSS para performance

### 11. Paleta de Colores Detallada
```css
:root {
  --hero-bg-start: #0f172a;
  --hero-bg-end: #1e293b;
  --hero-text-primary: #f8fafc;
  --hero-text-secondary: #cbd5e1;
  --hero-accent-primary: #3b82f6;
  --hero-accent-secondary: #8b5cf6;
  --hero-button-primary: #3b82f6;
  --hero-button-primary-hover: #2563eb;
  --hero-button-secondary: transparent;
  --hero-button-secondary-hover: rgba(255, 255, 255, 0.1);
  --hero-border: rgba(255, 255, 255, 0.1);
}
```

### 12. Animaciones Propuestas
- **Entrada contenido**: Fade-up con delay escalonado
- **Entrada imagen**: Fade-in con scale ligero
- **Hover CTAs**: Transición suave de 300ms
- **Scroll indicators**: Animación sutil de bounce

---

**Nota**: Estos mockups sirven como guía visual para la implementación. Los detalles exactos de implementación (medidas, colores específicos, etc.) pueden ajustarse durante el desarrollo para optimizar rendimiento y accesibilidad.