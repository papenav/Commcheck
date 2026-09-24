# Análisis funcional de la demo oficial

## Naturaleza

La demo es una especificación interactiva del producto esperado. Sirve para validar experiencia, flujo, campos y reglas visibles. No es la base técnica de producción: funciona principalmente con datos en memoria y contiene simulaciones.

## Recorrido funcional

1. Buscar, filtrar y seleccionar un proyecto.
2. Crear el proyecto y definir su configuración inicial.
3. Crear o seleccionar una plantilla de controles.
4. simular o importar la línea base de activos.
5. Crear, clasificar y administrar activos/TAG.
6. Configurar la línea base de puntos de control.
7. Revisar catálogo y aplicabilidad por tipo de activo.
8. Registrar resultados TM, avance físico y protocolos.
9. Realizar carga masiva y asociación documental.
10. Consultar dashboard, readiness y brechas.
11. Enviar activos al Líder TM para aprobación o rechazo.
12. Crear la entrega y ejecutar el gate TM → Precomisionamiento.
13. Aceptar o rechazar los activos recibidos en Precomisionamiento.
14. Ejecutar el registro Precom, representado parcialmente.
15. Continuar hacia Comisionamiento, aún no implementado funcionalmente.
16. Continuar hacia PEM y Operaciones, aún no implementado funcionalmente.
17. Consultar el repositorio y simular la exportación del dossier.

## Capacidades representadas

- Hub y creación de proyectos.
- Plantillas y configuración de puntos de control.
- Línea base, clasificación y detalle de activos.
- Aplicabilidad de controles por activo.
- Registro TM y Precom parcial.
- Protocolos y carga documental simulada.
- Indicadores contractuales y funcionales.
- Aprobación del Líder TM.
- Entregas, gates y revisión del receptor.
- Repositorio documental y dossier simulado.

## Limitaciones que no deben confundirse con requisitos finales

- No existe persistencia ni backend empresarial.
- Los datos no están realmente aislados por proyecto.
- Roles y permisos son demostrativos.
- Importaciones, documentos y exportaciones se simulan total o parcialmente.
- Hay dos catálogos internos de controles que deben unificarse.
- Precomisionamiento está representado parcialmente.
- Comisionamiento y PEM son principalmente navegación y transferencia.
- La demo requiere reconstrucción con seguridad, auditoría, transacciones y trazabilidad.

## Regla de interpretación

La ausencia de una función en la demo no autoriza a inventarla. Se registra como pendiente y se valida con el cliente antes de diseñarla o construirla.
