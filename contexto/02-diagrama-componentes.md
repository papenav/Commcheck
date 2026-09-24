# Diagrama conceptual del proyecto — versión 1

Estado: **borrador para validación**. Fuente: demo oficial F-012.

```mermaid
flowchart TB
    PROY[PROYECTO]

    ACT[ACTIVOS / TAG]
    ETAPA[ETAPAS DEL PROYECTO]
    USU[USUARIOS Y ROLES]
    REPO[REPOSITORIO DOCUMENTAL]

    PROY -->|tiene 1 a muchos| ACT
    PROY -->|tiene 4| ETAPA
    PROY -->|tiene 1 a muchos| USU
    PROY -->|tiene 1| REPO

    ETAPA --> TM[1. Terminación Mecánica]
    ETAPA --> PRE[2. Precomisionamiento]
    ETAPA --> COM[3. Comisionamiento]
    ETAPA --> PEM[4. Puesta en Marcha]

    TM -->|traspaso| PRE
    PRE -->|traspaso| COM
    COM -->|traspaso| PEM

    TM --> ESPTM[Especialidades]
    PRE --> ESPPRE[Especialidades]
    COM --> ESPCOM[Especialidades]
    PEM --> ESPPEM[Especialidades]

    ESPTM --> MEC1[Mecánica]
    ESPTM --> CAN1[Cañerías]
    ESPTM --> ELE1[Electricidad]
    ESPTM --> INS1[Instrumentación]

    ESPPRE --> MEC2[Mecánica]
    ESPPRE --> CAN2[Cañerías]
    ESPPRE --> ELE2[Electricidad]
    ESPPRE --> INS2[Instrumentación]

    ESPCOM --> MEC3[Mecánica]
    ESPCOM --> CAN3[Cañerías]
    ESPCOM --> ELE3[Electricidad]
    ESPCOM --> INS3[Instrumentación]

    ESPPEM --> MEC4[Mecánica]
    ESPPEM --> CAN4[Cañerías]
    ESPPEM --> ELE4[Electricidad]
    ESPPEM --> INS4[Instrumentación]

    MEC1 & CAN1 & ELE1 & INS1 -->|cada una tiene 0 a muchos| PCTM[Puntos de control TM]
    MEC2 & CAN2 & ELE2 & INS2 -->|cada una tiene 0 a muchos| PCPRE[Puntos de control Precom]
    MEC3 & CAN3 & ELE3 & INS3 -->|cada una tiene 0 a muchos| PCCOM[Puntos de control Com]
    MEC4 & CAN4 & ELE4 & INS4 -->|cada una tiene 0 a muchos| PCPEM[Puntos de control PEM]

    PCTM & PCPRE & PCCOM & PCPEM -->|cada punto pertenece a 1| CAM[Caminata 1, 2 o 3]

    ACT -->|según tipo y especialidad| APL[Controles aplicables al activo]
    PCTM & PCPRE & PCCOM & PCPEM --> APL

    APL -->|genera 0 o muchos| RES[Resultados / registros]
    RES -->|puede tener 0 o muchos| DOC[Protocolos y evidencias]
    DOC --> REPO

    RES -->|cuando cumple reglas| APR[Aprobación del líder de etapa]
    APR -->|agrupa 1 o muchos activos| ENT[Entrega / Gate]
    ENT --> REV[Revisión de etapa receptora]
    REV -->|acepta| SIG[Activo habilitado en la siguiente etapa]
    REV -->|rechaza| COR[Corrección y nueva revisión]
    COR --> ENT
```

## Lectura del modelo

- Un proyecto tiene uno o muchos activos.
- Un proyecto recorre cuatro etapas en orden: TM, Precomisionamiento, Comisionamiento y PEM.
- Cada etapa organiza sus controles por cuatro especialidades.
- Cada especialidad puede tener muchos puntos de control.
- Cada punto de control pertenece a una etapa, una especialidad y una caminata.
- Los puntos de control se asignan a los activos según su tipo, especialidad y aplicabilidad.
- Un control aplicado a un activo genera resultados y puede incorporar protocolos o evidencias.
- Cuando el activo cumple las reglas de la etapa, pasa a aprobación y luego a una entrega.
- La etapa receptora acepta el activo o lo devuelve para corrección.
- Los documentos generados quedan asociados al repositorio del proyecto.

## Aclaración estructural

Las cuatro etapas pertenecen al proyecto. Un punto de control específico pertenece a **una** etapa y a **una** especialidad; no es el mismo punto de control repetido obligatoriamente en las cuatro etapas. Cada etapa puede definir su propio catálogo de puntos de control.

Identificador de esta versión: `DC-001`.
