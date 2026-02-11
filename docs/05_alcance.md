# Alcance

En este documento se define con precisión qué funcionalidades están incluidas en la primera versión del SGAB y cuáles quedan explícitamente fuera del alcance, así como las suposiciones que limitan el trabajo.

## Funcionalidades incluidas

- Registro y gestión de usuarios (roles: administrador, profesor, estudiante).  
- CRUD de estudiantes (crear, leer, actualizar, eliminar).  
- CRUD de materias.  
- Registro y edición de calificaciones por materia y alumno.  
- Consultas y reportes simples: listado de calificaciones por alumno y por materia, exporte CSV.  
- Documentación mínima y pruebas manuales que demuestren el correcto funcionamiento.

## Funcionalidades excluidas

- Integración con pasarelas de pago.  
- Aplicación móvil nativa.  
- Mensajería masiva (notificaciones automáticas por correo/push).  
- Módulos avanzados de analítica o dashboard en tiempo real.

## Suposiciones del alcance

- El sistema operará en un servidor con acceso web y base de datos relacional.  
- Los volúmenes de datos serán moderados y no requieren arquitectura distribuida.  
- Los usuarios contarán con cuentas institucionales; si SSO no es posible, se implementará autenticación local.

## Ejemplo de cambio (scope creep) y su impacto

Cambio propuesto: "Agrega envío de correos automáticos a estudiantes cuando se suba una calificación".  
Impacto estimado: requiere diseño de plantilla de correo, integración con un servicio SMTP, manejo de colas (si hay muchos correos) y pruebas adicionales. Esto podría aumentar al menos 8-12 horas el esfuerzo total y añadir riesgo de seguridad/configuración (credenciales de SMTP). Por tanto, cualquier solicitud de este tipo debe seguir el proceso de control de cambios: solicitud formal, análisis de impacto en tiempo y riesgos, aprobación o rechazo y actualización de documentación.

## Proceso sugerido de control de cambios

1. Documentar la solicitud de cambio en `docs/` con fecha y descripción.  
2. Analizar impacto en horas, riesgos y calidad.  
3. Decidir (aprobar/rechazar/postergar) y registrar la decisión.  
4. Si se aprueba, actualizar los archivos de estimación y alcance y versionarlos en Git.
