# Plataforma de control de activos

Este repositorio es el único directorio oficial del proyecto.

## Regla de trabajo

1. La fuente funcional oficial es `fuente-oficial/commcheck_v8_STABLE.html`.
2. El diagrama `contexto/02-diagrama-componentes.md` es el instrumento principal de validación con el cliente.
3. La matriz `validacion/Matriz_validacion_funcional_demo_v2.xlsx` queda como referencia secundaria para consultar campos y cálculos.
4. `contexto/` contiene únicamente la interpretación consolidada de la demo.
5. Ningún archivo externo, Excel anterior o conversación modifica el alcance automáticamente.
6. Un detalle externo solo se incorpora después de una solicitud expresa, validación y registro en Git.

## Recorrido recomendado

1. Leer `contexto/00-fuente-y-alcance.md`.
2. Consultar `contexto/01-analisis-demo.md` para entender qué hace realmente el prototipo.
3. Revisar `contexto/02-diagrama-componentes.md` para comprender y validar la estructura conceptual y el flujo del proyecto.
4. Registrar las observaciones y decisiones de la revisión en `contexto/03-decisiones-y-pendientes.md`.
5. Consultar la matriz Excel solo cuando sea necesario revisar campos, opciones o cálculos detallados.
6. Consultar `contexto/04-cronograma-maestro.md` para planificar actividades, hitos y entregables desde la validación hasta producción.

## Estructura oficial

```text
Plataforma de control de activos/
├── README.md
├── fuente-oficial/
│   └── commcheck_v8_STABLE.html
├── contexto/
│   ├── 00-fuente-y-alcance.md
│   ├── 01-analisis-demo.md
│   ├── 02-diagrama-componentes.md
│   ├── 03-decisiones-y-pendientes.md
│   └── 04-cronograma-maestro.md
└── validacion/
    └── Matriz_validacion_funcional_demo_v2.xlsx
```

Los antecedentes retirados del árbol de trabajo permanecen recuperables en el historial de Git.
