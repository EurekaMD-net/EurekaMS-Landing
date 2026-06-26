# EurekaMS — Landing Site

**EurekaMS · Mind Services** — Capa de inteligencia para negocios mexicanos.

## Descripción

Landing corporativa de EurekaMS (Mind Services), empresa de EurekaMD-net que provee inteligencia de datos, automatización de voz y análisis territorial para retail y servicios con 10–500 tiendas en México.

## Stack

- HTML5 + CSS custom (variables, grid, flexbox) + Vanilla JS (IIFE, requestAnimationFrame)
- Sin frameworks — sitio estático deployable en cualquier host
- Fuente de verdad: `/docs/documento-fundacional.md`

## Estructura

```
EurekaMS-Landing/
├── index.html              # Landing page principal
├── docs/
│   └── documento-fundacional.md   # Documento fundacional v1.1
├── assets/                 # Logos, imágenes
└── README.md
```

## Marca

- **Paleta:** Negro profundo (#0A0A0F) · Blanco (#FFFFFF) · Ámbar (#F59E0B)
- **Logo:** Monograma PCB — "E" caótica (ámbar) → "M" ordenada (blanco). Del caos al orden.
- **Logo oficial:** https://drive.google.com/file/d/1g9MUH0ZRvdXij2-XypAzXP0Y9u6WnL3M/view

## Pilares de producto

1. **Intelligence Ops** — Analista de datos 24/7 vía lenguaje natural
2. **Voice Solutions** — Vendedor AI que nunca duerme (motor: PipeSong + Deepgram + Kokoro)
3. **Territory Ops** — Inteligencia territorial con 6.1M establecimientos DENUE/INEGI

## Target

Retail especializado, servicios y food service · 10 a 500 tiendas en México · Tienen datos pero no visión.

## Demos interactivos (sesión 2026-06-26)

Cada pilar tiene un demo animado inline (mismo nivel que el pilar card, no en sección separada):

### Intelligence Ops demo
- Paleta: azul índigo
- 3 turnos: ranking SKUs por ventas → gráfica de barras → redistribución de inventario
- Panel derecho: pestañas SKUs / Comparativa / Redistribución

### Voice Solutions demo
- Paleta: verde/teal
- 3 turnos: resumen de llamadas de la mañana → lead con llamada más larga → KPIs consolidados
- Panel derecho: pestañas Llamadas / Resultados / KPIs
- Datos simulados: 12 leads, 62% contacto, 38% conversión, 2:51 prom

### Territory Ops demo
- Paleta: ámbar/dorado
- 3 turnos: ranking zonas CDMX por oportunidad → gráfica demanda vs saturación → top 3 prioritarias
- Panel derecho: pestañas Zonas / Demanda / Resumen
- Datos simulados: 10 zonas CDMX, 6.1M registros DENUE, mejor zona = Narvarte

### Cadencia compartida
- Paneles izquierdo (chat) + derecho (dashboard) animados en paralelo
- El agente activa la pestaña correcta al responder
- Loop automático: fade-out → reset → fade-in (idéntico en los 3 demos)

## Layout (post-refactor 2026-06-26)

Estructura de sección "Los 3 pilares":
```
#pilares
├── .pilar-modulo (Intelligence Ops)
│   ├── .pilar-card-row  ← card del pilar
│   └── #demo-ops        ← demo inline
├── .pilar-modulo (Voice Solutions)
│   ├── .pilar-card-row  ← card del pilar
│   └── #demo-voice      ← demo inline
└── .pilar-modulo (Territory Ops)
    ├── .pilar-card-row  ← card del pilar
    └── #demo-territory  ← demo inline
```

Antes los demos eran `<section>` separadas después del grid de pilares.
Ahora cada demo es un bloque inline debajo de su pilar card.

## Spacing

Valores actuales post-ajuste (2026-06-26):
- `section` padding: `4rem 1.5rem` (era `6rem`)
- `pilar-modulo` margin-bottom: `3rem` (era `5rem`)
- `pilar-card-row` margin-top: `1.25rem` (era `3rem`)
- `demo-outer` / `tdemo-outer` margin-top: `0.75rem` (era `2rem`)

## Desarrollo local

```bash
npx serve .
# o abrir index.html directamente en navegador
```

## Deploy actual

Caddy en VPS — `https://eurekaMS.187.77.25.101.nip.io/`
El archivo `index.html` se sirve directamente desde `/root/claude/projects/EurekaMS-Landing/`.

Sitio estático — compatible con Vercel, Netlify, Caddy, GitHub Pages.

---

*Una empresa EurekaMD-net · Junio 2026*
