# Diseño: flujo experto de análisis de datos

#[[file:.kiro/steering/analyst-core.md]]
#[[file:.kiro/steering/analytical-workflow.md]]
#[[file:.kiro/skills/exploratory-data-analysis/SKILL.md]]
#[[file:.kiro/skills/data-quality-audit/SKILL.md]]

## Arquitectura conceptual

El agent `data-analyst-expert` orquesta cinco etapas: `Enmarcar → Inventariar → Preparar → Analizar → Comunicar`. La etapa de validación se ejecuta tanto después de preparar como antes de comunicar. Las instrucciones permanentes viven en steering; los procedimientos detallados viven en skills; esta Spec define el comportamiento esperado.

## Flujo de datos

1. **Entrada**: solicitud del usuario y archivos o tablas disponibles.
2. **Contrato analítico**: objetivo, alcance, métricas, definiciones y preguntas abiertas.
3. **Inventario**: perfil de esquema, calidad, granularidad y procedencia.
4. **Transformación derivada**: consultas o artefactos reproducibles sin modificar la fuente.
5. **Resultados**: estadísticas, tablas y visualizaciones con denominadores.
6. **Informe**: hallazgos, incertidumbre, limitaciones, recomendaciones y receta de reproducción.

## Componentes

- Agent: `/.kiro/agents/data-analyst-expert.json`.
- Steering permanente: principios de rigor, privacidad y contrato de salida.
- Steering automático: flujo de trabajo al tratar tareas analíticas.
- Steering por coincidencia: convenciones al abrir archivos de datos.
- Skills: exploración, auditoría de calidad y comunicación.

## Manejo de errores y límites

- Fuente ausente o ilegible: informar el bloqueo, pedir una fuente válida y no simular resultados.
- Esquema ambiguo: mostrar las columnas y solicitar definición de unidad o clave.
- Calidad insuficiente: cuantificar el problema, limitar el alcance y separar resultados confiables de exploratorios.
- Muestra pequeña o sesgada: evitar generalizaciones y reportar la limitación.
- Resultado no reproducible: conservar el método, parámetros, filtros y versión de la fuente.

## Estrategia de verificación

Revisar que cada cifra pueda rastrearse a una fuente y transformación, que los totales se reconcilien, que los filtros estén declarados y que las conclusiones no excedan la evidencia. La validación de configuración debe comprobar JSON válido, front matter válido, nombres de skills coincidentes con sus carpetas y rutas de recursos existentes.
