---
name: data-quality-audit
description: Audita calidad y confiabilidad de datos mediante controles de esquema, completitud, unicidad, validez, consistencia, actualidad y reconciliación.
---

# Auditoría de calidad de datos

## Dimensiones mínimas
- **Completitud**: faltantes por columna, segmento y periodo; distinguir ausencia válida de error.
- **Validez**: tipos, rangos, dominios permitidos, formatos y reglas de negocio.
- **Unicidad**: claves duplicadas y duplicación inesperada después de joins.
- **Consistencia**: relaciones entre tablas, totales, unidades, monedas y zonas horarias.
- **Actualidad**: fecha de actualización, retrasos, huecos temporales y registros futuros.
- **Integridad**: claves foráneas, conservación de filas y reconciliación contra totales de control.

## Procedimiento
1. Define reglas y umbrales antes de mirar los resultados.
2. Ejecuta controles a nivel de archivo, columna, fila y relación.
3. Cuantifica fallos con conteo y porcentaje, siempre con denominador.
4. Clasifica severidad: bloqueante, alta, media o informativa.
5. Aísla ejemplos representativos sin exponer información sensible.
6. Decide si corregir, excluir, imputar o escalar; documenta el motivo.
7. Repite los controles después de transformar y antes de comunicar.

Nunca declares que los datos son "limpios" sin especificar qué controles se ejecutaron y qué límites permanecen.
