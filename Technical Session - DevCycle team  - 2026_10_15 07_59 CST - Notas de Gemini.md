oct 15, 2026

## **Technical Session \- DevCycle team** 

Invitado [Maria Fernanda Torres (Mafer)](mailto:mftorresp@liverpool.com.mx) [JONATHAN JESUS ROMERO TORRECILLA](mailto:jjromerot@liverpool.com.mx) [IVONNE ANAYELLI HERNANDEZ CASTELLANOS](mailto:iahernandezc@liverpool.com.mx) [JOSETTE REDONDA ALVA](mailto:jiredondaa@liverpool.com.mx) [Dulce Kesia Valadez Guzman](mailto:dulce.valadez@qualtop.com) [ANDRES BELENDEZ SALDAÑA](mailto:abelendezs@liverpool.com.mx) [BRIAN HERNANDEZ GARCIA](mailto:bhernandeg01@liverpool.com.mx) [LUZ VANESSA BECERRA RIVERA](mailto:lvbecerrar@liverpool.com.mx) [ERICK IVAN SORIA MORALES](mailto:eisoriam@liverpool.com.mx) [JORGE ALBERTO OZUNA CRUZ](mailto:jaozunac@liverpool.com.mx) [IVÁN BARAJAS MUÑOZ](mailto:jibarajasm@liverpool.com.mx) [JAVIER ENRIQUE TREJO RODRIGUEZ](mailto:jtrejor@liverpool.com.mx) [JOSEFINA LUNA](mailto:jlunac@liverpool.com.mx) [Itzana Jiménez Chavero](mailto:ijimenezc02@liverpool.com.mx) [J. INES ALMAZAN VALERIO](mailto:jialmazanv@liverpool.com.mx) [ADRIANA HERNANDEZ PARRA](mailto:ahernandep13@liverpool.com.mx) [BELEN ROMERO ARZATE](mailto:bromeroa01@liverpool.com.mx) [ARGOS EYRA MARTINEZ ZEFERINO](mailto:aemartinezz@liverpool.com.mx) [DULCE KESIA VALADEZ GUZMAN](mailto:dkvaladezg@liverpool.com.mx) ~~[ELODIA MORENO](mailto:ecmorenoh@liverpool.com.mx)~~ ~~[Daniel Uribe](mailto:edhernandezu@liverpool.com.mx)~~ ~~[ALEJANDRO JAVIER MIRANDA DUARDO](mailto:ajmirandad@liverpool.com.mx)~~

