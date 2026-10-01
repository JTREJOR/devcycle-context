# DevCycle Automatization — Contexto y Estado del Proyecto

Documento de referencia y resumen ejecutivo del proyecto **DevCycle Automatization** (Liverpool), consolidado a partir de las minutas y sesiones técnicas del equipo (agosto - septiembre 2026).

> Se puede consultar el repositorio de la aplicación en este enlace: [JTREJOR/devcycle-back-front](https://github.com/JTREJOR/devcycle-back-front).

---

## 1. Visión General del Proyecto

### ¿Qué es DevCycle?
**DevCycle Automatization** es una iniciativa estratégica para unificar, acelerar y automatizar el ciclo de vida completo de iniciativas tecnológicas en Liverpool:
1. **Intake / Discovery**: Registro estandarizado y asistido de ideas y proyectos.
2. **Validación y Priorización de Portafolio**: Filtrado de impacto tecnológico y ordenamiento dinámico por cartera de negocio.
3. **Estimación Asistida con Inteligencia Artificial**: Generación de canvas, dimensionamiento (sizing) y hojas de costos preliminares.
4. **Comités y Formalización**: Aprobaciones de líderes de arquitectura, técnicos y Business Partners (BP/BRM), reduciendo comités presenciales.
5. **Gestión de Capacidad y Sincronización**: Enlace automático entre Jira (ejecución técnica) y Monday (visibilidad directiva/portafolio), facilitando la salida de Trisquel (diciembre 2026).

### Justificación e Impacto
- **Problema**: Los comités semanales y la elaboración manual de charters y hojas de costo consumen ~400 horas hombre al mes.
- **Meta**: Automatizar el **90.67%** del flujo operativo, liberando **~304 horas al mes**.
- **Esquema**: Prototipo de innovación (MVP financiado por innovación) con roadmap a 4 sprints concluyendo a mediados de diciembre de 2026, para luego transicionar a proyecto formal.

---

## 2. Participantes y Gobernanza

- **Patrocinador Principal (Sponsor)**: Jorge Sánchez.
- **Stakeholders clave / Directivos**: Omar, Clemente (BRM), César Guzmán, Alexis Labrada (PMO / Monday).
- **Financiamiento Prototipo**: Itzana Jiménez Chavero.
- **Product Owner / Facilitación / Metodología**: Daniel Uribe.
- **Portafolio / Intake / Monday**: Ivonne Hernández Castellanos, Belén Romero, Josefina Luna, Mafer Torres.
- **Equipo Técnico / IA / Backend / Sincronización**: Argos Eyra Martínez Zeferino ("El man"), Jonathan Romero, Iván Barajas, Miguel Bermejo, Brian Hernández, Erick Soria, J. Inés Almazán.
- **Líder Frontend**: **Javier Enrique Trejo Rodríguez**.
- **UX / Diseño de Interfaz / Librerías**: Gustavo Vargas, Cassandra.

---

## 3. Arquitectura Funcional por Tracks

```text
[ 1. Intake / Discovery ] 
       │ (Registro con brief asistido por IA, ROI y validación TI)
       ▼
[ 2. Cartera de Pendientes & Priorización ] 
       │ (Validación de impacto TI, visualización por cartera, drag & drop)
       ▼
[ 3. Canvas & Estimaciones Asistidas (IA) ] 
       │ (Gemini + NextJS + Calculadora Building API GCP, preguntas sizing)
       ▼
[ 4. Validación Técnica y Arquitectura ] 
       │ (VoBo simultáneo de Líder Técnico y Arquitecto, refinamiento)
       ▼
[ 5. Formalización & Sincronización ]
         (Generación de Charter/Hoja de costos, sincronización Jira <-> Monday)
```

---

## 4. Estado y Especificaciones para "El Front" (Frontend)

El frontend es la cara visible que integra los diferentes tracks en una experiencia unificada de usuario.

### 4.1. Alcance del MVP Visual
El desarrollo actual del frontend está enfocado en entregar un **MVP visual funcional** con datos de prueba (*mock*) que demuestre el flujo completo punta a punta.

### 4.2. Módulos y Pantallas Clave a Construir

1. **Pantalla de Inicio / Mis Iniciativas**:
   - Resumen ejecutivo de las iniciativas registradas por el usuario autenticado.
   - Indicador de estado (Por iniciar, En curso, Finalizado, Atrasado) y etapa actual (Definición, Estimación, Ejecución, Cierre).

2. **Formulario de Registro / Intake & Discovery**:
   - **Campos principales**: Título, Unidad de Negocio (Digital, EPL, Negocios Financieros, Tecnología, etc.), Solicitante (correo corporativo), Sponsor (correo corporativo).
   - **Asistente Virtual (Chat IA)**: Widget/chat flotante o lateral para ayudar al usuario a redactar y estructurar la descripción de la necesidad.
   - **Impacto Tecnológico**: Confirmación de si requiere TI y buscador de sistemas/plataformas afectadas.
   - **Beneficios y ROI**: Selección de tipo de beneficio (ahorros directos, horas hombre, nuevos ingresos, KPIs) con sus inputs y cálculos correspondientes.
   - *Campos eliminados deliberadamente para no generar ruido*: Presupuesto manual, dependencias arquitectónicas y fecha objetivo.

3. **Bandeja de Cartera de Pendientes & Portafolio (Backlog)**:
   - **Filtros por Dirección/Cartera**: Visualización independiente para cada Portfolio Manager (evitando mezcla de carteras).
   - **Priorización Visual (Drag & Drop)**: Ordenamiento vertical por arrastre (tipo Jira), eliminando campos numéricos manuales de prioridad.
   - **Alertas de Desplazamiento**: Al mover una iniciativa de orden, notificar cuántas iniciativas se desplazan.
   - **Botón de Confirmar / Formalizar**: Guarda el orden de prioridades y gatilla notificaciones automáticas.

4. **Vistas de Estimación, Canvas y Aprobación**:
   - Interfaz con el agente de IA para responder preguntas de dimensionamiento (*sizing*: tráfico mensual, transacciones, infraestructura).
   - Visualización preliminar del Canvas y desglose de hoja de costos.
   - Flujo de doble validación (Líder Técnico + Líder de Arquitectura) con acción de "Refinar estimación" en caso de observaciones.

### 4.3. Lineamientos Técnicos y UX
- **Ecosistema**: React / Next.js.
- **Componentes y Diseño**: Alinear con las librerías de estilos y componentes desarrolladas por el equipo de **Gus Vargas** y las directrices de UX de **Cassandra**, asegurando identidad visual Liverpool y consistencia para posible embebido/integración en **Monday**.
- **Gestión de Código**: Trabajo en ramas propias para control de versiones y pull requests hacia la rama principal.

---

## 5. Estatus Actual (Sprint 21 Sep - 02 Oct)

- **Objetivo del Sprint**:
  - Refinar el prototipo visual / mockup del **Paso 1 (Levantamiento y Priorización de iniciativas)**.
  - Sesión de alineación de estándares visuales con Cassandra (UX).
  - Integrar las validaciones de impacto en TI y sistemas afectados en la vista de backlog.
- **Cadencia**: Sprints de 2 semanas, revisiones quincenales y demostraciones mensuales hacia stakeholders clave. Cierre de prototipo estimado a mediados de diciembre 2026.
