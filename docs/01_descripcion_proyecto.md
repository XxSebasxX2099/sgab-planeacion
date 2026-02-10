# Descripción del Proyecto

El objetivo de este documento es explicar con claridad qué se pretende construir, por qué es necesario y bajo qué supuestos operará el Sistema de Gestión Académica Básico (SGAB). El SGAB es una aplicación web pensada para facilitar la administración de información académica en una asignatura o en un pequeño departamento, está nos permitirá registrar estudiantes, materias, asignaciones y calificaciones, así como consultar reportes básicos. El propósito central es reducir la carga administrativa manual, evitar errores en el registro de calificaciones y ofrecer información consolidada sobre rendimiento académico que sirva tanto a profesores como a alumnos para tomar decisiones informadas.

El SGAB surge para atender la problemática recurrente en la gestión manual de información académica como procesos administrativos lentos y propensos a errores al registrar calificaciones, falta de trazabilidad en las modificaciones, inconsistencia de datos entre formatos físicos y digitales y la carencia de reportes consolidados que permitan evaluar el desempeño académico. Estas deficiencias generan carga administrativa excesiva para el personal, demoras en la entrega de resultados, errores en el cálculo de promedios y una experiencia de usuario que reduce la adopción de herramientas digitales. Además, la ausencia de registros de auditoría impide identificar con claridad quién realizó cambios y cuándo, dificultando la resolución de disputas y la garantía de integridad en los registros académicos.

Los usuarios principales del sistema serán administradores (personal encargado de la gestión de datos y configuración), profesores (quienes registran y editan calificaciones y gestionan la carga académica) y estudiantes (que consultan calificaciones y reportes).

Para las suposiciones iniciales se considerara que:

* La infraestructura de servidores será proveída por la institución.
* Se cuenta con acceso a internet estable en el campus.
* Los estudiantes cuentan con correo institucional para la autenticación en 2 pasos.