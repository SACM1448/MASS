
# Modelo de Atención Transversal de la VAF

> **Tema:** Transformación del modelo de atención y servicios administrativos y financieros.  
> **Institución:** Universidad de los Andes.  
> **Objetivo general:** Mejorar la experiencia de profesores, administrativos y estudiantes mediante la integración, estandarización y automatización de los servicios.

---

## 1. Contexto y propósito

El **Modelo de Atención Transversal de la VAF** busca mejorar la experiencia de profesores, administrativos y estudiantes en el acceso a los servicios administrativos y financieros de la Universidad de los Andes.

El propósito es evolucionar hacia un modelo de atención más eficiente, integrado y centrado en el usuario, reduciendo los procesos manuales mediante:

- Estandarización de procedimientos.
- Automatización de actividades repetitivas.
- Integración entre las diferentes unidades.
- Centralización de los canales de atención.
- Mejoramiento de la experiencia del usuario.
- Gestión y aprovechamiento del conocimiento institucional.

### 1.1. Conceptos institucionales

| Concepto | Descripción |
|---|---|
| **VAF** | Vicerrectoría Administrativa y Financiera. |
| **PDI** | Plan de Desarrollo Institucional. |
| **DISRUPTIA** | Espacio de cocreación entre unidades y la DSIT, orientado a la adaptación al cambio y la construcción conjunta de soluciones. |
| **Eje estratégico de la VAF** | Experiencia total y de servicio. |

---

## 2. Metodología para abordar las necesidades

El levantamiento de MASS se concentra en observar e interpretar los servicios de IA existentes. Su alcance es comprender y documentar su funcionamiento técnico, funcional y operativo.

Se plantea una metodología de tres etapas:

### 2.1. Observar

**Objetivo:** identificar y comprender las necesidades, dificultades y puntos de dolor de los usuarios.

Consideraciones:

- Escuchar y comprender las necesidades de los usuarios.
- Identificar dificultades recurrentes.
- Obtener una visión general del panorama.
- Evitar concentrarse prematuramente en casos específicos.
- No proponer soluciones durante esta etapa.

**Resultado esperado:** comprensión general de la problemática y las necesidades del servicio.

### 2.2. Interpretar

**Objetivo:** analizar cómo funciona actualmente el servicio.

Consideraciones:

- Identificar los procesos involucrados.
- Comprender el funcionamiento del servicio.
- Reconocer los actores y responsables.
- Identificar dependencias entre unidades.
- Detectar oportunidades de mejora.
- Reconocer actividades manuales susceptibles de automatización.

**Resultado esperado:** entendimiento del funcionamiento actual y de los aspectos que requieren intervención.

### 2.3. Intervenir

**Objetivo:** diseñar, construir e implementar soluciones que respondan a las necesidades identificadas.

Consideraciones:

- Diseñar soluciones basadas en las necesidades observadas.
- Estandarizar procedimientos.
- Automatizar actividades cuando sea viable.
- Integrar plataformas y servicios.
- Mejorar la experiencia de los usuarios.

**Resultado esperado:** implementación de soluciones que optimicen el modelo de atención.

### 2.4. Representación de la metodología

```text
        ┌─────────────────────┐
        │     OBSERVAR        │
        │ Comprender dolores  │
        │ y necesidades       │
        └──────────┬──────────┘
                   │
                   ▼
        ┌─────────────────────┐
        │    INTERPRETAR      │
        │ Comprender procesos │
        │ y funcionamiento    │
        └──────────┬──────────┘
                   │
                   ▼
        ┌─────────────────────┐
        │     INTERVENIR      │
        │ Diseñar e           │
        │ implementar         │
        │ soluciones          │
        └─────────────────────┘
```

---

## 3. Modelo de atención End-to-End

El modelo de atención debe garantizar que cada solicitud sea gestionada de manera integral, desde su recepción hasta su resolución y cierre.

### 3.1. Principios del modelo

