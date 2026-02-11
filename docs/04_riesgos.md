# Riesgos

A continuación se listan riesgos identificados, su tipo, probabilidad, impacto y la estrategia propuesta para su mitigación.

| ID | Riesgo | Tipo | Probabilidad | Impacto | Estrategia de respuesta |
|----|--------|------|:------------:|:-------:|-------------------------|
| R1 | Dependencia de servicio de autenticación externo (SSO) que cambia o no está disponible | Dependencia | Media | Alto | Evitar/mitigar: preparar autenticación local como plan B y documentar requisitos SSO. |
| R2 | Requisitos incompletos o mal definidos sobre reglas de calificación | Requisitos | Alta | Alto | Mitigar: validar reglas con el profesor/instructor antes de implementar; usar ejemplos concretos. |
| R3 | Falta de experiencia del desarrollador con la tecnología elegida | Humano/Técnico | Media | Medio | Mitigar: elegir stack conocido, reservar tiempo para aprendizaje y buscar apoyo en recursos. |
| R4 | Pérdida de datos por errores en almacenamiento o migraciones | Técnico | Baja | Alto | Mitigar/aceptar: realizar respaldos periódicos y pruebas de migración en entornos locales. |
| R5 | Cambios frecuentes (scope creep) por solicitudes extra de funcionalidades | Gestión/Alcance | Alta | Medio | Mitigar: definir proceso de control de cambios y aceptar solo cambios que pasen análisis de impacto. |
| R6 | Vulnerabilidades de seguridad por entrada no validada | Técnico/Seguridad | Media | Alto | Mitigar: validar entradas, sanitizar datos y revisar prácticas básicas de seguridad (uso de HTTPS). |

## Matriz de priorización

Se priorizan los riesgos que combinan alta probabilidad con alto impacto: R2 (requisitos incompletos) y R5 (scope creep) deben ser tratados primero mediante sesiones de clarificación y documento de alcance firmado. R1 (SSO) tiene impacto alto si ocurre, por lo que la mitigación con autenticación local como plan B es obligatoria.

## Plan de respuesta y seguimiento

- Registrar cada riesgo en `docs/04_riesgos.md` con fecha y responsable.  
- Revisar la lista de riesgos en cada commit significativo y actualizar probabilidad/impacto si cambian las condiciones.  
- Implementar controles técnicos (respaldo de BD, validaciones) y controles de gestión (reunión de aclaración de requisitos).