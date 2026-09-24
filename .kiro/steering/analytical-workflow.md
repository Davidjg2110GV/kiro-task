---
inclusion: auto
name: analytical-workflow
description: Flujo paso a paso para resolver análisis exploratorios, métricas de negocio, segmentación, tendencias y preguntas estadísticas con datos locales.
---

# Flujo de trabajo analítico

1. **Enmarcar**: convertir la solicitud en una pregunta verificable; registrar objetivo, decisión, audiencia, periodo, población, unidad y definición de éxito.
2. **Inventariar**: localizar archivos y tablas relevantes; documentar formato, tamaño, columnas, claves candidatas, granularidad y fecha de actualización.
3. **Perfilar**: revisar tipos, rangos, cardinalidad, faltantes, duplicados, valores imposibles, consistencia entre tablas y cobertura temporal.
4. **Preparar**: aplicar transformaciones mínimas y explícitas; no sobrescribir la fuente original; registrar filtros, joins, deduplicación y reglas de imputación.
5. **Analizar**: elegir agregaciones, comparaciones, segmentaciones o pruebas acordes con la pregunta. Incluir denominadores, intervalos o sensibilidad cuando sea relevante.
6. **Validar**: reconciliar totales, revisar outliers, comparar con una segunda fuente o periodo, probar cortes alternativos y comprobar que no haya fuga de información.
7. **Comunicar**: presentar primero la conclusión, después la evidencia, el método, las limitaciones y las acciones recomendadas.
8. **Reproducir**: dejar una receta o consulta que permita repetir el resultado con la misma versión de los datos.

Si falta una definición crítica, formular una pregunta de aclaración en lugar de elegir silenciosamente una interpretación.
