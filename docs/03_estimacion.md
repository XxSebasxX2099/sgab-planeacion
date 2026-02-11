# Estimación

En esta sección se expone la descomposición del proyecto en módulos, la estimación de esfuerzo por módulo (horas/persona) y el nivel de incertidumbre asociado.

## Supuestos generales

- Trabajo individual (una persona con conocimientos básicos de desarrollo web y Git).  
- Volumen moderado de datos (hasta 2,000 registros).  
- No se integran servicios externos complejos ni pasarelas de pago.  
- Se dispone de una semana para la planeación y otros 3-4 semanas para una primera implementación si se continuara.

## Descomposición en módulos

1. Registro y autenticación de usuarios.  
2. Gestión de estudiantes (CRUD).  
3. Gestión de materias (CRUD).  
4. Registro y edición de calificaciones.  
5. Reportes y consultas (listados y exportes simples).  
6. Documentación y pruebas básicas.

## Tabla de estimación (horas)

| Módulo                            | Horas estimadas | Incertidumbre |
|-----------------------------------|----------------:|:-------------:|
| Registro y autenticación          |             10  |     Medio     |
| Gestión de estudiantes (CRUD)     |             12  |     Bajo      |
| Gestión de materias (CRUD)        |             10  |     Bajo      |
| Registro y edición de calificaciones |          14  |     Medio     |
| Reportes y consultas              |             12  |     Medio     |
| Documentación y pruebas           |             8   |     Bajo      |
| **Total estimado**                |           **66**|               |

Estas horas incluyen análisis, diseño ligero, pruebas manuales y documentación para cada módulo. La incertidumbre "Media" se asigna a módulos que dependen de reglas de negocio (p. ej. cálculo de promedios y validaciones de calificaciones) o de ajustes en autenticación institucional. Si se trabaja en equipo, dividir las tareas reduce horas por persona pero añade tiempo de coordinación.

## Justificación narrativa

Las estimaciones provienen de descomponer tareas en pasos realizables (formularios, validaciones, persistencia en BD, interfaces) y asignar horas realistas para desarrollo y verificación. Por ejemplo, registrar y autenticar usuarios implica diseñar el flujo, crear la tabla de usuarios, implementar registro y login seguro, y probar escenarios de roles; por eso se asignan 10 horas con incertidumbre media si se requiere integrar SSO institucional. Documentación y pruebas se estimaron de forma conservadora pero suficiente para evidenciar calidad mínima para la entrega.