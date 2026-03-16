# Análisis de Contraste y Nueva Escala Tipográfica

## Análisis del Contraste Actual

### Colores y Contrastes
| Elemento | Color | Fondo | Ratio WCAG | Nivel WCAG |
|----------|-------|-------|------------|------------|
| Texto principal | #ffffff | #0a0a0f | 21:1 | AAA |
| Texto atenuado | #b3b3b3 | #0a0a0f | 7.5:1 | AA |
| Texto tenue | #808080 | #0a0a0f | 4.5:1 | AA |
| Acento | #00d4aa | #0a0a0f | 8.2:1 | AAA |
| Botón primario | #ffffff | #667eea | 4.7:1 | AA |
| Botón secundario | #ffffff | transparente | 21:1 | AAA |

### Jerarquía Tipográfica Actual
| Elemento | Tamaño móvil | Tamaño desktop | Peso | Color |
|----------|--------------|----------------|------|-------|
| h1 | 3rem (48px) | 4.5rem (72px) | 700 | #ffffff |
| Subtítulo | 1.25rem (20px) | 1.5rem (24px) | 600 | gradiente |
| Párrafo | 1.125rem (18px) | 1.25rem (20px) | 400 | #ffffff |
| Botones | 1rem (16px) | 1rem (16px) | 600 | varios |

## Problemas Identificados

1. **Jerarquía insuficiente**: La diferencia entre h1 y subtítulo es de solo 2.5x
2. **Contraste de color limitado**: Todos los textos usan blanco o variantes
3. **Falta de énfasis**: No hay suficiente diferenciación visual entre niveles
4. **Escala no modular**: Los tamaños no siguen una escala armoniosa

## Nueva Escala Tipográfica Propuesta

### Principios de Diseño
1. **Escala modular 1.25** (relación dorada)
2. **Contraste de color jerárquico**
3. **Pesos tipográficos diferenciados**
4. **Responsividad fluida**

### Nueva Escala (basada en 16px = 1rem)

| Nivel | Tamaño móvil | Tamaño desktop | Peso | Color | Ratio vs base |
|-------|--------------|----------------|------|-------|---------------|
| h1 (Nivel 1) | 3.5rem (56px) | 5rem (80px) | 800 | #ffffff | 5.0x |
| h1 acento | 3.5rem (56px) | 5rem (80px) | 800 | #00d4aa | 5.0x |
| Subtítulo (Nivel 2) | 1.75rem (28px) | 2.25rem (36px) | 600 | #b3b3b3 | 2.25x |
| Lead (Nivel 3) | 1.25rem (20px) | 1.5rem (24px) | 500 | #ffffff | 1.5x |
| Párrafo (Nivel 4) | 1rem (16px) | 1.125rem (18px) | 400 | #b3b3b3 | 1.125x |
| Small (Nivel 5) | 0.875rem (14px) | 1rem (16px) | 400 | #808080 | 1.0x |

### Especificaciones de Contraste Mejorado

1. **h1 principal**: 
   - Color: #ffffff (blanco puro)
   - Peso: 800 (extra bold)
   - Tracking: -0.02em (ligeramente condensado)
   - Line height: 1.1

2. **h1 acento**:
   - Color: #00d4aa (acento principal)
   - Peso: 800 (extra bold)
   - Efecto: text-shadow suave para profundidad

3. **Subtítulo**:
   - Color: #b3b3b3 (gris claro)
   - Peso: 600 (semi-bold)
   - Tracking: 0.01em (ligeramente expandido)
   - Line height: 1.3

4. **Texto lead**:
   - Color: #ffffff (blanco)
   - Peso: 500 (medium)
   - Line height: 1.6
   - Max width: 65ch (óptimo para lectura)

5. **Botones CTA**:
   - Primario: #00d4aa sobre #0a0a0f (8.2:1)
   - Secundario: #ffffff sobre transparente con borde (21:1)
   - Tamaño: 1.125rem (18px)
   - Peso: 600 (semi-bold)