- **Conectividad:** las diferentes unidades deben estar articuladas.
- **Responsabilidad:** cada etapa debe contar con responsables definidos.
- **Estandarización:** los procedimientos deben estar documentados.
- **Trazabilidad:** debe ser posible conocer el estado de cada solicitud.
- **Tiempos de atención:** establecer tiempos de respuesta y resolución.
- **Continuidad:** evitar interrupciones o reprocesos entre unidades.

### 3.2. Flujo general de una solicitud

```text
   ┌─────────────────────────┐
   │    Usuario solicita     │
   │       un servicio       │
   └────────────┬────────────┘
                │
                ▼
   ┌─────────────────────────┐
   │   Canal de atención     │
   │  Entrada centralizada   │
   └────────────┬────────────┘
                │
                ▼
   ┌─────────────────────────┐
   │  Clasificación y        │
   │  asignación             │
   └────────────┬────────────┘
                │
                ▼
   ┌─────────────────────────┐
   │  Gestión y resolución   │
   │  N0 / N1 / N2           │
   └────────────┬────────────┘
                │
                ▼
   ┌─────────────────────────┐
   │  Respuesta al usuario   │
   │  y cierre de solicitud  │
   └─────────────────────────┘
```

**Objetivo:** evitar que el usuario deba gestionar manualmente su solicitud entre diferentes áreas.

---

## 4. Niveles del modelo de atención

El modelo contempla canales de entrada centralizados y tres niveles de atención.

### 4.1. Canales de atención

**Objetivo:** centralizar y estandarizar la recepción de solicitudes.

Los canales deben permitir que la información llegue de manera estructurada a los procesos correspondientes.

### 4.2. Nivel 0 — N0: SénecaBot

**Función principal:** autoservicio y atención automatizada.

Características:

- Estandarización del lenguaje.
- Reducción de tecnicismos.
- Atención de consultas frecuentes.
- Automatización de solicitudes sencillas.
- Orientación al usuario.
- Escalamiento a niveles superiores cuando corresponda.

### 4.3. Nivel 1 — N1: Atención inicial

**Función principal:** atención y resolución de solicitudes que requieren intervención humana de primer nivel.

Contexto identificado:

- Referencia: Leidy (lunes).
- Apoyo financiero.
- Procesos relacionados con matrículas.
- Atención de actividades centrales del negocio.
- Uso de Excel como base de conocimiento.

**Observación importante:**

Algunos usuarios no tienen acceso a Power BI o desconocen cómo utilizarlo.

Esto representa una barrera para el acceso a la información y debe considerarse en el diseño del servicio.

### 4.4. Nivel 2 — N2: Servicio especializado

**Función principal:** resolver solicitudes de mayor complejidad.

Características:

- Atención de casos especializados.
- Conocimiento técnico o funcional específico.
- Resolución de situaciones que no pueden ser atendidas en N0 o N1.
- Apoyo a la estandarización del conocimiento.
- Identificación de procedimientos que puedan delegarse a niveles inferiores.

### 4.5. Objetivo: pirámide invertida de atención

El modelo busca trasladar progresivamente la capacidad de resolución hacia los niveles inferiores.

**Delegación esperada:**

- **N2 → N1:** transferir procedimientos especializados que puedan estandarizarse.
- **N1 → N0:** automatizar solicitudes frecuentes mediante SénecaBot.

```text
          MODELO DE ATENCIÓN

    ┌───────────────────────────┐
    │            N0             │
    │         SénecaBot         │
    │   Autoservicio masivo     │
    └───────────────────────────┘
       ┌─────────────────────┐
       │         N1          │
       │  Atención inicial   │
       └─────────────────────┘
          ┌───────────────┐
          │      N2       │
          │ Especializado │
          └───────────────┘

       Transferencia de conocimiento:

              N2 → N1 → N0
```

**Resultado esperado:** aumentar la proporción de solicitudes resueltas en N0 y N1, reservando N2 para casos de mayor complejidad.

---

## 5. Plataformas, sistemas y herramientas

El inventario identifica herramientas mencionadas en el levantamiento. Las integraciones, los ambientes y las dependencias se validan por separado para cada servicio.

Se identificaron las siguientes herramientas dentro del ecosistema de atención.

