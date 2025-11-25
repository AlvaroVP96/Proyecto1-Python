# Proyecto 1 — Estación de llenado y taponado

Repositorio base para el proyecto de Python (introductorio) orientado a análisis de datos industriales.

## Estructura
```
.
├── data/                  # CSV de entrada (solo lectura). Pon aquí: telemetria.csv, eventos.csv, botellas.csv
├── fig/                   # Gráficos generados (PNG + SVG)
├── src/                   # Funciones reutilizables
├── notebooks/             # Notebooks de trabajo y reporte
├── requirements.txt       # Dependencias
├── proyecto_llenado.ipynb # Notebook principal
└── README.md
```

## Cómo ejecutar (paso a paso)
1. Crea un entorno (opcional pero recomendado):
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # Windows: .venv\Scripts\activate
   ```
2. Instala dependencias:
   ```bash
   pip install -r requirements.txt
   ```
3. Copia los CSV a `data/`.
4. Abre el notebook:
   ```bash
   jupyter lab  # o jupyter notebook
   ```
## 📄 Informe Ejecutivo

El análisis completo está documentado en **[`notebooks/informe.md`](notebooks/informe.md)**.

### Ver el informe

**En VS Code:**
- Abre `notebooks/informe.md`
- Presiona `Ctrl+Shift+V` para vista previa renderizada

**En navegador:**
```bash
start notebooks/informe.md  # Windows
open notebooks/informe.md   # macOS/Linux
```

### Exportar a PDF

**Opción 1: Pandoc** (recomendado - genera PDF profesional)
```bash
# Instalar pandoc: https://pandoc.org/installing.html
pandoc notebooks/informe.md -o notebooks/informe.pdf \
  --pdf-engine=xelatex \
  -V geometry:margin=2cm \
  -V linkcolor=blue \
  --toc \
  --toc-depth=2
```

**Opción 2: Extensión de VS Code**
1. Instalar extensión "Markdown PDF"
2. Abrir `notebooks/informe.md`
3. `Ctrl+Shift+P` → "Markdown PDF: Export (pdf)"

**Opción 3: Grip (visualización web)**
```bash
pip install grip
grip notebooks/informe.md
# Abrir http://localhost:6419 → Imprimir con Ctrl+P
```

### Contenido del informe

- **Resumen Ejecutivo:** Mensajes clave del análisis
- **KPIs Principales:** OEE, Scrap, Wh/ud por turno
- **Hallazgos:** 5 insights cuantificados con evidencia
- **Recomendaciones SMART:** 3 acciones con ROI calculado
- **Impacto Estimado:** OEE +9.4%, Scrap -69%, Payback 2.4 meses
- **Figuras Referenciadas:** 5 visualizaciones con interpretación
