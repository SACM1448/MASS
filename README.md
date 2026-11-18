# MASS — Modelo de atención transversal y ecosistema de IA

> **Institución:** Universidad de los Andes · **Estado:** levantamiento de información · **Actualizado:** 18 de noviembre de 2026  
> **Alcance:** comprender y documentar el modelo de atención de la VAF, los agentes de IA en producción, sus plataformas, integraciones y operación. MASS no presupone la construcción de una nueva solución ni la asignación de responsabilidades de soporte.

## 1. Propósito y alineación institucional

El modelo de atención transversal de la **Vicerrectoría Administrativa y Financiera (VAF)** busca mejorar la experiencia de estudiantes, profesores y administrativos mediante procesos articulados, atención consistente y menor dependencia de actividades manuales.

El **Programa de Desarrollo Integral (PDI) 2026–2030** de Uniandes es la hoja de ruta institucional. Este levantamiento se relaciona especialmente con:

| Referente del PDI | Relación con el modelo de atención |
|---|---|
| **Eficiencia administrativa que impulsa la sostenibilidad y la innovación institucional** (p. 41) | Integración de procesos, información y tecnología; interoperabilidad y automatización. El PDI menciona el **Sistema de Gestión de la Arquitectura Institucional (SGAI)** como habilitador. |
| **Bienestar y cultura de servicio para transformar la experiencia universitaria** (p. 42) | Atención centrada en las personas, asistentes virtuales, servicios omnicanal y capacidades digitales, analíticas y de servicio. |
| **Excelencia transformadora: tecnología para evolucionar con propósito** (p. 45) | Automatización inteligente, trazabilidad, integración de plataformas y gobernanza responsable de la IA. |
| **Interacciones significativas en el ecosistema universitario** (p. 46) | Experiencias ágiles y efectivas, visión integral del usuario y extensión del modelo único de atención a las unidades, con IA. |
| **Colaboración decidida para la generación de valor con datos** (pp. 47–48) | Interoperabilidad y uso de información confiable para decisiones; colaboración entre unidades. |
| **Evolución consciente de nuestra cultura de trabajo** (p. 49) | Adaptación, aprendizaje continuo y fortalecimiento de competencias técnicas y digitales. |

**Criterio:** estas son orientaciones institucionales del PDI, no evidencia de que cada capacidad ya esté implementada.

**Fuente:** Universidad de los Andes, *Programa de Desarrollo Integral 2026–2030*, pp. 41–49, documento institucional aportado al levantamiento.

### Enfoque de trabajo

1. **Observar:** escuchar necesidades y puntos de dolor sin anticipar soluciones.
2. **Interpretar:** comprender servicios, actores, flujos, dependencias y operación real.
3. **Intervenir:** etapa posterior de diseño o mejora, solo cuando corresponda.

**DISRUPTIA:** espacio reportado de cocreación entre unidades y DSIT para abordar cambios y soluciones conjuntas. Su alcance formal está por precisar.

## 2. Modelo de atención transversal

El objetivo es una atención **end-to-end**: recibir la solicitud, clasificarla, asignar responsables, gestionarla, responder y cerrar con trazabilidad. Se busca evitar que el usuario deba coordinar por sí mismo las transferencias entre unidades.

### Canales de entrada identificados

| Canal | Observación |
|---|---|
| Correo electrónico | Canal de atención reportado. |
| Llamadas telefónicas | Canal de atención reportado. |
| SénecaIA / SénecaBot | Canal automatizado de atención (N0). |
| Atención presencial | Canal de contacto directo. |
| Formularios específicos de servicios | Entradas propias de determinados procesos. |
| Otros | Categoría reportada, pendiente de desagregar. |

**Estado:** inventario inicial de canales realizado. Falta precisar responsables por canal, cobertura, registro y trazabilidad de solicitudes, interoperabilidad, y qué otros canales existen. No se asume que todos estén centralizados técnicamente.

### Niveles de atención

| Nivel | Papel previsto |
|---|---|
| **N0 — SénecaBot** | Autoservicio, orientación con lenguaje sencillo y tratamiento de solicitudes frecuentes. |
| **N1 — Atención inicial** | Apoyo funcional, especialmente en asuntos financieros y matrículas. Se reportó uso de Excel como base de conocimiento y barreras de acceso o manejo de Power BI para algunos usuarios. |
| **N2 — Especializado** | Resolución de casos que requieren conocimiento o intervención especializada. |

**Evolución buscada:** transferir conocimiento/procedimientos estandarizables de **N2 → N1 → N0**, para ampliar la resolución temprana sin sacrificar calidad ni acompañamiento humano. Los criterios concretos de escalamiento y los tiempos de atención aún deben levantarse.

## 3. Inventario de herramientas y agentes

| Componente | Función o relación conocida | Estado |
|---|---|---|
| **SénecaBot / SénecaIA** | Atención automatizada N0 y derivación hacia CuentaIA para asuntos de cuenta institucional. | Reportado |
| **CuentaIA** | Agente web que orienta en gestiones de acceso a la cuenta Uniandes. | Reportado; respaldado parcialmente por guía funcional |
| **CariAI** | Mencionado en relación con SénecaBot. | Función por validar |
| **Inconcert** | Centralización de correo y telefonía; se contempla gestión de turnos e integración futura con SénecaBot. | Uso y proyección reportados |
| **Salesforce** | CRM institucional. | Participación específica en el flujo por validar |
| **Acquia** | Gestión de sitios web institucionales. | Identificado |
| **Faro Uniandes** | Apoyo financiero. | Identificado |
| **Excel / Power BI** | Conocimiento operativo y consulta/visualización de información, respectivamente. | Uso y barreras reportados |

