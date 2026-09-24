# Decisiones y pendientes

## Decisiones vigentes

| ID | Decisión | Estado |
|---|---|---|
| DEC-001 | La demo F-012 es la única fuente funcional inicial. | Aprobada |
| DEC-002 | El repositorio es el único directorio oficial del proyecto. | Aprobada |
| DEC-003 | Los Excel y documentos anteriores no forman parte del alcance automático. | Aprobada |
| DEC-004 | La matriz demo v2 queda como referencia secundaria para campos y cálculos. | Reemplazada por DEC-007 |
| DEC-005 | Los antecedentes retirados se conservan únicamente en el historial de Git o en sus ubicaciones originales. | Aprobada |
| DEC-006 | `02-diagrama-componentes.md` es la fuente canónica del modelo entidad–relación. | Aprobada |
| DEC-007 | El diagrama conceptual `DC-001` es el instrumento principal de validación con el cliente. | Aprobada |
| DEC-008 | El desarrollo se planificará en un único cronograma maestro, desde validación del modelo hasta producción, con hitos verificables. | Aprobada |
| DEC-009 | El alcance objetivo de la primera plataforma incluye operación completa de TM, Precomisionamiento, Comisionamiento y PEM. La demo es incompleta en las últimas etapas; sus reglas se definirán y validarán antes de construirlas. | Definida por solicitante; pendiente ratificación cliente |
| DEC-010 | Identidad, login y perfiles son una base transversal. La aplicación de permisos a Proyecto, Activos y demás objetos se integra durante la construcción de cada componente. | Reemplazada por DEC-011; se conserva como historial |
| DEC-011 | Usuarios y acceso se implementan después de Construcción y Reportabilidad. Allí se definen perfiles, login y recuperación, administración central y asociación de permisos a cada objeto y reporte. El hito funcional anterior no autoriza producción. El escenario V5 proponía mayo de 2027. | Secuencia vigente; fecha V5 reemplazada por DEC-012 |
| DEC-012 | La fecha límite solicitada cambia a marzo de 2027. El cronograma V6 propone PROD el 31/03/2027 mediante frentes paralelos de acceso, pruebas y QA, con aceptación parcial solapada y sin reserva amplia para defectos. Se conserva el alcance completo y los gates de seguridad/cliente. | Definida por solicitante; escenario pendiente de validar capacidad y ratificación cliente |

## Pendientes prioritarios de validación

| ID | Tema | Resultado requerido |
|---|---|---|
| PEN-001 | Datos obligatorios del proyecto | Formulario aprobado |
| PEN-002 | Aislamiento y configuración por proyecto | Regla aprobada |
| PEN-003 | Catálogo único de controles de la demo | Catálogo aprobado |
| PEN-004 | Definición única de activo listo | Criterios y fórmula aprobados |
| PEN-005 | Reglas de aprobación y rechazo del Líder TM | Flujo aprobado |
| PEN-006 | Entrega y revisión TM → Precom | Estados y permisos aprobados |
| PEN-007 | Alcance funcional completo de Precomisionamiento | Backlog aprobado |
| PEN-008 | Alcance funcional de Comisionamiento | Backlog aprobado |
| PEN-009 | Alcance funcional de PEM y transferencia a Operaciones | Backlog aprobado |
| PEN-010 | Persistencia, auditoría, seguridad y permisos | Requisitos no funcionales aprobados |
| PEN-011 | Validar el diagrama conceptual `DC-001` con el cliente | Jerarquías, cardinalidades y flujo aprobados |
| PEN-012 | Fechar el cronograma maestro y asignar responsables, entregables y aceptación | Gantt comprometido aprobado |

## Protocolo de actualización

1. Registrar aquí las observaciones y decisiones obtenidas con el cliente.
2. Ajustar el diagrama cuando cambie una relación, cardinalidad o secuencia.
3. Actualizar la matriz Excel únicamente cuando una decisión afecte campos, opciones o cálculos detallados.
4. Crear un commit que explique el cambio.
