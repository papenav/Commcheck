# Fuente y alcance oficial

## Fuente funcional única

- Archivo: `fuente-oficial/commcheck_v8_STABLE.html`
- Identificador documental: F-012
- SHA-256: `cd639c6aedc328a5908b5e14a5fc7852a10fb6855295960b2cdae0ad629296ee`
- Decisión: su flujo, pantallas, campos, catálogos y cálculos observables son la fuente funcional inicial. **No cubre por completo Precomisionamiento, Comisionamiento ni PEM**. El alcance objetivo de la primera entrega incluye las cuatro etapas (DEC-009); las reglas faltantes no se deducen automáticamente de la demo y se validarán con el cliente.

## Instrumento principal de validación

- Archivo: `contexto/02-diagrama-componentes.md`
- Versión: `DC-001`
- Uso: validar con el cliente la estructura, jerarquías, cardinalidades y flujo general del proyecto.

## Referencia funcional secundaria

- Archivo: `validacion/Matriz_validacion_funcional_demo_v2.xlsx`
- SHA-256 inicial: `0818c1a00b741846d2028b4872a1662098b011287eafda21b081cabb62005de7`
- Contenido: 146 elementos organizados en 17 pasos, más flujo resumido y catálogos.
- Uso: consultar detalles de campos, opciones y cálculos cuando sea necesario; no será el instrumento principal de la reunión.

El hash de la matriz cambiará cuando se incorporen decisiones aprobadas. Cada versión debe quedar registrada en Git.

## Fuera del alcance automático

- Libros Excel anteriores.
- Minutas y análisis históricos.
- Interpretaciones surgidas en conversaciones.
- Reglas habituales de otras plataformas PPM.

Estos antecedentes pueden consultarse fuera del repositorio, pero solo entran a la solución mediante una decisión explícita y versionada.

## Jerarquía ante contradicciones

1. Decisión del cliente registrada en `03-decisiones-y-pendientes.md`.
2. Diagrama conceptual vigente aprobado por el cliente.
3. Comportamiento observable en la demo oficial.
4. Detalle disponible en la matriz Excel de referencia.

Si ninguna de estas capas resuelve una duda, el punto permanece pendiente para el cliente.
