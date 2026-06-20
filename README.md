# Deuda Injusta — Radiografía pública del CAE

**No hay pago justo ante una deuda injusta.**

Sitio estático reproducible. Contiene los JSON, el GeoJSON y las descargas CSV/ZIP; la biblioteca de gráficos se carga desde el CDN oficial de Plotly.

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
- 35 de 35 controles de calidad aprobados.
- 339 de 341 registros comunales se cartografían de forma consistente.
- Los cruces socioeconómicos son agregados territoriales; no constituyen microdatos individuales ni permiten inferencia causal.