| Plataforma | Función |
|---|---|
| **Faro Uniandes** | Apoyo financiero. |
| **Salesforce (CRM)** | Gestión de relaciones e interacciones con los usuarios. |
| **Acquia** | Gestión de sitios web institucionales. |
| **Inconcert** | Gestión y centralización de correos electrónicos y telefonía. |
| **SénecaBot** | Atención automatizada de nivel 0. |
| **Power BI** | Consulta y visualización de información. |
| **Excel** | Herramienta utilizada como base de conocimiento en algunos procesos. |

### 5.1. Inconcert

Actualmente se identifica como una plataforma para:

- Gestión de correos electrónicos.
- Centralización de comunicaciones.
- Gestión de telefonía.

**Evolución prevista:**

- Gestión de turnos presenciales.
- Integración futura con SénecaBot.

### 5.2. SénecaBot

Se identificó la siguiente relación entre componentes:

**Reportado.** El siguiente esquema conserva el orden en que se mencionaron los componentes. La dirección efectiva del intercambio y la función de cada enlace están pendientes de validación.

```text
    ┌──────────────┐
    │    CariAI    │
    └──────┬───────┘
           │
           ▼
    ┌──────────────┐
    │  SénecaBot   │
    └──────┬───────┘
           │
           ▼
    ┌──────────────┐
    │    Cuenta    │
    └──────────────┘
```

**Pendiente de validación:**

- Función específica de CariAI.
- Función del componente Cuenta.
- Tipo de integración entre los componentes.
- Flujo de información entre las plataformas.

---

## 6. Proyección estratégica 2027

Se identifican dos temas relevantes para el año 2027.

### 6.1. Seguridad psicológica

Promover un entorno de confianza en el que los equipos puedan:

- Expresar inquietudes.
- Compartir ideas.
- Proponer mejoras.
- Participar en procesos de transformación.
- Adaptarse a los cambios organizacionales.

### 6.2. Afinidad con la analítica de datos

Fortalecer las capacidades de los equipos para utilizar datos como apoyo a la gestión de los servicios.

Aspectos relacionados:

- Comprensión de información.
- Interpretación de indicadores.
- Toma de decisiones basada en datos.
- Identificación de oportunidades de mejora.
- Desarrollo de capacidades analíticas.

---

## 7. Síntesis de la iniciativa

La transformación del modelo de atención transversal de la VAF se fundamenta en cinco elementos principales:

1. **Experiencia del usuario:** mejorar la interacción con los servicios institucionales.
2. **Integración de procesos:** conectar las diferentes unidades involucradas.
3. **Automatización:** reducir actividades manuales y repetitivas.
4. **Gestión del conocimiento:** facilitar el acceso y transferencia de información entre niveles.
5. **Mejora continua:** evolucionar los servicios a partir de las necesidades identificadas.

### 7.1. Objetivo final

Consolidar un modelo de atención unificado, donde los usuarios puedan realizar solicitudes a través de canales estandarizados, recibir respuestas oportunas y contar con seguimiento de extremo a extremo, independientemente de las unidades que intervengan.

---

## 8. Aspectos pendientes de profundización

Los siguientes puntos requieren mayor información para comprender completamente el modelo:

- [ ] Identificar todos los canales de atención actuales.
- [ ] Comprender la arquitectura funcional de SénecaBot.
- [ ] Identificar la función de CariAI.
- [ ] Identificar el componente denominado Cuenta.
- [ ] Comprender cómo se integra Inconcert con las demás plataformas.
- [ ] Determinar el papel de Salesforce dentro del ciclo de atención.
- [ ] Identificar los responsables de cada nivel.
- [ ] Documentar los criterios de escalamiento entre N0, N1 y N2.
- [ ] Identificar las bases de conocimiento existentes.
- [ ] Definir los tiempos de respuesta y resolución.
- [ ] Identificar los procesos manuales susceptibles de automatización.
- [ ] Comprender los indicadores utilizados para medir la experiencia del usuario.

---

