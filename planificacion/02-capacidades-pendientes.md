# Capacidades por validar para una plataforma empresarial de activos

Estado: **recomendaciones de alcance, no funcionalidad aprobada ni programada**. La demo HTML sigue siendo la fuente funcional inicial para el flujo de negocio. La primera entrega objetivo comprende TM, Precomisionamiento, Comisionamiento y PEM; este documento registra capacidades transversales que podrían faltar para una plataforma profesional.

## Decisiones antes de aprobar la línea base de V1

1. **Identidad y acceso.** Aprobar una matriz **perfil × acción × componente × alcance** para toda la plataforma; decidir cuentas locales o SSO, necesidad de MFA, usuarios externos, alta/baja, recuperación y política de sesiones. El cronograma V6 sitúa la implementación después de Construcción y Reportabilidad; mantiene en el mismo bloque la asociación de permisos a cada componente y reporte. La solución técnica, los perfiles concretos y las reglas de herencia/restricción siguen abiertos.
2. **Auditoría operativa.** Definir qué cambios y decisiones deben quedar trazados (usuario, momento, objeto, valor anterior/nuevo, motivo), quién consulta el historial y tiempo de conservación. Se menciona en el cronograma conceptual, pero no es una actividad separada con esfuerzo aprobado.
3. **Líneas base y versiones.** Determinar qué se congela por proyecto/etapa/activo, cómo se compara avance contra línea base y cómo se aprueba una modificación. No asumir que un único campo de estado resuelve el control de cambios.
4. **Gobierno de datos e importación inicial.** Acordar identificador único de TAG, catálogos, duplicados, validación, carga masiva, migración desde Excel y responsable de calidad de datos. Sin datos confiables, los indicadores y traspasos pierden valor.
5. **Operación productiva.** Fijar respaldo y restauración probada, monitoreo y alertas, capacidad/rendimiento esperado, soporte e incidentes, actualización y plan de reversión. El cronograma contempla parte del despliegue; faltan niveles de servicio y criterios medibles.

## Capacidades para priorizar con el cliente

- **Notificaciones y tareas pendientes:** avisos por asignación, rechazo, aprobación, vencimiento y traspaso; reglas para evitar ruido.
- **Búsqueda, filtros y vistas por rol:** localizar activos, controles, evidencias y entregas en grandes proyectos sin exponer datos fuera de permiso.
- **Indicadores trazables:** definir numerador, denominador, período, exclusiones y fuente de cada KPI antes de construir dashboards.
- **Gestión documental:** versiones, vigencia, permisos, tipos de evidencia y relación con el resultado aprobado.
- **Accesibilidad y experiencia de campo:** navegación usable, responsive y comportamiento con conectividad limitada si el cliente trabaja en terreno.
- **Integraciones/API y exportación:** formatos, destinatarios, límites y contratos de intercambio con sistemas existentes.
- **Visión de cartera PPM:** comparación entre proyectos, prioridades, riesgos, recursos y decisiones de gobernanza. Esta es una ampliación de alcance, no un requisito implícito del flujo TM → Precom.

## Criterio de planificación

Para cada punto elegido: propietario de la decisión, regla validada, entregable, prueba de aceptación, esfuerzo y dependencia. Solo entonces incorporarlo al **mismo cronograma maestro** con fechas. La fecha límite de marzo en V6 es un escenario acelerado de alto riesgo; revisarla antes de aprobar una línea base.