**Precaución:** el inventario no implica que todas estas plataformas estén integradas.

### 3.1. SénecaBot y CuentaIA

- **Reportado:** hay derivación de usuarios en ambos sentidos entre SénecaBot y CuentaIA. Falta confirmar reglas de derivación, mecanismos técnicos y transferencia de contexto.
- **Pendiente:** precisar la función de CariAI y su relación técnica con SénecaBot.

**CuentaIA — evidencia documental:** el documento *Flujo 2 – Restablecer y Cambio de Contraseña*, versión 5.4 (4 de marzo de 2025), está identificado como material de base de conocimiento para Copilot Studio. Orienta sobre cambio y restablecimiento de contraseña, primer acceso y contraseña vencida o vulnerable, con referencia al portal Cuenta Uniandes y canales oficiales. El agente no debe solicitar ni almacenar contraseñas o códigos.

**Arquitectura reportada de CuentaIA (levantamiento del 18/11/2026):**

| Plataforma | Participación reportada |
|---|---|
| Copilot Studio | Construcción del agente. |
| Power Automate | Automatizaciones del agente. |
| MuleSoft | Capa de integración para consulta o modificación de información, según el flujo. |
| Azure | Alojamiento del canal web reportado. |
| Cloudflare / DNS institucional | Publicación del servicio bajo dominio institucional; configuración por validar. |

**Sin confirmar:** recorrido técnico completo de una petición, responsabilidades precisas de Power Automate y MuleSoft, permisos, registros y acciones ejecutadas en sistemas externos. La existencia de la guía no demuestra que MuleSoft cambie contraseñas.

## 4. Operación y levantamiento técnico

Los agentes que gestiona la persona a entrevistar están **en producción**; su función es de **soporte, no de desarrollo**. No está definido si MASS tendrá responsabilidades futuras de soporte. El levantamiento busca entender primero qué existe y cómo opera.

### Agenda A — Si conoce arquitectura, repositorios y datos (90 min)

| Tiempo | Tema y objetivo |
|---|---|
| 10 min | **Inventario:** agentes, propósito, usuarios y canales. |
| 15 min | **Arquitectura:** componentes, infraestructura, orquestación y dependencias. |
| 15 min | **Construcción:** plataformas, tecnologías, repositorios, versiones y despliegues. |
| 15 min | **Datos/conocimiento:** fuentes, actualización, RAG, embeddings o BD vectoriales, si existen. |
| 15 min | **Proveedores e integraciones:** LLM, API, autenticación, middleware y sistemas institucionales. |
| 15 min | **Operación:** administración, monitoreo, logs, incidentes, seguridad y continuidad. |
| 5 min | **Cierre:** documentación y responsables de información faltante. |

**Demostración útil:** seguir una solicitud real de extremo a extremo e identificar dónde se registra, procesa, consulta y responde.

### Agenda B — Si conoce principalmente proveedores, comunicación y soporte (75 min)

| Tiempo | Tema y objetivo |
|---|---|
| 10 min | **Servicios:** agentes en producción, funciones y canales. |
| 15 min | **Proveedores:** plataformas y responsabilidades operativas. |
| 15 min | **Comunicación:** relación entre agentes, APIs, derivaciones y sistemas externos. |
| 15 min | **Administración:** consolas, monitoreo, logs, alertas e indicadores. |
| 10 min | **Incidentes:** fallos frecuentes, diagnóstico, escalamiento y límites del soporte. |
| 5 min | **Seguridad/continuidad:** permisos, datos y contingencias. |
| 5 min | **Cierre:** manuales, diagramas y contactos técnicos. |

**Demostración útil:** recorrer una consola operativa y un incidente real, sin exponer información sensible.

### Registro de evidencias

Clasificar cada hallazgo como **confirmado** (verificado), **reportado** (declarado), **hipótesis**, **pendiente** o **descartado**. Registrar fecha y fuente cuando sean conocidas. Distinguir iniciativas institucionales futuras de herramientas efectivamente implementadas.

## 5. Pendientes vigentes

- [ ] Precisar los **otros canales** y mapear responsabilidades, trazabilidad y sistemas utilizados en cada entrada.
- [ ] Comprender la arquitectura funcional, dependencias y herramientas de operación de SénecaBot.
- [ ] Aclarar el papel de CariAI.
- [ ] Validar la derivación bidireccional SénecaBot–CuentaIA y la conservación de contexto.
- [ ] Identificar el alcance real de Inconcert y Salesforce en el ciclo de atención.
- [ ] Documentar responsables, escalamiento N0/N1/N2 y tiempos de atención.
- [ ] Inventariar bases de conocimiento, fuentes de datos y responsables de actualización por agente.
- [ ] Identificar tareas manuales con potencial de estandarización, sin asumir una decisión de automatización.
- [ ] Conocer indicadores de atención, experiencia de usuario, disponibilidad e incidentes.
- [ ] Completar el mapa de proveedores, permisos, monitoreo y mecanismos de continuidad.

### Hallazgos ya incorporados (no pendientes)

- Inventario inicial de canales: correo, teléfono, SénecaIA/SénecaBot, presencial y formularios específicos; «otros» requiere desglose.
- Identificación de **Cuenta** como **CuentaIA** en el levantamiento y descripción de su orientación funcional.
- Identificación inicial de plataformas asociadas a CuentaIA, aún con integraciones concretas por validar.
- Alineación del objetivo del modelo de atención con las orientaciones del **PDI 2026–2030**.

---

> **Alcance documental:** notas de levantamiento complementadas con el PDI institucional. Las iniciativas estratégicas, observaciones operativas y hechos técnicos se diferencian expresamente para no presentar supuestos como implementaciones confirmadas.