Archivos adjuntos [Technical Session - DevCycle team ](https://calendar.google.com/calendar/event?eid=Z2k2NGF1aGhrdXNpMmtyYms1b3Q5MHI0bmFfMjAyNjEwMTVUMTQwMDAwWiBhaGVybmFuZGVwMTNAbGl2ZXJwb29sLmNvbS5teA) [Technical Session - DevCycle team  - 2026/09/02 06:55 CST - Recording](https://drive.google.com/file/d/1vjWfQbQz_MJF_EjGJoKnQHpl2LdVOwGt/view?usp=drive_web) [Notas de Gemini](https://docs.google.com/document/d/1LNel3sJ0-DRC456mxJoF9o2SmS3jOJbF4mKdKXfF9Lo/edit?usp=meet_tnfm_calendar) [Notas de Gemini](https://docs.google.com/document/d/1OibJ5WDlDCJ8WQYb216uF05P7b9CjareY8nA21EVf4Y/edit?usp=meet_tnfm_calendar)

Registros de la reunión [Grabación](https://drive.google.com/file/d/1_Yd0EzRIQhP2fzkjkasqWsSSzmMtLxOx/view?usp=drive_web) 

### **Resumen**

Definición de navegación, reestructuración de equipos y optimización de arquitectura técnica vía sprints.

**Refinamiento de navegación y microservicios**  
Prototipos de navegación del paso cero definidos en paralelo. Contratos de microservicios establecidos con JSON.

**Reducción de reuniones y desarrollo**  
Juntas semanales reducidas para optimizar la ejecución. Figma confirmado como herramienta para experiencia de usuario.

**Infraestructura en Google Cloud**  
Aplicaciones alojadas en Google Cloud Platform mediante Cloud Run. Terraform utilizado para infraestructura como código.

### **Decisiones**

## Acordada

* **Definición de contratos para microservicios** El equipo extraerá todos los contratos y definiciones de microservicios durante el sprint actual para su integración en el frontend.

* **Estructura de repositorios separados para backend y frontend** Se utilizará un repositorio independiente para el backend y otro para el frontend trabajando con distintas ramas.

* **Optimización y reducción de sesiones de equipo** Se reducirán y ajustarán las reuniones recurrentes para priorizar el tiempo de ejecución del equipo de desarrollo.

* **Configuración de proyectos en GCP mediante sandbox y prototipo** Las aplicaciones operarán en el mismo proyecto de GCP empleando entornos sandbox para pruebas y prototipos para producción.

* **Implementación de infraestructura como código con Terraform** Se creará la infraestructura como código utilizando Terraform en alineación con los Golden Pipelines.

### **Próximos pasos**

- [ ] \[El equipo\] Definir contratos: Definir los contratos de todos los microservicios necesarios para la integración con el frontend.

- [ ] \[Alguien en Dirección Ejecutiva TI (Mario Pani \- Edif. C, PB)\] Crear repositorios: Crear el repositorio para el backend y el repositorio para el frontend.

- [ ] \[ANDRES BELENDEZ SALDAÑA\] Acceder a proyectos: Solicitar el acceso al proyecto de infraestructura y al repositorio de GitHub.

- [ ] \[Iván\] Subir historias: Subir las historias al backlog para el siguiente sprint.

- [ ] \[ANDRES BELENDEZ SALDAÑA\] Diseñar arquitectura: Diseñar la solución de arquitectura que contemple todas las aplicaciones.

- [ ] \[Alguien en Dirección Ejecutiva TI (Mario Pani \- Edif. C, PB)\] Compartir diagrama: Enviar el diagrama base de arquitectura a Andrés para su revisión.

- [ ] \[ANDRES BELENDEZ SALDAÑA\] Alinear infraestructura: Alinear la estrategia de infraestructura y Golden Pipelines con el equipo de infraestructura.

- [ ] \[El equipo\] Compartir estilos: Compartir las hojas de estilo o URL de referencia para el diseño del frontend.

### **Detalles**

**Refinamiento de la navegación del paso cero y contratos de microservicios**: alguien en Dirección Ejecutiva TI (Mario Pani \- Edif. C, PB) explicó que el equipo de frontend, compuesto por tres integrantes, trabaja en los prototipos de navegación para el paso cero sin crear aún microservicios ni integraciones. El objetivo para este sprint es definir los contratos y microservicios necesarios para conectarlos al frontend. Marianita sumará un recurso para apoyar con los formularios del proceso de admisión. La definición de contratos incluye ejemplos de respuestas en formato JSON, parámetros de entrada, tipos de valores y tipos de invocación (GET, POST). Este trabajo de arquitectura y definición de microservicios se realizará en paralelo durante el sprint, excluyendo la calculadora por pertenecer al paso uno.

---

**Reestructuración de equipos y mapeo de microservicios**: alguien en Dirección Ejecutiva TI (Mario Pani \- Edif. C, PB) indicó que, debido a cambios en los entregables, su célula ya no materializará dicho entregable y sus integrantes se sumarán a otros equipos. El equipo trabaja en la lista y funcionamiento de los microservicios necesarios, como el de roles y usuarios. Alguien en Dirección Ejecutiva TI (Mario Pani \- Edif. C, PB) se llevó la tarea de solicitar un repositorio para el backend y otro para el frontend, gestionando el proyecto a través del presupuesto de innovación.

---

**Reducción de reuniones y optimización de la agenda**: alguien en Dirección Ejecutiva TI (Mario Pani \- Edif. C, PB) expuso una petición del equipo para reducir el tiempo en reuniones, ya que tienen una dedicación de 4.5 horas semanales, pero la semana pasada consumieron casi 5 horas en juntas, afectando la ejecución. Alguien en Dirección Ejecutiva TI (Mario Pani \- Edif. C, PB) propuso optimizar las sesiones de estatus limitando la asistencia a personas clave como Javi y eliminar reuniones redundantes como las de los lunes y jueves sobre alcances de gira. Las sesiones fijas de los martes y jueves de 8:00 a 9:00 AM enviadas por Andre se mantendrán como espacios reservados para refinamientos, mientras que las sesiones técnicas se realizarán a petición.

---

**Lineamientos de desarrollo y diseño en Figma**: alguien en Dirección Ejecutiva TI (Mario Pani \- Edif. C, PB) confirmó que los lineamientos de desarrollo y la definición de experiencia de usuario están comprometidos para este sprint, utilizando tecnologías como React y TurboPack. JAVIER ENRIQUE TREJO RODRIGUEZ confirmó que Figma es la herramienta utilizada para el diseño de experiencia de usuario, la cual será certificada por el equipo. Alguien en Dirección Ejecutiva TI (Mario Pani \- Edif. C, PB) aclaró la diferencia entre el prototipo de la aplicación Monday (identificada visualmente por tonos rosados) y la interfaz frontend final de Argos, y JAVIER ENRIQUE TREJO RODRIGUEZ compartió por chat un diagrama y audio de trabajo para coordinar con CAS.

---

**Recorrido y modularización de pantallas de Argos**: alguien en Dirección Ejecutiva TI (Mario Pani \- Edif. C, PB) revisó la interfaz frontend modularizada mediante habilidades de Vercel. La vista principal muestra proyectos según la participación de cada usuario (por ejemplo, los administradores de portafolio visualizan todos los proyectos) y pestañas para elementos en la lista de pendientes (backlog), aprobados, rechazados o por definir. Las personas usuarias pueden consultar proyectos o generar nuevas iniciativas mediante un formulario estandarizado que retorna a la vista principal. El portafolio permite gestionar prioridades a través de etapas como priorización, estimación, autorización, formalización, ejecución y cierre. Asimismo, se contemplan evaluaciones mediante pirámide y un ciclo de refinamiento de lienzos (canvas) con vicepresidentes antes de regresar a la vista principal. Estos puntos de navegación se convertirán en microservicios durante el siguiente sprint.

---

**Planificación del sprint y asignación de tareas**: alguien en Dirección Ejecutiva TI (Mario Pani \- Edif. C, PB) estableció las fechas del próximo sprint del 19 al 30\. John se concentrará en las conexiones de generación aumentada por recuperación (RAG), la optimización de bases de conocimiento y el refinamiento de respuestas. Ivón tomará las historias correspondientes para el equipo de datos y las subirá a la lista de pendientes (backlog). Se aclaró que las etiquetas F1, F2 y F3 corresponden a clasificaciones internas, donde F3 denota los lineamientos de desarrollo.

---

**Arquitectura, infraestructura en Google Cloud y Terraform**: ANDRES BELENDEZ SALDAÑA participó para revisar el diseño de solución, señalando que existe un borrador para Assisti y que se debe integrar la arquitectura del programa Argos. Alguien en Dirección Ejecutiva TI (Mario Pani \- Edif. C, PB) y ANDRES BELENDEZ SALDAÑA discutieron alojar las aplicaciones en el mismo proyecto de Google Cloud Platform (GCP) para compartir comunicación mediante Cloud Run, manteniendo el uso de Firebase Firestore y Gemini. Evaluaron el uso de entornos de pruebas (sandbox) y entornos prototipo para componentes listos para producción que requieren tickets. ANDRES BELENDEZ SALDAÑA explicó la implementación de infraestructura como código utilizando Terraform y Google Cloud Build, alineándose con las tuberías estandarizadas (Golden Pipelines) de Diego Eulogio. ANDRES BELENDEZ SALDAÑA acordó colaborar en las sesiones de arquitectura a partir del martes siguiente.

---

**Accesos a repositorios y organización de espacios**: alguien en Dirección Ejecutiva TI (Mario Pani \- Edif. C, PB) solicitó correos electrónicos para integrar a perfiles como Kevin Solano a los equipos de GitHub y coordinar las vistas del gestor de capacidad con el equipo pertinente. Se confirmaron las reservas de salas en las ubicaciones de Quad y Pani para las sesiones de arquitectura. JOSETTE REDONDA ALVA indicó que al ser Iván la persona técnica del equipo, JOSETTE REDONDA ALVA no requiere acceso al repositorio de GitHub, mientras que alguien en Dirección Ejecutiva TI (Mario Pani \- Edif. C, PB) solicitó accesos al proyecto y repositorio a ANDRES BELENDEZ SALDAÑA.

*Revisa las notas de Gemini para asegurarte de que sean precisas. [Obtén sugerencias y descubre cómo Gemini toma notas](https://support.google.com/meet/answer/14754931)*

*Cómo es la calidad de **estas notas específicas?** [Responde una breve encuesta](https://google.qualtrics.com/jfe/form/SV_5bXzKQfylMIhSXc?confid=N7b9U5xKCwzTCz0EJP30DxISOBEQAjIGCIoCIAAYAQg&detailLevel=standard&hasImages=False&entryPoint=footerMain&isGoogler=False&lang=es-US) para darnos tu opinión; por ejemplo, cuán útiles te resultaron las notas.*