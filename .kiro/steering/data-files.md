---
inclusion: fileMatch
fileMatchPattern:
  - "**/*.csv"
  - "**/*.tsv"
  - "**/*.json"
  - "**/*.xlsx"
  - "**/*.xls"
  - "**/*.parquet"
  - "**/*.sql"
  - "**/*.ipynb"
---

# Convenciones para archivos de datos

- No modificar ni reemplazar archivos fuente; crear salidas derivadas con nombre y fecha claros.
- Detectar codificación, separador, encabezados, zona horaria y formato de fechas antes de cargar un archivo tabular.
- Confirmar tipos y granularidad; una fila no debe interpretarse como una entidad sin comprobarlo.
- Para joins, identificar claves, cardinalidad esperada y filas que se pierden o multiplican.
- Para fechas, declarar si los periodos son inclusivos, la zona horaria y el tratamiento de valores nulos.
- Para muestras o agregados, conservar denominadores y reglas de exclusión.
- Tratar notebooks como documentos ejecutables: distinguir celdas de exploración, resultados guardados y código reproducible.
- No publicar datos personales o confidenciales en tablas, logs, notebooks, artefactos ni prompts externos.
