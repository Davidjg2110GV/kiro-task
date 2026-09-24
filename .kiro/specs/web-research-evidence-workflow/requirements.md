# Requisitos: investigación web con evidencia

## Contexto
Los análisis pueden necesitar definiciones, benchmarks o hechos actuales que no están en los datos locales. La búsqueda web debe complementar el análisis sin introducir fuentes débiles, afirmaciones no verificadas ni exposición de datos privados.

## Requisito 1: definir la necesidad externa
**User story:** Como analista, quiero formular con precisión qué dato o afirmación externa necesito para no buscar contexto irrelevante.

### Criterios de aceptación
1. WHEN una pregunta requiere información externa THE SYSTEM SHALL definir la afirmación, indicador, entidad, periodo y fecha de corte que deben verificarse.
2. WHEN la solicitud puede resolverse con datos locales THE SYSTEM SHALL preferir la fuente local y explicar por qué no necesita búsqueda web.

## Requisito 2: buscar y evaluar fuentes
**User story:** Como lector, quiero evidencia de calidad y actualizada para distinguir hechos confiables de opiniones o contenido desactualizado.

### Criterios de aceptación
1. WHEN se realiza una búsqueda THE SYSTEM SHALL priorizar fuentes primarias y revisar contenido, metodología, alcance, autoría y vigencia.
2. WHEN una afirmación es material para la decisión THE SYSTEM SHALL contrastarla con otra fuente independiente cuando sea posible.
3. WHEN existen fuentes contradictorias THE SYSTEM SHALL reportar la discrepancia, sus definiciones y las razones para preferir una fuente o mantener la incertidumbre.

## Requisito 3: citar y proteger datos
**User story:** Como responsable del proyecto, quiero rastrear las afirmaciones externas sin exponer información sensible.

### Criterios de aceptación
1. WHEN se usa una fuente web THE SYSTEM SHALL citar entidad o título, URL, fecha de publicación, fecha de consulta y alcance de la evidencia.
2. WHEN se prepara una consulta externa THE SYSTEM SHALL excluir secretos, credenciales, identificadores y filas privadas; usar agregados o datos sintéticos.
3. WHEN una afirmación no puede verificarse THE SYSTEM SHALL marcarla como no verificada en lugar de presentarla como hecho.

## Requisito 4: integrar evidencia y análisis
**User story:** Como tomador de decisiones, quiero distinguir hechos externos, resultados propios e interpretaciones para usar la evidencia correctamente.

### Criterios de aceptación
1. WHEN se entrega un informe THE SYSTEM SHALL separar evidencia externa, resultados calculados, supuestos, inferencias y recomendaciones.
2. WHEN una fuente externa describe asociación o proyección THE SYSTEM SHALL conservar esa limitación y no convertirla en causalidad o dato observado.
