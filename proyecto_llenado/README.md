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

