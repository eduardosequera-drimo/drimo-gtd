# Benchmark de Competidores · GTD

Informe interactivo de **experiencia, usabilidad y diseño** de los sitios públicos de la
competencia regional de GTD (Chile, Perú, Colombia y referentes globales), pensado para
alimentar el rediseño de los sitios de GTD.

El sitio es un **único archivo `index.html`, totalmente autocontenido** (todas las capturas
van embebidas en base64, sin dependencias externas salvo las tipografías de Google Fonts).

## Qué contiene

- **30 sitios** analizados en 3 segmentos — **B2B (Empresas)**, **B2C (Hogar)** y **Ciberseguridad** —
  con constancia de país y fecha de revisión. 28 puntuados; 2 registrados como no accesibles.
- **Scorecard Hito 5:** 10 dimensiones ponderadas (suman 100 %), cada una puntuada 1–5, con
  **total ponderado 0–100** y justificación por dimensión basada en evidencia.
- Capturas de inicio, producto y contacto en **escritorio y móvil**.
- **Biblioteca de patrones** (qué adoptar / qué evitar) y listas accionables por competidor.

## Funciones del informe

- **Un solo filtro de segmento** (Todos · B2B · B2C · Ciberseguridad) que gobierna a la vez
  el panorama comparativo y las fichas; más filtros por país, búsqueda y orden.
- **Modo claro / oscuro** y look & feel alineado con DRIMO (Inter + JetBrains Mono, base
  grafito-azulada y acento violeta).
- Casilla de “revisada” y **notas por competidor** que se guardan en el navegador
  (`localStorage`).

## Despliegue en Vercel

Sitio 100 % estático, sin build.

- **Framework Preset:** `Other`
- **Build Command:** *(vacío)*
- **Output Directory:** *(raíz)*

Vercel sirve `index.html` en la raíz automáticamente. Cada `push` a `main` redepliega.

> **Privacidad:** es material competitivo. Para que la URL no sea pública, activa
> **Deployment Protection** (contraseña / SSO) en *Project → Settings → Deployment Protection*.

## Vista previa local

```bash
python3 -m http.server 8000
# abre http://localhost:8000
```

## Estructura

```
vercel_benchmark_gtd/
├── index.html        # el informe completo (autocontenido)
├── vercel.json       # configuración de despliegue (estático, cleanUrls)
└── README.md
```
