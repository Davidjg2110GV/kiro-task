# Diseño: investigación web con evidencia

#[[file:.kiro/steering/web-research.md]]
#[[file:.kiro/skills/web-research-evidence/SKILL.md]]
#[[file:.kiro/steering/analyst-core.md]]

## Arquitectura conceptual

La investigación web es una etapa opcional y controlada del agent `data-analyst-expert`. Se activa cuando el usuario necesita datos actuales, contexto externo, documentación o verificación. El flujo es `Necesidad → Consulta → Fuente primaria → Contraste → Registro → Integración`.

## Flujo de información

1. **Necesidad**: registrar afirmación, indicador, entidad, alcance y fecha de corte.
2. **Consulta**: crear búsquedas neutrales sin incluir datos privados del proyecto.
3. **Evaluación**: revisar autoridad, fecha, metodología, definiciones y cobertura de la fuente.
4. **Contraste**: buscar evidencia independiente para afirmaciones materiales.
5. **Registro**: guardar cita, URL, fechas, fragmento o dato respaldado y limitaciones.
6. **Integración**: unir la evidencia externa con resultados locales indicando claramente la procedencia.

## Modelo de evidencia

Cada evidencia se registra con:

| Campo | Propósito |
|---|---|
| Afirmación | Qué se intenta verificar |
| Fuente | Entidad, título y URL |
| Publicación | Fecha de la fuente |
| Consulta | Fecha en que se revisó |
| Evidencia | Qué respalda exactamente |
| Confianza | Confirmada, parcial, contradictoria o no verificable |
| Limitaciones | Alcance, sesgo, definición o vigencia |

## Manejo de errores y límites

- Sin acceso web: comunicar que no se pudo verificar y ofrecer una estrategia de búsqueda manual.
- Página bloqueada o incompleta: no inferir su contenido; buscar una fuente primaria alternativa.
- Fuentes contradictorias: conservar ambas, comparar metodologías y evitar una certeza artificial.
- Fuente desactualizada: mostrar la fecha y buscar una actualización.
- Datos sensibles en la pregunta: detener la búsqueda externa, anonimizar y pedir confirmación si aún fuese necesaria.

## Criterios de seguridad

El agente debe minimizar la información enviada a herramientas web. Las URLs, consultas y resultados no deben contener secretos ni datos identificables. Las citas deben estar cerca de la afirmación que respaldan y no deben atribuir a una fuente algo que no demuestra.

## Estrategia de verificación

Se revisará que todas las afirmaciones externas tengan cita, que las fechas estén presentes, que las fuentes primarias se hayan priorizado, que las contradicciones estén declaradas y que el informe distinga evidencia web de cálculos locales.
