sept 14, 2026

## **DevCycle**

Invitado [MIGUEL JAVIER BERMEJO GUERRERO](mailto:mjbermejog@liverpool.com.mx) [ALEJANDRO JAVIER MIRANDA DUARDO](mailto:ajmirandad@liverpool.com.mx) [ARGOS EYRA MARTINEZ ZEFERINO](mailto:aemartinezz@liverpool.com.mx) [MANUEL CHAVEZ RUIZ](mailto:mchavezr07@liverpool.com.mx) [JAVIER ENRIQUE TREJO RODRIGUEZ](mailto:jtrejor@liverpool.com.mx)

Archivos adjuntos [DevCycle](https://calendar.google.com/calendar/event?eid=NDRsZWJkdDM0bXBhYXN2aWpwNnE5NXYwOGMgYWptaXJhbmRhZEBsaXZlcnBvb2wuY29tLm14)

### **Resumen**

Revisión del flujo de proyectos con integración y priorización.

**Sincronización y registro inicial**  
Implementación de herramienta para sincronizar horas entre Jira y Monday. Se decidió utilizar un formulario estandarizado para la captura de iniciativas.

**Diseño de portafolios y visualización**  
Definición de vistas independientes por cartera de negocio. Se acordó ordenar las iniciativas mediante la posición visual en lugar de una columna numérica.

**Etapas y validación tecnológica**  
Estructuración de 4 etapas principales en el ciclo de vida del proyecto. Se estableció una cartera de pendientes para validar obligatoriamente el impacto en tecnologías de información.

### **Decisiones**

## Requiere más debate

* **Periodicidad de priorización anual y trimestral.** Se debatió la conveniencia de cambiar la priorización anual a trimestral, quedando pendiente de validación definitiva.

## Acordada

* **Uso de ramas propias para control de código.** Se estableció que los integrantes deben descargar el repositorio y subir sus cambios a su propia rama.

* **Encolamiento inicial de iniciativas sin estatus prioritario.** Se acordó que cada iniciativa nueva se encola sin estatus de prioridad hasta que se le asigne un número en el backlog.

* **Enfoque de entrega mediante diseño visual MVP.** Se acordó entregar el desarrollo actual como un MVP enfocado inicialmente en el diseño visual.

* **Construcción inicial de la vista completa general.** Se acordó construir primero la vista completa del sistema para posteriormente ajustarla a cada perfil.

* **Implementación del correo electrónico para solicitantes** Se acordó modificar el formulario de iniciativas para registrar tanto al solicitante como al sponsor mediante su correo electrónico corporativo.

* **Eliminación del campo de dependencias arquitectónicas** Se decidió remover la sección de referencias y dependencias de arquitectura del formulario para evitar generar ruido e confusión.

* **Eliminación de la columna explícita de prioridad** Se acordó retirar la columna explícita de prioridad y definir el orden de las iniciativas según su posición visual determinada por el portafolio manager.

### **Próximos pasos**

- [ ] \[Argos Eyra Martinez Zeferino\] Entregar lista proyectos: Proporcionar los proyectos asignados para el registro de horas en la aplicación.

- [ ] \[Argos Eyra Martinez Zeferino\] Añadir notas diagrama: Incluir notas en el tablero de Miro para los procedimientos de proyectos no prioritarios.

- [ ] \[El grupo\] Solicitar reglas priorización: Obtener las normas internas de cada dirección para organizar las tareas. Gestionar la solicitud de estas políticas de trabajo.

- [ ] \[Argos Eyra Martinez Zeferino\] Pedir documento Canvas: Solicitar el documento necesario para el llenado de ideas y especificaciones del proyecto.

- [ ] \[Argos Eyra Martinez Zeferino\] Marcar desconocidos diagrama: Señalar en el diagrama los puntos donde falta claridad sobre el flujo de completado. Utilizar un color diferenciado para estas áreas.

- [ ] \[The group\] Notificar cambios prioridad: Notificar siempre a los gerentes de portafolio, gerentes de proyecto y gerentes de relaciones de negocio sobre cambios en la prioridad de los proyectos mediante correo electrónico y chat.

- [ ] \[The group\] Definir beneficios: Definir los tipos de beneficios cuantificables, sus fórmulas de cálculo y los inputs requeridos para la captura de iniciativas.

- [ ] \[The group\] Construir vista portafolio: Construir la vista completa del portafolio en la herramienta y posteriormente realizar los ajustes necesarios según el perfil de cada usuario.

- [ ] \[The group\] Ajustar formulario registro: Ajustar el formulario de registro de iniciativas en Monday para incluir el correo electrónico del solicitante en lugar de su nombre y añadir un campo de búsqueda para sistemas y plataformas.

- [ ] \[The group\] Limpiar campos formulario: Eliminar el campo de presupuesto y la fecha objetivo del formulario de registro de iniciativas para evitar ruido en la gestión inicial.

- [ ] \[The group\] Definir etapa backlock: Incluir una etapa de backlock inicial en el flujo del sistema donde se deba validar si el proyecto requiere intervención de TI.

- [ ] \[El grupo\] Actualizar pantalla backlog: Incluir validaciones para sistemas afectados y el impacto de TI en la pantalla de backlog. Habilitar la confirmación de estas secciones como parte del flujo de trabajo.

- [ ] \[El grupo\] Agregar confirmación total: Implementar un botón de confirmar todo dentro de la interfaz. Configurar el sistema para que regrese al backlog una vez realizada la confirmación.

- [ ] \[El grupo\] Definir pantallas adicionales: Crear las dos pantallas adicionales necesarias para la gestión de estados. Asegurar que estas interfaces permitan la navegación según lo discutido.

### **Detalles**

* **Herramienta de sincronización de horas entre Jira y Monday**: ARGOS EYRA MARTINEZ ZEFERINO (El man) explica el desarrollo de una aplicación propuesta por Omar para sincronizar las horas de los proyectos directamente entre Jira y Monday, evitando que los equipos tengan que duplicar tareas y registrar horas manualmente en Triskel de manera ineficiente. MIGUEL JAVIER BERMEJO GUERRERO menciona que actualmente cargan sus horas diarias en un solo proyecto llamado Datamesh en lugar de dividirlas por cada tarea específica. La decisión es implementar esta solución para simplificar el reporte de actividades y horas del equipo.

* **Configuración del repositorio de código**: MIGUEL JAVIER BERMEJO GUERRERO informa que ya logró acceder al repositorio de Javi Trejo, pero consulta la estrategia operativa sobre si debe clonar y crear una rama propia o trabajar directamente. ARGOS EYRA MARTINEZ ZEFERINO (El man) indica la instrucción de descargar el repositorio y subir los cambios a una rama personal.

* **Revisión inicial del diagrama de flujo y validación de tecnología**: ARGOS EYRA MARTINEZ ZEFERINO (El man) y MIGUEL JAVIER BERMEJO GUERRERO revisan el diagrama en Miro sobre el flujo de proyectos. Se analiza que tras registrar una iniciativa, esta pasa al PMO (portafolio manager), quien valida si requiere la participación del equipo de tecnología (TI); si no la requiere, el flujo se descarta por esa vía, y si la requiere, se procede a su priorización. Se debate que este filtro debe garantizarse desde el llenado del formulario inicial.

* **Reglas de negocio y periodicidad de priorización por dirección**: ARGOS EYRA MARTINEZ ZEFERINO (El man) señala que la priorización de proyectos se realiza bajo diferentes periodos según la dirección: anual para digital, tecnología, transformación y construcción; trimestral para negocios financieros. Se discute la problemática de tener que esperar hasta un año para priorizar proyectos en áreas como digital, lo cual genera fricción y dudas sobre la agilidad del proceso. Se plantea la necesidad de revisar si estas frecuencias anuales son funcionales o si deberían ajustarse a esquemas trimestrales.

* **Gestión de proyectos pequeños y mejora continua**: ARGOS EYRA MARTINEZ ZEFERINO (El man) y MIGUEL JAVIER BERMEJO GUERRERO debaten sobre cómo manejar los proyectos pequeños o mejoras continuas (como la automatización de archivos en Excel), los cuales a menudo evaden los canales formales debido a su urgencia. Se discute la necesidad de distinguir entre iniciativas nuevas y mejoras existentes, concluyendo que independientemente de su tamaño, consumen recursos de el equipo, por lo que el portafolio manager debe evaluar su costo y beneficio real en comparación con proyectos grandes.

* **Diseño del visualizador y visibilidad de impactos en el backlog**: ARGOS EYRA MARTINEZ ZEFERINO (El man) propone un visualizador por cartera de negocio donde se muestren los proyectos encolados y no priorizados, ordenados por fecha u orden de entrada. Se explica que al mover y subir de posición un proyecto en la lista, esto afectará a otros proyectos que ya se encuentran en fases de ejecución o discovery, brindando visibilidad sobre las repercusiones de integrar nuevas iniciativas.

* **Mecánica de priorización numérica y control de desplazamientos**: ARGOS EYRA MARTINEZ ZEFERINO (El man) y MIGUEL JAVIER BERMEJO GUERRERO discuten las dificultades de permitir que los solicitantes asignen prioridades numéricas sin generar conflictos o duplicidades en listas extensas. Se acuerda que las iniciativas ingresan inicialmente en una cola sin estatus de prioridad, y al asignarles una posición numérica, el sistema emitirá alertas indicando cuántos proyectos se desplazarán, permitiendo a la persona responsable evaluar el impacto antes de confirmar.

* **Formalización del backlog y notificaciones automáticas**: ARGOS EYRA MARTINEZ ZEFERINO (El man) detalla que tras realizar los movimientos de priorización, existirá un botón para formalizar y guardar los cambios. El sistema enviará automáticamente notificaciones por correo electrónico y mensajes de Google Chat a los portafolios managers (PMO), BRMs (Business Requirements Managers), vicepresidentes y a la persona funcional solicitante, asegurando transparencia y manteniendo un historial de modificaciones.

* **Ampliación de involucrados en el registro de solicitudes**: ARGOS EYRA MARTINEZ ZEFERINO (El man) propone que el formulario de solicitud no registre únicamente a la persona que levanta el ticket, sino que permita agregar múltiples correos de otras personas interesadas del área de negocio, para que todas reciban las notificaciones de priorización y actualizaciones.

* **Llenado del Canvas de ideas y revisión de calidad**: ARGOS EYRA MARTINEZ ZEFERINO (El man) explica el siguiente paso del flujo, donde la persona funcional que solicita el proyecto interactúa con un agente virtual para responder preguntas y construir el canvas de la iniciativa (integrando descripción, beneficios, capacidades y alineación estratégica). Posteriormente, el BRM realiza una revisión de calidad del canvas para verificar que la información esté correcta y completa.

* **Clarificación de roles organizacionales: BRM, Portfolio Manager y Project Manager**: MIGUEL JAVIER BERMEJO GUERRERO solicita aclarar los roles dentro del proceso, y ARGOS EYRA MARTINEZ ZEFERINO (El man) explica que el BRM (Business Requirements Manager, como Clemente) posee el contexto completo del negocio y actúa como el principal vínculo con tecnología. El portafolio manager opera a nivel de dirección ejecutiva gestionando carteras de proyectos y definiendo prioridades, diferenciándose del project manager que gestiona proyectos individuales.

* **Desarrollo del Producto Mínimo Viable (MVP) y vistas independientes por cartera**: ARGOS EYRA MARTINEZ ZEFERINO (El man) y MIGUEL JAVIER BERMEJO GUERRERO conversan sobre enfocar los esfuerzos actuales en construir el diseño visual del Producto Mínimo Viable para este flujo inicial. Asimismo, se acuerda que la interfaz debe permitir filtrar y visualizar las carteras de negocio de forma independiente (como digital, plataforma o negocios financieros) según el perfil del portafolio manager.

* **Captura inicial de iniciativas en Monday y reglas de negocio**: El problema central radica en cómo estandarizar la captura de ideas de proyectos para que lleguen al registro general (\*backlog\*) de cada oficina de gestión de proyectos con reglas de negocio claras. ARGOS EYRA MARTINEZ ZEFERINO (El man) propuso utilizar un formulario estandarizado en la plataforma Monday para capturar variables como beneficios cuantificados y monetizados, descripción de necesidades, unidad de negocio, impacto en tecnologías de información y referencias de sistemas, basándose en un concepto de tipo \*blueprint\*. Como decisión, se acordó implementar esta primera etapa mediante el formulario mencionado para estructurar adecuadamente la información de entrada.

* **Diseño de la vista de portafolio y formulario de registro**: Se discutió el problema de cómo visualizar las carteras de proyectos y registrar nuevas iniciativas de manera clara. ARGOS EYRA MARTINEZ ZEFERINO (El man) presentó la interfaz actual del portafolio con el estado de cada iniciativa y mostró el formulario de registro que solicita título, unidad de negocio, solicitante y descripción de necesidad. Surgió un debate sobre si el solicitante debía registrarse mediante nombre o correo corporativo, donde se concluyó que el registro debe realizarse a través del correo electrónico para mantener la consistencia con el patrocinador (\*sponsor\*). Asimismo, ARGOS EYRA MARTINEZ ZEFERINO (El man) sugirió integrar un asistente de chat en la interfaz para ayudar a redactar la descripción de la necesidad, lo cual fue aceptado como parte del diseño del formulario.

* **Validación del impacto en tecnologías de información y referencias de arquitectura**: El problema analizado fue cómo registrar de forma adecuada el impacto tecnológico y las dependencias arquitectónicas de una iniciativa sin generar confusión en las personas solicitantes. ARGOS EYRA MARTINEZ ZEFERINO (El man) planteó incluir preguntas sobre si se requiere equipo de tecnologías de información y campos de texto para buscar sistemas o plataformas impactadas. Aunque inicialmente se consideró incluir un campo de referencias de arquitectura y dependencias previas, ARGOS EYRA MARTINEZ ZEFERINO (El man) propuso eliminarlo para evitar generar ruido técnico innecesario a los solicitantes, y el grupo acordó suprimir dicha sección.

* **Definición de tipos de beneficios y cálculo en las iniciativas**: Se abordó el problema de cómo cuantificar los beneficios esperados de un proyecto (como eficiencia en horas hombre, nuevos ingresos, ahorros directos, reducción de tiempos, mitigación de riesgos y cumplimiento). ARGOS EYRA MARTINEZ ZEFERINO (El man) explicó que cada tipo de beneficio requiere reglas de cálculo y fórmulas específicas similares a los objetivos clave de rendimiento. Se identificó que faltaba información detallada proporcionada por las áreas correspondientes sobre las fórmulas de cálculo, por lo que se acordó definir los insumos necesarios y adaptar el sistema para que solicite métricas de éxito clave y datos cuantificables según el tipo de beneficio elegido.

* **Visualización del inicio, portafolios y filtros por unidad de negocio**: El problema consistía en determinar cómo las personas usuarias visualizan el estado de sus proyectos tras el envío y cómo las personas administradoras gestionan el portafolio general. ARGOS EYRA MARTINEZ ZEFERINO (El man) propuso renombrar la pestaña de portafolio a inicio para que cada persona usuaria vea las iniciativas que registró, y habilitar un menú de gestión de portafolio con filtros específicos por dirección de negocios. Se discutió si los portafolios debían mostrarse mezclados o prefiltrados, decidiéndose que cada administrador o administradora de portafolio pueda seleccionar exclusivamente su cartera correspondiente mediante filtros para evitar la mezcla de iniciativas entre diferentes áreas.

* **Estructuración de etapas y estados de los proyectos**: Se debatió el problema de cómo estructurar correctamente las etapas del ciclo de vida del proyecto (como priorización, definición, estimación y ejecución) y sus estados asociados (por iniciar, en curso, finalizado, atrasado) sin sobrecargar la interfaz. ARGOS EYRA MARTINEZ ZEFERINO (El man) y MIGUEL JAVIER BERMEJO GUERRERO analizaron las discrepancias entre etapa y estado, donde MIGUEL JAVIER BERMEJO GUERRERO sugirió un estado inicial de creado. Tras una discusión detallada sobre flujos separados de creación y avance, se acordó simplificar el modelo a cuatro etapas principales (definición de proyecto, estimación de proyecto, ejecución del proyecto y cierre) combinadas con cuatro estados estándar (por iniciar, en curso, finalizado y atrasado), eliminando sub-ramas complejas para mantener una vista ejecutiva clara.

* **Discusión sobre la columna de prioridad y el ordenamiento visual**: El problema evaluado fue si se debía mantener una columna explícita de prioridad numérica o si la prioridad debía deducirse por la posición visual en el sistema. MIGUEL JAVIER BERMEJO GUERRERO preguntó si la columna de prioridad podía ser útil para la oficina de gestión de proyectos. ARGOS EYRA MARTINEZ ZEFERINO (El man) argumentó que dicha columna genera ruido y confusión cuando múltiples iniciativas tienen la misma prioridad alta, proponiendo en su lugar que la prioridad esté determinada estrictamente por la posición visual vertical en la lista gestionada por el administrador de portafolio. Como conclusión, se acordó eliminar la columna explícita de prioridad y basar el orden de atención en la ubicación dentro del portafolio.

* **Configuración de la etapa de cartera de pendientes y confirmación de sistemas afectados**: El problema final consistió en definir el flujo previo a la priorización para validar formalmente el impacto tecnológico de cada iniciativa. ARGOS EYRA MARTINEZ ZEFERINO (El man) propuso agregar una etapa inicial denominada cartera de pendientes (\*backlog\*), donde se debe confirmar obligatoriamente si el proyecto tiene impacto en tecnologías de información y verificar los sistemas afectados antes de pasar a la priorización. Se acordó diseñar una pantalla específica dentro de esta etapa donde el administrador pueda confirmar los sistemas afectados y el impacto tecnológico mediante un botón de confirmación que devuelva la iniciativa al flujo general.

*Revisa las notas de Gemini para asegurarte de que sean precisas. [Obtén sugerencias y descubre cómo Gemini toma notas](https://support.google.com/meet/answer/14754931)*

*Cómo es la calidad de **estas notas específicas?** [Responde una breve encuesta](https://google.qualtrics.com/jfe/form/SV_5bXzKQfylMIhSXc?confid=nrWcIByI0lJFmOtTQeQrDxIYOBEBMgUIigIgABgBCA&detailLevel=standard&hasImages=False&entryPoint=footerMain&isGoogler=False) para darnos tu opinión; por ejemplo, cuán útiles te resultaron las notas.*