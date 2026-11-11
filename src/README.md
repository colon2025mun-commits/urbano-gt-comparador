# Desarrollo técnico reproducible (`gt-salud-metropolitana`)

Espacio para versionar los scripts (Google Earth Engine, Python, openEO, R o SQL espacial) que generen las capas publicables en `geovisor/` y las contribuciones a `atlas/products/`.

| Ruta | Contenido |
|---|---|
| `gee/geourbano_comparador.js` | Script del Code Editor de Earth Engine: editas centroide, radio en km y años, y obtienes cuadrícula por año, deslizador A \| B, filtro de las 5 categorías, gráfico y estadísticas. |
| `python/comparador_gee.py` | Misma lógica con la API de Python; genera miniaturas y estadísticas que el sitio publica en `/comparador/`. Lo ejecuta `.github/workflows/comparador.yml`. |

Guía completa: [`docs/comparador-multitemporal.md`](../docs/comparador-multitemporal.md).
