# Requisitos: flujo experto de análisis de datos

## Contexto
El workspace necesita un flujo consistente para responder preguntas analíticas con datos locales, manteniendo calidad, reproducibilidad y una comunicación útil para decisiones.

## Requisito 1: enmarcar la pregunta
**User story:** Como responsable de una decisión, quiero que mi pregunta se traduzca a métricas y alcance explícitos para saber qué se está midiendo.

### Criterios de aceptación
1. WHEN se recibe una solicitud analítica THE SYSTEM SHALL identificar objetivo, audiencia, población, unidad de observación, periodo, métricas, dimensiones y decisión asociada.
2. WHEN falta una definición que pueda cambiar el resultado THE SYSTEM SHALL pedir aclaración o declarar una interpretación provisional antes de calcular.

## Requisito 2: inspeccionar y preparar datos
**User story:** Como analista, quiero conocer la estructura y calidad de las fuentes antes de analizarlas para evitar conclusiones basadas en datos defectuosos.

### Criterios de aceptación
1. WHEN se selecciona una fuente THE SYSTEM SHALL registrar formato, tamaño, columnas, tipos, granularidad, fechas, claves candidatas y procedencia.
2. WHEN se prepara una fuente THE SYSTEM SHALL conservar el original y documentar filtros, joins, deduplicación, imputaciones y conversiones.
3. WHEN se detectan problemas THE SYSTEM SHALL cuantificar faltantes, duplicados, valores inválidos, inconsistencias y cobertura con denominadores.

## Requisito 3: analizar y validar
**User story:** Como usuario, quiero hallazgos cuantificados y comprobados para poder confiar en ellos.

### Criterios de aceptación
1. WHEN se presenta una cifra THE SYSTEM SHALL incluir unidad, periodo, población, denominador y método de cálculo.
2. WHEN se compara un grupo o periodo THE SYSTEM SHALL comprobar comparabilidad, tamaño de muestra y sensibilidad a definiciones alternativas.
3. WHEN una relación no tiene evidencia causal suficiente THE SYSTEM SHALL describirla como asociación y declarar las explicaciones alternativas relevantes.

## Requisito 4: comunicar de forma reproducible
**User story:** Como lector, quiero entender qué se encontró, qué limita el resultado y cómo repetirlo para convertirlo en una decisión informada.

### Criterios de aceptación
1. WHEN finaliza el análisis THE SYSTEM SHALL entregar pregunta, datos, método, hallazgos, limitaciones, recomendaciones y pasos reproducibles.
2. WHEN se incluye una visualización THE SYSTEM SHALL mostrar título, unidades, fuente, periodo, filtros y una escala que no distorsione la comparación.
3. WHEN no es posible verificar un resultado THE SYSTEM SHALL expresarlo claramente y no inventar valores ni conclusiones.
