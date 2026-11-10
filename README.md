# DevCycle Automatization — Contexto y Estado del Proyecto

Documento maestro de referencia y resumen ejecutivo del proyecto **DevCycle Automatization** (Liverpool), consolidado y actualizado a partir de todas las minutas y sesiones técnicas del equipo (**31 de agosto al 10 de noviembre de 2026**).

> - **Repositorio de la aplicación (Monorepo Front + Back)**: [JTREJOR/devcycle-back-front](https://github.com/JTREJOR/devcycle-back-front)
> - **Memoria de control de lectura para IA**: [`COPILOT_MEMORY.md`](./COPILOT_MEMORY.md) *(registro de minutas ya procesadas para actualizaciones incrementales)*

---

## 1. Visión General del Proyecto

### ¿Qué es DevCycle Automatization?
**DevCycle Automatization** es una iniciativa estratégica para unificar, acelerar y automatizar de punta a punta el ciclo de vida de iniciativas tecnológicas en Liverpool *(decisión de unificación y nombre acordada el **31/08/2026** en `Technical Session - DevCycle team  - 2026_08_31 11_58 CST - Notas de Gemini.md` y `Sprint Planning - DevCycle team  - 2026_08_31 15_57 CST - Notas de Gemini.md`)*:

1. **Stage 0 — Intake / Descubrimiento (Discovery)**: Registro estandarizado y asistido por IA de ideas y necesidades de negocio, beneficios cuantificables/ROI e identificación inicial de impacto tecnológico.
2. **Stage 1 — Cartera de Pendientes y Priorización de Portafolio**: Validación obligatoria de impacto TI y sistemas afectados, evaluación mediante **Pizza, Pirámide y Scorecard**, y ordenamiento visual (*drag & drop* + ajuste manual justificado) por cartera de negocio.
3. **Refinamiento de Lienzo (Canvas)**: Construcción asistida por agente virtual e iteración de calidad y retroalimentación entre el área funcional, Business Partners (BP/BRM) y Vicepresidentes (VPs).
4. **Estimación Asistida con IA (*Assisti* / Calculadoras)**: Dimensionamiento (*sizing*), RAG con históricos y tarifas centralizadas de proveedores/BMO, cálculo de infraestructura GCP (Billing API) y generación de hojas de costos con escenarios multianuales, supuestos y riesgos.
5. **Validación Técnica y de Arquitectura**: Revisión y VoBo simultáneo de Líder Técnico y Arquitecto de Dominio (con ciclo de *"Refinar estimación"* en caso de observaciones).
6. **Generación Documental (*Quickly* — RFS / BRD / Charter)**: Agente en Google Cloud ADK conectado a Confluence y GESS para estructurar y emitir automáticamente los documentos de formalización.
7. **Formalización, Ejecución y Sincronización**: Trazabilidad bidireccional entre **Monday** (portafolio y visibilidad ejecutiva) y **Jira** (ejecución técnica), habilitando la baja definitiva de **Trisquel (Triskel)** en diciembre de 2026.

### Estrategia de Entrega en Dos Versiones: *Foundation* vs. *Enterprise*
> **Decisión clave (03/11/2026, 05/11/2026 y 09/11/2026)** — Documentos: `Technical Session - DevCycle team  - 2026_11_03 08_02 CST - Notas de Gemini.md`, `Technical Session - DevCycle team  - 2026_11_05 08_03 CST - Notas de Gemini.md` y `Sprint 3 Planning - DevCycle team  - 2026_11_09 15_59 CST - Notas de Gemini.md`.

Ante el vencimiento de licencias de **Trisquel en diciembre de 2026**, la entrega se dividió estratégicamente en dos fases:
- **Versión *Foundation* (Foundation Argos en Monday — En Producción desde el 09/11/2026)**:
  - Acotada exclusivamente al **registro digital de ideas 2027 y su trazabilidad en Monday**, sin calculadoras ni almacenamiento externo complejo.
  - Utilizada por la PMO (Alexis Labrada) y los Business Partners para capturar iniciativas reales y generar retroalimentación temprana sin bloquear la salida de Trisquel.
- **Versión *Enterprise* (Plataforma integral DevCycle)**:
  - Aplicación full-stack (Frontend React/Next.js + Backend de microservicios en Cloud Run + Agentes IA + Modelo de datos unificado con Monday).
  - Su primer incremento integrado abarca el **Stage 0 (Descubrimiento)** y **Stage 1 (Priorización con Pizza, Pirámide y Score)**, integrando progresivamente el Canvas, la calculadora (*Assisti*) y el generador de RFS/BRD (*Quickly*).

### Justificación e Impacto
- **Problema**: Los comités semanales y la elaboración manual de charters, RFS y hojas de costo consumen **~400 horas hombre al mes** *(validado el **22/09/2026** en `Technical Session - DevCycle team  - 2026_09_22 07_31 CST - Notas de Gemini.md`)*.
- **Meta**: Automatizar el **90.67%** del flujo operativo, liberando **~304 horas al mes** *(definido el **31/08/2026** en `Sprint Planning - DevCycle team  - 2026_08_31 15_57 CST - Notas de Gemini.md`)*.
- **Esquema y Transición**: Prototipo financiado por Innovación durante 2026 (con demostración ejecutiva a inicios de diciembre de 2026) que se congela al cierre de diciembre para transicionar formalmente al **modelo de Equipo Escalado en enero de 2027** *(confirmado el **10/11/2026** en `Technical Session - DevCycle team  - 2026_11_10 08_03 CST - Notas de Gemini.md`)*.

---

## 2. Participantes, Células y Gobernanza

- **Patrocinador Principal (Sponsor)**: Jorge Sánchez *(definido el **31/08/2026** en `Sprint Planning - DevCycle team  - 2026_08_31 15_57 CST - Notas de Gemini.md`)*.
- **Stakeholders Clave / Directivos**: Omar, Clemente (BRM), César Guzmán, Alexis Labrada (PMO / Monday), Patricia Santana (BMO / Tarifas / Validación funcional de flujos y costos).
- **Financiamiento de Innovación y Estrategia**: Itzana Jiménez Chavero, Adriana Hernández Parra, J. Inés Almazán Valerio.
- **Gobernanza Ágil, Facilitación y Seguimiento**:
  - **Alfredo Ledezma Cruz**: Asume el seguimiento general del proyecto y la transición a Equipo Escalado a partir del Sprint 3 *(anunciado el **09/11/2026** en `Sprint 3 Planning - DevCycle team  - 2026_11_09 15_59 CST - Notas de Gemini.md`)*.
  - **Dulce Kesia Valadez Guzmán**: Facilitación / Scrum Master durante Sprints 1–2 y promovida a **Coach de Agilidad** en noviembre de 2026 *(09/11/2026)*.
  - **Daniel Uribe**: Product Owner / Metodología inicial (Sprints 1–2).
- **Frentes y Células de Trabajo**:
  - **Frontend / UI & Lineamientos (*Argos / DevCycle Front*)**: **Javier Enrique Trejo Rodríguez** (Líder Frontend), en colaboración con Argos Eyra Martínez Zeferino, Miguel Javier Bermejo Guerrero y Manuel Chávez Ruiz.
  - **Backend, Modelo de Datos y Microservicios (*Data SWAT*)**: **Alejandro Javier Miranda Duardo** (Líder Backend / Modelo de datos), Argos Eyra Martínez Zeferino ("El man"), Miguel Javier Bermejo Guerrero, Manuel Chávez Ruiz, Brian Hernández García.
  - **Portafolio, Intake y Monday (*Foundation & Enterprise*)**: Ivonne Anayelli Hernández Castellanos, Belén Romero Arzate, Josefina Luna, María Fernanda Torres (Mafer), Alma Reyna Alba Rivera.
  - **Estimaciones y Calculadora con IA (*Assisti*)**: Jonathan Jesús Romero Torrecilla, Erick Iván Soria Morales.
  - **Agente de Documentación RFS/BRD y Confluence (*Quickly*)**: Iván Barajas Muñoz, Josette Redonda Alva.
  - **Arquitectura Cloud, Infraestructura y Golden Pipelines**: Andrés Beléndez Saldaña, Elodia Moreno, Jorge Alberto Ozuna Cruz, Josué González Escandón, Luz Vanessa Becerra Rivera.
  - **UX / Sistema de Diseño / Librerías**: Gustavo Vargas, Cassandra (certificación en Figma).

---

## 3. Arquitectura Funcional y Técnica

### 3.1. Flujo Funcional de 7 Pasos

```text
[ Stage 0: Intake / Descubrimiento ]
       │ (Formulario estandarizado, chat IA, correos corporativos, ROI/beneficios e impacto TI)
       ▼
[ Stage 1: Cartera de Pendientes & Priorización ]
       │ (Validación TI y sistemas afectados, evaluación Pizza + Pirámide + Score,
       │  ordenamiento Drag & Drop o ajuste manual justificado, alertas y notificaciones)
       ▼
[ Paso 2: Lienzo de Iniciativa (Canvas IA) ]
       │ (Construcción asistida por IA y ciclo iterativo de VoBo entre Funcional y BP/VP)
       ▼
[ Paso 3: Estimación Asistida (Assisti / Calculadora IA) ]
       │ (Preguntas contextuales de sizing, RAG de históricos + tarifas BMO/SAP + GCP Billing API,
       │  escenarios multianuales y pestañas de supuestos y riesgos)
       ▼
[ Paso 4: Validación Técnica y de Arquitectura ]
       │ (VoBo paralelo de Líder Técnico y Arquitecto de Dominio; flujo de "Refinar estimación")
       ▼
[ Paso 5: Generación Documental (Quickly — RFS / BRD / Charter) ]
       │ (Agente ADK en GCP + Vertex AI conectado a Confluence y GESS con plantillas JSON/MD)
       ▼
[ Paso 6: Formalización, Ejecución y Cierre ]
         (Modelo de datos unificado BD <-> Monday y sincronización de ejecución con Jira)
```

### 3.2. Arquitectura Cloud, Backend e Integración
Definida en las sesiones de arquitectura de octubre y noviembre de 2026 (`Technical Session - DevCycle team  - 2026_10_15 07_59 CST - Notas de Gemini.md`, `Technical Session - DevCycle team  - 2026_10_20 07_59 CST - Notas de Gemini.md` y `Technical Session - DevCycle team  - 2026_11_05 08_03 CST - Notas de Gemini.md`):

- **Infraestructura en Google Cloud Platform (GCP)**:
  - Todas las aplicaciones conviven en un mismo proyecto de GCP comunicándose mediante **Cloud Run**, operando con entornos **sandbox** (pruebas) y **prototipo** (producción) *(acordado el **15/10/2026**)*.
  - Aprovisionamiento mediante **Infraestructura como Código (Terraform)** y **Google Cloud Build**, alineado con los **Golden Pipelines** corporativos *(acordado el **15/10/2026**)*.
- **Modelo de Datos Unificado y Contratos**:
  - Contratos de microservicios estandarizados en **JSON** (GET/POST, tipado estricto) para desacoplar el frontend del backend *(acordado el **15/10/2026**)*.
  - **Modelo de datos unificado** diseñado para persistir la información de manera consistente tanto en la base de datos de la aplicación como en los tableros de **Monday** *(acordado el **05/11/2026**)*.
- **Inteligencia Artificial y Bases de Conocimiento**:
  - **Assisti (Calculadora)**: Motor con Gemini + RAG sobre históricos de charters/hojas de costos, pestañas de supuestos y riesgos en BD *(01/10/2026)*, escenarios multianuales *(03/11/2026)*, preguntas contextuales automáticas cuando faltan métricas como peticiones por segundo *(20/10/2026)* y catálogo centralizado de tarifas de proveedores/BMO (con revisión de integración SAP) *(22/10/2026)*.
  - **Quickly (RFS / BRD)**: Migrado de Gemini Enterprise al **Agent Development Kit (ADK)** en GCP con **Vertex AI**, lectura/escritura en **Confluence** y conexión con **GESS**, usando templates estructurados en JSON/XML/Markdown *(01/10/2026, 20/10/2026 y 03/11/2026)*.

---

## 4. Especificaciones y Evolución del Frontend ("El Front")

El frontend (liderado por **Javier Enrique Trejo Rodríguez**) evolucionó de un mockup inicial a una arquitectura modular con lineamientos estrictos de desarrollo y diseño.

### 4.1. Pantallas y Reglas Funcionales Vigentes

1. **Pantalla de Inicio (*Home* / Mis Iniciativas)**:
   - Muestra las iniciativas según el perfil/participación del usuario (los Portfolio Managers visualizan el portafolio completo de su cartera; los solicitantes ven sus iniciativas registradas) *(14/09/2026 y 15/10/2026)*.
   - **Categorías de estatus en el Home**: *Backlog*, *Aprobadas*, *Rechazadas* y *Sin etapa definida* *(acordado el **14/10/2026** en `DevCycle_ Front_ 2026_10_14 07_19 CST - Notas de Gemini.md`)*.
   - **Botones de acción rápida simplificados**: Se eliminaron los botones *"Ir a priorización"* y *"Ver comité"*, conservando únicamente **"Seguimiento de portafolio"** y **"Levantar iniciativa"** *(acordado el **14/10/2026** en `DevCycle_ Front_ 2026_10_14 07_19 CST - Notas de Gemini.md`)*.
   - Al seleccionar una iniciativa, navega a la **Ficha de Proyecto** con el resumen y avance a través de las etapas alineadas con Monday y Miro (*Priorización, Estimación, Autorización, Formalización, Ejecución y Cierre*) *(14/10/2026 y 15/10/2026)*.

2. **Formulario de Registro — Stage 0 (Intake & Discovery)**:
   - **Campos principales**: Título, Unidad de Negocio / Dirección (Digital, EPL, Negocios Financieros, Tecnología, Transformación, Construcción), Solicitante y Sponsor mediante **correo electrónico corporativo**, más correos adicionales de interesados del negocio para notificaciones *(14/09/2026)*.
   - **Asistente Virtual (Chat IA)**: Apoyo interactivo para redactar y estructurar la necesidad de negocio *(14/09/2026)*.
   - **Impacto Tecnológico**: Confirmación de intervención de TI y buscador de sistemas/plataformas impactadas *(14/09/2026)*.
   - **Beneficios, ROI y Presupuesto**: Captura de beneficios cuantificables/monetizados (horas hombre, nuevos ingresos, ahorros directos, reducción de tiempos, mitigación de riesgos/cumplimiento) y sección de presupuesto validada *(14/09/2026 y 01/10/2026)*.
   - **Campos excluidos en captura inicial**: Dependencias arquitectónicas previas y fecha objetivo manual para evitar ruido al solicitante *(14/09/2026)*.

3. **Cartera de Pendientes y Priorización — Stage 1**:
   - **Validación previa en Backlog**: Confirmación obligatoria por el Portfolio Manager de si la iniciativa tiene impacto TI y validación de sistemas afectados antes de priorizar *(14/09/2026)*.
   - **Filtros por Dirección/Cartera**: Vistas independientes por cartera de negocio según el perfil del Portfolio Manager *(14/09/2026)*.
   - **Evaluación Multicriterio (Pizza, Pirámide y Scorecard)**: Herramientas visuales de evaluación de valor/esfuerzo y alineación estratégica construidas en conjunto entre Argos y Javier Trejo *(14/10/2026 y 05/11/2026)*.
   - **Ordenamiento Visual (*Drag & Drop*) + Modificación Manual ("Dedazo")**: Sin columna numérica manual en el registro inicial; ordenamiento vertical tipo Jira con opción de ajuste manual justificado ante emergencias o cambios directivos de negocio *(14/09/2026, 17/09/2026 y 14/10/2026)*.
   - **Alertas de Desplazamiento y Formalización**: Alerta del número de proyectos desplazados al reordenar y botón de confirmar/formalizar que dispara notificaciones por correo y Google Chat a PMO, BRMs, VPs y solicitantes *(14/09/2026)*.

4. **Lienzo (Canvas), Estimación (*Assisti*) y Aprobaciones**:
   - Flujo iterativo de refinamiento del Canvas entre usuario funcional y Business Partner / VP hasta el VoBo *(02/09/2026 y 14/10/2026)*.
   - Interacción con el chat de la calculadora (*Assisti*), que detecta datos faltantes y lanza preguntas contextuales de *sizing* *(20/10/2026)*.
   - Integración de la calculadora en la aplicación principal bajo un **documento formal de lineamientos de integración** elaborado por el frente de UI *(10/11/2026)*.
   - Doble validación simultánea (Líder Técnico + Arquitecto de Dominio) con acción de **"Refinar estimación"** si existen observaciones, previo a emitir la hoja de costos y el RFS/Charter *(02/09/2026)*.

5. **Administración de Roles, Perfiles y Permisos**:
   - Matriz y tabla depurada de usuarios, roles y permisos para controlar el acceso y acciones por pantalla *(14/10/2026 y 15/10/2026)*.

### 4.2. Lineamientos Técnicos, UX y Operativos
- **Stack Frontend**: React / Next.js con **Turbopack**, desplegado en **Vercel** para revisiones ágiles y preparado para contenedorización en **Cloud Run** *(14/10/2026 y 15/10/2026)*.
- **Diseño y UX**: Diseño certificado en **Figma** con **Cassandra** y alineado a las librerías de **Gustavo Vargas**, diferenciando el estilo visual definitivo de DevCycle frente a los mockups preliminares de Monday *(17/09/2026 y 15/10/2026)*.
- **Documentación de Lineamientos (Entregables F3 / F4)**: Separación formal en dos documentos rectores —lineamientos de desarrollo Frontend y lineamientos de desarrollo Backend— junto con los diagramas de flujo de navegación *(15/10/2026 y 20/10/2026)*.
- **Capacidad y Dedicación del Equipo**: Límite operativo acordado de **4.5 horas semanales** por integrante técnico y depuración de reuniones redundantes (conservando sesiones de refinamiento martes y jueves y sesiones técnicas bajo demanda) *(14/10/2026 y 15/10/2026)*.

---

## 5. Bitácora Cronológica de Decisiones Importantes

Cada decisión relevante incluye la **fecha exacta** y el **documento fuente** donde fue acordada:

| Fecha | Decisión Acordada | Documento Fuente |
| :--- | :--- | :--- |
| **31/08/2026** | Consolidar los esfuerzos aislados en **un único proyecto unificado de punta a punta** con un **frontend indispensable** liderado por Javier Enrique Trejo Rodríguez e integrando librerías del equipo de Gus Vargas. | `Technical Session - DevCycle team  - 2026_08_31 11_58 CST - Notas de Gemini.md` |
| **31/08/2026** | Adoptar el nombre **DevCycle Automatization**, designar a **Jorge Sánchez** como sponsor principal (con Omar, Clemente, César Guzmán y Alexis Labrada como stakeholders) y financiar la fase inicial como **prototipo de innovación** (presupuesto de Itzana Jiménez) ante el vencimiento de **Trisquel en diciembre de 2026**. | `Sprint Planning - DevCycle team  - 2026_08_31 15_57 CST - Notas de Gemini.md` |
| **02/09/2026** | Asignar al **Business Partner (BP/BRM)** la responsabilidad de complementar el contexto técnico (*sizing*), validar la calidad del Canvas y entregar la estimación final al negocio; integrar desde el inicio al **Líder Técnico y Arquitecto de Dominio** para validación paralela y nombrar **"Refinar estimación"** al flujo de ajuste. | `Technical Session - DevCycle team  - 2026_09_02 06_55 CST - Notas de Gemini.md` |
| **14/09/2026** | Trabajar en **ramas propias** en Git; registrar solicitante y sponsor por **correo corporativo**; eliminar del formulario inicial los campos de presupuesto manual, fecha objetivo y dependencias de arquitectura; crear la etapa previa de **Cartera de Pendientes (Backlog)** para confirmar impacto TI; **eliminar la columna numérica de prioridad** en favor de la posición visual; y definir 4 etapas y 4 estados base. | `DevCycle_ 2026_09_14 07_21 CST - Notas de Gemini.md` |
| **17/09/2026** | Implementar ordenamiento de prioridades mediante **arrastrar y soltar (*Drag & Drop* tipo Jira)** y estructurar el tablero de seguimiento en **3 niveles** (épica, historia, tarea) replicado en Monday. | `Technical Session - DevCycle team  - 2026_09_17 07_15 CST - Notas de Gemini.md` |
| **22/09/2026** | Acotar el cronograma del prototipo a **4 sprints hasta mediados de diciembre de 2026** (con revisiones quincenales y demos mensuales), usar flujo simplificado en Jira y validar la métrica de negocio (**~400 h/mes** invertidas en comités vs. **90.67%** de mejora en velocidad). | `Technical Session - DevCycle team  - 2026_09_22 07_31 CST - Notas de Gemini.md` |
| **01/10/2026** | **Conservar las pestañas de supuestos, riesgos y detalle de GCP** en base de datos dentro de la hoja de costos para que la IA las utilice en la estimación de infraestructura; traducir las plantillas de Confluence (Canvas/RFS) a formatos estructurados (**JSON/XML**). | `Technical Session - DevCycle team  - 2026_10_01 07_27 CST - Notas de Gemini.md` |
| **14/10/2026** | Establecer en el **Home** los estatus *Backlog, Aprobadas, Rechazadas y Sin etapa definida*; eliminar los botones *"Ir a priorización"* y *"Ver comité"* dejando solo **"Seguimiento de portafolio"** y **"Levantar iniciativa"**; incorporar evaluación con **Pirámide y Scorecards** permitiendo modificación manual (*"dedazo"*) por emergencias; dividir la entrega de la Etapa 1 en dos partes; y fijar un **límite de 4.5 horas semanales** reduciendo juntas excesivas. | `DevCycle_ Front_ 2026_10_14 07_19 CST - Notas de Gemini.md` |
| **15/10/2026** | Extraer y estandarizar los **contratos de microservicios en JSON** para el frontend; confirmar **Figma** como herramienta de UX; alojar todas las aplicaciones en el mismo proyecto de **GCP (Cloud Run)** usando entornos *sandbox* y *prototipo*; e implementar **Infraestructura como Código con Terraform y Cloud Build** bajo **Golden Pipelines**. | `Technical Session - DevCycle team  - 2026_10_15 07_59 CST - Notas de Gemini.md` |
| **20/10/2026** | Incorporar estimación de capacidad con **Story Points** a partir del Sprint 3; formalizar todas las ideas nuevas en **Monday** por la baja de Trisquel; **cancelar el desarrollo directo de entregables para la Academia**; migrar el agente de *Quickly* a **ADK en GCP** con Confluence; agregar **preguntas contextuales automáticas en el chat de la calculadora**; y formalizar en documentos separados los **Lineamientos de Desarrollo Backend y Frontend**. | `Technical Session - DevCycle team  - 2026_10_20 07_59 CST - Notas de Gemini.md` |
| **22/10/2026** | Evitar la extracción manual desde anexos PDF y **consolidar una base centralizada de tarifas de proveedores con la BMO** (Patricia Santana), evaluando la consulta de tarifas vía servicio en **SAP**, manteniendo temporalmente una tabla de proveedores/precios en BD. | `Technical Session - DevCycle team  - 2026_10_22 08_04 CST - Notas de Gemini.md` |
| **03/11/2026** | Concluir los requerimientos de la versión **Foundation** en Monday para sustituir Trisquel; abrir el **Sprint 3 en Miro**; realizar revisión interna de cierre de sprint y **reprogramar la demostración oficial con el sponsor para los primeros días de diciembre**; y crear historia de usuario específica para seguimiento de demos por *stage*. | `Technical Session - DevCycle team  - 2026_11_03 08_02 CST - Notas de Gemini.md` |
| **05/11/2026** | Delimitar el alcance de **Foundation** (solo registro digital y trazabilidad de ideas 2027 en Monday, **sin calculadoras**) frente a **Enterprise** (flujo completo de 7 pasos, iniciando con Stage 0 Descubrimiento y Stage 1 Priorización con Pizza, Pirámide y Score); establecer **sesiones recurrentes de revisión de feedback**; y crear un **modelo de datos unificado** entre la BD y Monday. | `Technical Session - DevCycle team  - 2026_11_05 08_03 CST - Notas de Gemini.md` |
| **09/11/2026** | Lanzar a producción la versión **Foundation** en Monday; fijar el **Sprint 3 del 10 al 24 de noviembre de 2026** (ajustado por el festivo del 16 de noviembre); definir por votación el objetivo del Sprint 3 (*"Demostrar el primer incremento del producto para acelerar la toma de decisiones estratégicas sustentando la automatización de procesos y la homologación de conocimientos"*); crear un **backlog específico para pruebas (QA)**; registrar el soporte de Monday como tareas directas; y oficializar la transición de seguimiento a **Alfredo Ledezma Cruz** y el ascenso de **Dulce Valadez** a Coach de Agilidad. | `Sprint 3 Planning - DevCycle team  - 2026_11_09 15_59 CST - Notas de Gemini.md` |
| **10/11/2026** | Asignar las **pruebas funcionales** actuales al equipo de Ivonne mientras se coordina con QA central el esquema de pruebas especializadas tempranas (seguridad, IA, volumen); elaborar el **documento de lineamientos de integración** para incorporar la calculadora (*Assisti*) a la interfaz principal; alinear la estructura del Canvas contra el RFS; y confirmar el **congelamiento de actividades en diciembre de 2026** tras el último sprint para transicionar al **Equipo Escalado en enero de 2027** (capacitación el 17/12/2026). | `Technical Session - DevCycle team  - 2026_11_10 08_03 CST - Notas de Gemini.md` |

---

## 6. Estatus Actual (Sprint 3: 10 Nov – 24 Nov 2026)

- **Objetivo del Sprint 3**:
  > *"Demostrar el primer incremento del producto para acelerar la toma de decisiones estratégicas sustentando la automatización de procesos y la homologación de conocimientos."*
- **Hitos Recientes Alcanzados**:
  - **Versión *Foundation* en Producción (09/11/2026)**: Operando en Monday para la migración y captura de ideas 2027 por parte de la PMO y Business Partners antes de la baja de Trisquel.
  - **Lineamientos Técnicos y Monorepo (`devcycle-back-front`)**: Estandarización de lineamientos de Frontend y Backend, flujo de navegación y prototipos de Stage 0 y Stage 1 (Pizza, Pirámide y Scorecard).
- **Foco de Ejecución en el Sprint 3**:
  - **Frontend / UI (Javier Trejo)**: Refinamiento consensuado de la interfaz gráfica (tarea F4), atención a hallazgos de pruebas funcionales en el nuevo backlog de QA y redacción del **documento de lineamientos de integración** para la calculadora de Jonathan Romero.
  - **Backend / Data SWAT (Alejandro Miranda, Argos y equipo)**: Entrega de las 3 tareas troncales comprometidas (arquitectura, modelo de datos unificado BD/Monday y contratos de microservicios).
  - **Canvas y Agente *Quickly* (Iván Barajas, Josette Redonda)**: Alineación de la estructura de campos del Lienzo (Canvas) e identificadores contra el RFS/BRD, validación con Patricia Santana y despliegue del agente ADK en GCP / Vertex AI.
  - **Calculadora *Assisti* (Jonathan Romero)**: Integración bajo lineamientos de UI, escenarios multianuales, responsables de costos y base de conocimiento (RAG) con tarifas consolidadas de BMO.
  - **Soporte Monday (Ivonne Hernández)**: Tareas técnicas de habilitación de APIs, permisos y replicación de datos para la versión *Enterprise*, además de ejecución de pruebas funcionales.
- **Próximos Hitos de Cierre 2026 – Inicio 2027**:
  - **24 de noviembre de 2026**: Cierre del Sprint 3.
  - **Principios de diciembre de 2026**: Demostración ejecutiva del primer incremento del producto ante el sponsor (**Jorge Sánchez**).
  - **Diciembre de 2026 (Sprint 4 / Último sprint del año)**: Cierre del ciclo de prototipo, baja definitiva de Trisquel, **capacitación de Equipo Escalado (17 de diciembre de 2026 por Alfredo Ledezma)** y congelamiento de fin de año.
  - **Enero de 2027**: Reanudación y escalamiento formal del producto bajo el modelo de **Equipo Escalado**.