### Implementación CSS

```css
/* Nueva escala tipográfica */
:root {
  /* Tamaños base */
  --text-xs: 0.75rem;    /* 12px */
  --text-sm: 0.875rem;   /* 14px */
  --text-base: 1rem;     /* 16px */
  --text-lg: 1.125rem;   /* 18px */
  --text-xl: 1.25rem;    /* 20px */
  --text-2xl: 1.5rem;    /* 24px */
  --text-3xl: 1.875rem;  /* 30px */
  --text-4xl: 2.25rem;   /* 36px */
  --text-5xl: 3rem;      /* 48px */
  --text-6xl: 3.75rem;   /* 60px */
  --text-7xl: 4.5rem;    /* 72px */
  --text-8xl: 5rem;      /* 80px */
  
  /* Pesos tipográficos */
  --font-thin: 100;
  --font-extralight: 200;
  --font-light: 300;
  --font-normal: 400;
  --font-medium: 500;
  --font-semibold: 600;
  --font-bold: 700;
  --font-extrabold: 800;
  --font-black: 900;
  
  /* Colores jerárquicos */
  --text-primary: #ffffff;
  --text-secondary: #b3b3b3;
  --text-tertiary: #808080;
  --text-accent: #00d4aa;
  --text-accent-hover: #00f5c4;
}

/* Aplicación en Hero */
.hero-title {
  font-size: clamp(3.5rem, 8vw, 5rem);
  font-weight: var(--font-extrabold);
  line-height: 1.1;
  letter-spacing: -0.02em;
  color: var(--text-primary);
  margin-bottom: 1.5rem;
}

.hero-title .accent {
  color: var(--text-accent);
  text-shadow: 0 0 30px rgba(0, 212, 170, 0.3);
}

.hero-subtitle {
  font-size: clamp(1.75rem, 4vw, 2.25rem);
  font-weight: var(--font-semibold);
  line-height: 1.3;
  letter-spacing: 0.01em;
  color: var(--text-secondary);
  margin-bottom: 2rem;
}

.hero-lead {
  font-size: clamp(1.25rem, 2.5vw, 1.5rem);
  font-weight: var(--font-medium);
  line-height: 1.6;
  color: var(--text-primary);
  max-width: 65ch;
  margin: 0 auto 3rem;
}

.hero-cta {
  font-size: var(--text-lg);
  font-weight: var(--font-semibold);
  padding: 1rem 2.5rem;
}

/* Responsividad fluida */
@media (max-width: 768px) {
  .hero-title {
    font-size: 2.5rem;
    margin-bottom: 1rem;
  }
  
  .hero-subtitle {
    font-size: 1.5rem;
    margin-bottom: 1.5rem;
  }
  
  .hero-lead {
    font-size: 1.125rem;
    margin-bottom: 2rem;
  }
}

/* Mejoras de contraste para accesibilidad */
@media (prefers-contrast: high) {
  :root {
    --text-secondary: #d9d9d9;
    --text-tertiary: #b3b3b3;
  }
  
  .hero-title .accent {
    color: #00ffcc;
    text-shadow: 0 0 20px #00ffcc;
  }
}
```

### Beneficios de la Nueva Escala

1. **Mejor jerarquía visual**: Relación 5:2.25:1.5 entre niveles
2. **Contraste optimizado**: Cumple con WCAG AA/AAA en todos los niveles
3. **Responsividad fluida**: Usa clamp() para transiciones suaves
4. **Accesibilidad mejorada**: Soporte para alto contraste
5. **Consistencia**: Escala modular aplicable a todo el sitio

### Próximos Pasos

1. Implementar las nuevas variables CSS en :root
2. Actualizar los estilos del componente Hero
3. Aplicar la escala a otros componentes del sitio
4. Realizar pruebas de contraste con herramientas WCAG
5. Validar la responsividad en diferentes dispositivos