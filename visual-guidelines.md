# Visual Guidelines — Ingenia Latam

Lineamientos gráficos para todos los artifacts, informes HTML,
dashboards y entregables visuales generados en Claude.

---

## Paleta de Color

| Nombre       | HEX       | Uso principal                                      |
|--------------|-----------|-----------------------------------------------------|
| Rojo Ingenia | `#ff110a` | Acentos fuertes, alertas, CTAs primarios, headers  |
| Naranja      | `#ff5800` | Elementos secundarios, íconos, bordes activos       |
| Naranja Claro| `#ff9400` | Highlights, badges, estados positivos, gradientes   |
| Blanco       | `#ffffff` | Fondos principales, texto sobre oscuro              |
| Plomo        | `#eeeeee` | Fondos secundarios, separadores, filas alternas     |

---

## Reglas de Aplicación

### Fondos
- Fondo principal de página/reporte: `#ffffff`
- Secciones alternas o cards secundarias: `#eeeeee`
- Headers de sección o banners: `#ff110a` con texto blanco

### Tipografía — Colores
- Texto principal sobre fondo blanco: `#1a1a1a` (negro suave)
- Texto sobre fondos de color (`#ff110a`, `#ff5800`): `#ffffff`
- Labels y metadatos: `#666666`

### Jerarquía de Color
1. `#ff110a` — Elemento dominante, una vez por vista (header, título principal)
2. `#ff5800` — Soporte estructural (subheaders, íconos, líneas divisoras)
3. `#ff9400` — Énfasis puntual (badges, estados, highlights de datos)
4. `#eeeeee` — Relleno neutro (backgrounds secundarios, tablas)
5. `#ffffff` — Espacio respirable, base

### Gradientes permitidos
- Primario: `linear-gradient(135deg, #ff110a, #ff5800)`
- Cálido: `linear-gradient(135deg, #ff5800, #ff9400)`

---

## Tipografía

### Fuentes de marca

| Fuente         | Rol                                         | Disponibilidad          |
|----------------|---------------------------------------------|-------------------------|
| Space Grotesk  | Headings, títulos, KPIs, números destacados | Google Fonts (pública)  |
| Google Sans    | Cuerpo de texto, párrafos, labels           | Propietaria de Google   |

> **Nota:** Google Sans no está disponible en Google Fonts público.
> En artifacts HTML usar **DM Sans** como sustituto — mismas proporciones,
> estilo geométrico idéntico. En contextos internos de Google (Slides, Docs),
> Google Sans carga automáticamente.

---

### Carga de fuentes — CDN (para HTML/artifacts)

```html
<!-- Siempre incluir en <head> -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;400;500;600;700&family=DM+Sans:ital,opsz,wght@0,9..40,300;0,9..40,400;0,9..40,500;0,9..40,600;1,9..40,400&display=swap" rel="stylesheet">
```

O como `@import` en CSS:

```css
@import url('https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;400;500;600;700&family=DM+Sans:ital,opsz,wght@0,9..40,300;0,9..40,400;0,9..40,500;0,9..40,600;1,9..40,400&display=swap');
```

---

### Fallback local (sin conexión)

Si el CDN no está disponible, el stack de fallback es:

```css
/* Headings — similar a Space Grotesk */
font-family: 'Space Grotesk', 'Trebuchet MS', 'Arial Narrow', sans-serif;

/* Body — similar a Google Sans / DM Sans */
font-family: 'DM Sans', 'Google Sans', 'Segoe UI', 'Helvetica Neue', Arial, sans-serif;
```

---

### Escala tipográfica

| Elemento       | Fuente        | Peso  | Tamaño sugerido |
|----------------|---------------|-------|-----------------|
| H1 / Título    | Space Grotesk | 700   | 2rem            |
| H2 / Sección   | Space Grotesk | 600   | 1.5rem          |
| H3 / Subsección| Space Grotesk | 500   | 1.2rem          |
| Body / Párrafo | DM Sans       | 400   | 1rem            |
| Label / Meta   | DM Sans       | 400   | 0.875rem        |
| KPI / Número   | Space Grotesk | 700   | 2.5rem+         |
| Caption        | DM Sans       | 300   | 0.75rem         |

---

## HTML / CSS — Variables Estándar

Cuando se genere código HTML, siempre declarar en `:root`:

```css
:root {
  --color-primary:   #ff110a;
  --color-secondary: #ff5800;
  --color-accent:    #ff9400;
  --color-white:     #ffffff;
  --color-light:     #eeeeee;
  --color-text:      #1a1a1a;
  --color-muted:     #666666;

  --font-heading: 'Space Grotesk', 'Trebuchet MS', sans-serif;
  --font-body:    'DM Sans', 'Google Sans', 'Segoe UI', Arial, sans-serif;
  --radius:       8px;
  --shadow:       0 2px 12px rgba(0,0,0,0.08);
}
```

---

## Componentes Base

### Botón primario
```css
background: var(--color-primary);
color: var(--color-white);
border-radius: var(--radius);
```

### Card / Panel
```css
background: var(--color-white);
border-left: 4px solid var(--color-primary);
box-shadow: var(--shadow);
border-radius: var(--radius);
```

### Badge / Estado
```css
background: var(--color-accent);   /* positivo */
background: var(--color-primary);  /* alerta / urgente */
color: var(--color-white);
```

### Tabla
```css
/* Encabezado */
background: var(--color-primary); color: var(--color-white);
/* Filas alternas */
background: var(--color-light);
```

---

## Qué NO hacer

- No usar más de 3 colores de la paleta en una misma vista
- No combinar `#ff110a` y `#ff9400` como fondos adyacentes sin separador blanco
- No usar `#eeeeee` como color de texto
- No agregar colores fuera de la paleta sin aprobación explícita

---

## Scope de Aplicación

Estos lineamientos aplican a:
- Artifacts HTML generados en Claude
- Dashboards y reportes interactivos
- Infografías y resúmenes visuales
- Documentos con estructura visual (no aplica a .docx o .pptx nativos)

---

*Última actualización: 2026-03-07*
