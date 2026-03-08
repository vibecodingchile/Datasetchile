# DataCL — Marketplace de Datasets para Chile 🇨🇱

> El primer marketplace de datasets curados para Chile y Latam. Datos limpios, listos para usar, con licencias claras y cumplimiento legal chileno.

**[→ Ver demo en vivo](https://vibecodingchile.github.io/datachile)**

---

## ¿Qué es DataCL?

DataCL es un marketplace especializado en datasets del mercado chileno y latinoamericano. A diferencia de plataformas genéricas como Kaggle o AWS Data Exchange, DataCL está **100% enfocado en datos locales** con:

- Licencias en pesos chilenos (CLP)
- Cumplimiento con Ley 19.628 / Ley 21.696 de Datos Personales
- Datasets enriquecidos con contexto chileno (CUT comunal, RUT, CIIU Rev.4, CIE-10)
- Sectores relevantes para el mercado local

## Sectores disponibles

| Sector | Datasets | Descripción |
|--------|----------|-------------|
| 🗺️ Geoespacial | 3 | GeoJSON comunas, tráfico RM, precio de suelo |
| 👷 Laboral | 2 | ENE histórico, remuneraciones sector público |
| 📊 Financiero | 3 | Bienes raíces RM, ChileCompra, deuda CMF |
| 🏥 Salud | 2 | Egresos hospitalarios DEIS, lista espera GES |
| 🛒 Comercio | 2 | E-commerce retail, locales SII geolocalizados |
| 🤖 IA / NLP | 2 | Corpus NLP chileno, dataset sintético personas |
| ⚖️ Jurídico | 2 | Jurisprudencia 280K sentencias, normativa legal |

## Características del MVP

- **Catálogo completo** con 14 datasets reales, búsqueda y filtros
- **Fichas detalladas** con esquema de campos, muestra de datos y casos de uso
- **3 tipos de licencia** por dataset: personal/investigación, comercial, suscripción
- **Documentación API** con ejemplos en curl, Python y formato de respuesta JSON
- **Página de planes** con 3 tiers: Explorer (gratis), Pro ($89K CLP/mes), Enterprise
- **Portal de proveedores** (WIP) para que otros puedan vender sus datasets
- Diseño responsive, dark mode, SPA sin frameworks

## Stack técnico

```
frontend/
├── index.html          # Entry point (GitHub Pages compatible)
├── css/
│   └── main.css        # Estilos completos (~600 líneas)
└── js/
    ├── datasets.js     # Data layer: 14 datasets completos
    └── app.js          # SPA router + toda la lógica UI
```

**Sin dependencias externas** — solo Google Fonts. 100% estático, desplegable en GitHub Pages en 30 segundos.

## Deploy en GitHub Pages

```bash
# 1. Crear repo en GitHub
git init
git remote add origin https://github.com/TU_USER/datachile.git

# 2. Push
git add .
git commit -m "feat: DataCL MVP inicial"
git push -u origin main

# 3. Activar GitHub Pages
# Settings → Pages → Source: Deploy from a branch → main / root
# En ~60 segundos: https://TU_USER.github.io/datachile
```

## Roadmap

### v0.2 — Backend básico
- [ ] API REST real (FastAPI + PostgreSQL)
- [ ] Autenticación con API Keys
- [ ] Checkout con Webpay / Stripe
- [ ] Dashboard de compras

### v0.3 — Datos reales
- [ ] Pipeline ETL para actualización automática de datasets
- [ ] Integración con fuentes públicas (SII, INE, MINSAL, Poder Judicial)
- [ ] Sistema de versioning de datasets

### v0.4 — Marketplace completo
- [ ] Portal de proveedores (subir y vender datasets)
- [ ] Sistema de reviews y ratings reales
- [ ] Facturación electrónica (DTE)
- [ ] Suscripciones recurrentes

### v1.0 — Expansión Latam
- [ ] Datasets de Colombia, Perú, Argentina
- [ ] Multi-moneda (USD, PEN, ARS, COP)
- [ ] SDK Python y Node.js

## Modelo de negocio

| Tipo | Split |
|------|-------|
| Datasets propios | 100% DataCL |
| Datasets de terceros | 70% proveedor / 30% DataCL |
| Plan Pro mensual | 100% DataCL |
| Enterprise | Negociado |

## Contacto

- Email: hola@datachile.io
- GitHub: [@vibecodingchile](https://github.com/vibecodingchile)

---

**Hecho con ♥ en Santiago, Chile 🇨🇱**

> *"Nadie más tiene esto enfocado en Chile o mercados latinos."*
