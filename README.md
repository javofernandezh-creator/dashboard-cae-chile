# Deuda Injusta — Radiografía pública del CAE

**No hay pago justo ante una deuda injusta.**

Sitio estático auditable. Contiene los JSON, el GeoJSON y las descargas CSV/ZIP; la biblioteca de gráficos se carga desde el CDN oficial de Plotly. Los extractos conservan fuente y página, pero el repositorio todavía no incluye un pipeline completo de extracción desde los documentos originales.

## Vista local

Desde la carpeta raíz del proyecto:

```powershell
python -m http.server 8765 --directory dashboard_publico
```

Abrir `http://127.0.0.1:8765`. No abrir `index.html` directamente: los navegadores bloquean la carga local de JSON mediante `fetch`.

## Publicación

Subir el contenido completo de `dashboard_publico` a cualquier hosting estático (GitHub Pages, Cloudflare Pages, Netlify, S3 u otro). No requiere proceso de compilación.

## Corte y limitaciones

- Indicadores estructurados principales: diciembre de 2023.
- 40 controles automáticos ejecutados entre integridad, reconciliación y cobertura; su aprobación no equivale a certificación externa.
- 339 de 341 registros comunales se cartografían de forma consistente.
- Los cruces socioeconómicos son agregados territoriales; no constituyen microdatos individuales ni permiten inferencia causal.
- 45 filas comunales no cumplen exactamente `al día + morosos = total`; se conservan los valores publicados y se muestran ambos denominadores agregados.