> **Nota:** Este documento organiza los apuntes recopilados sobre el Modelo de Atención Transversal de la VAF. Algunas descripciones fueron ampliadas para facilitar su comprensión. Las relaciones técnicas, integraciones y responsabilidades específicas deberán validarse con los equipos correspondientes.

---

## 9. Entrevistas sobre agentes en producción

La entrevista está dirigida a quien administra o da soporte a los agentes en producción. Se parte del contexto reportado de que la persona entrevistada no participa directamente en su desarrollo. Al inicio, identificar qué conoce de primera mano sobre arquitectura, integraciones y operación. Usar la agenda A si conoce la construcción técnica, la B si su experiencia es principalmente operativa, o combinar los bloques pertinentes. La reunión se centra en comprender los servicios y sus dependencias.

### 9.1. Agenda A — Conocimiento técnico integral

Duración sugerida de 90 minutos.

| Tiempo | Tema | Preguntas guía |
|---|---|---|
| 10 min | Inventario y canales | ¿Qué agentes están en producción, qué funciones tienen y por qué canales atienden? |
| 15 min | Arquitectura e infraestructura | ¿Qué componentes intervienen, dónde se alojan y existe un orquestador central? |
| 15 min | Construcción y despliegue | ¿Qué tecnologías, plataformas y repositorios utilizan? ¿Quién los administra? ¿Cómo versionan y despliegan las soluciones? |
| 15 min | Datos y conocimiento | ¿Qué fuentes consultan y cómo se actualizan? ¿Se usan RAG, embeddings o bases de datos vectoriales? |
| 15 min | Proveedores e integraciones | ¿Qué proveedores, modelos y APIs usan? ¿Cómo interactúan con sistemas institucionales y de qué servicios externos dependen? |
| 15 min | Operación y seguridad | ¿Cómo administran, monitorean y diagnostican los servicios? ¿Cómo gestionan los accesos y los incidentes? |
| 5 min | Documentación y cierre | ¿Qué documentación técnica existe y quién puede aclarar lo que quede pendiente? |

Solicitar diagramas de arquitectura y una demostración cuando estén disponibles.

### 9.2. Agenda B — Conocimiento operativo y soporte

Duración sugerida de 75 minutos.

| Tiempo | Tema | Preguntas guía |
|---|---|---|
| 10 min | Inventario operativo | ¿Qué agentes y servicios administra o soporta? ¿Qué función cumple cada uno? |
| 15 min | Plataformas y proveedores | ¿Qué plataformas y proveedores participan? ¿Qué función operativa asume cada uno? |
| 15 min | Comunicación e integraciones | ¿Qué relación tienen SénecaBot, CariAI y otros agentes? ¿Cómo se comunican entre sí y con los sistemas institucionales? ¿Qué ocurre cuando falla una integración? |
| 15 min | Administración y monitoreo | ¿Qué consolas utiliza? ¿Dónde consulta registros, alertas e indicadores? |
| 10 min | Diagnóstico y escalamiento | ¿Qué incidentes se repiten? ¿Cómo localiza el origen del fallo? ¿Qué resuelve directamente y qué casos escala? |
| 5 min | Seguridad y continuidad | ¿Cómo se administran permisos y accesos? ¿Qué mecanismos de continuidad existen? |
| 5 min | Documentación y cierre | ¿Qué guías operativas existen y quién puede responder las preguntas pendientes? |

Solicitar una demostración de las consolas y el recorrido de un incidente real, con los datos sensibles omitidos.

### 9.3. Registro y validación de hallazgos

| Estado | Criterio |
|---|---|
| Confirmado | El hallazgo se verificó con documentación, una demostración o un equipo que puede corroborarlo. |
| Reportado | El hallazgo se mencionó durante el levantamiento y está por corroborar. |
| Hipótesis | Es una interpretación técnica que requiere verificación. |
| Pendiente | Falta información o queda una pregunta abierta. |
| Descartado | Una fuente de validación refutó expresamente el hallazgo. |

Para cada hallazgo, registrar la fecha, el servicio o componente, la fuente, el estado y la evidencia o pregunta de validación. Si se corrige un dato, actualizar su descripción y conservar la trazabilidad del cambio.
