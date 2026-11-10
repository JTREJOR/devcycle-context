oct 22, 2026

## **Technical Session \- DevCycle team** 

Invitado [Maria Fernanda Torres (Mafer)](mailto:mftorresp@liverpool.com.mx) [JONATHAN JESUS ROMERO TORRECILLA](mailto:jjromerot@liverpool.com.mx) [IVONNE ANAYELLI HERNANDEZ CASTELLANOS](mailto:iahernandezc@liverpool.com.mx) [JOSETTE REDONDA ALVA](mailto:jiredondaa@liverpool.com.mx) [ELODIA MORENO](mailto:ecmorenoh@liverpool.com.mx) [Dulce Kesia Valadez Guzman](mailto:dulce.valadez@qualtop.com) [ANDRES BELENDEZ SALDAÑA](mailto:abelendezs@liverpool.com.mx) [LUZ VANESSA BECERRA RIVERA](mailto:lvbecerrar@liverpool.com.mx) [ERICK IVAN SORIA MORALES](mailto:eisoriam@liverpool.com.mx) [JORGE ALBERTO OZUNA CRUZ](mailto:jaozunac@liverpool.com.mx) [IVÁN BARAJAS MUÑOZ](mailto:jibarajasm@liverpool.com.mx) [JAVIER ENRIQUE TREJO RODRIGUEZ](mailto:jtrejor@liverpool.com.mx) [Daniel Uribe](mailto:edhernandezu@liverpool.com.mx) [JOSEFINA LUNA](mailto:jlunac@liverpool.com.mx) [ALEJANDRO JAVIER MIRANDA DUARDO](mailto:ajmirandad@liverpool.com.mx) [Itzana Jiménez Chavero](mailto:ijimenezc02@liverpool.com.mx) [J. INES ALMAZAN VALERIO](mailto:jialmazanv@liverpool.com.mx) [ADRIANA HERNANDEZ PARRA](mailto:ahernandep13@liverpool.com.mx) [BELEN ROMERO ARZATE](mailto:bromeroa01@liverpool.com.mx) [ARGOS EYRA MARTINEZ ZEFERINO](mailto:aemartinezz@liverpool.com.mx) [DULCE KESIA VALADEZ GUZMAN](mailto:dkvaladezg@liverpool.com.mx) [Patricia Santana](mailto:jsantanar@liverpool.com.mx) [Josue GONZALEZ ESCANDON](mailto:jgonzaleze@liverpool.com.mx) ~~[BRIAN HERNANDEZ GARCIA](mailto:bhernandeg01@liverpool.com.mx)~~

Archivos adjuntos [Technical Session - DevCycle team ](https://calendar.google.com/calendar/event?eid=Z2k2NGF1aGhrdXNpMmtyYms1b3Q5MHI0bmFfMjAyNjEwMjJUMTQwMDAwWiBhaGVybmFuZGVwMTNAbGl2ZXJwb29sLmNvbS5teA) [Technical Session - DevCycle team  - 2026/09/02 06:55 CST - Recording](https://drive.google.com/file/d/1vjWfQbQz_MJF_EjGJoKnQHpl2LdVOwGt/view?usp=drive_web) [Notas de Gemini](https://docs.google.com/document/d/1LNel3sJ0-DRC456mxJoF9o2SmS3jOJbF4mKdKXfF9Lo/edit?usp=meet_tnfm_calendar) [Notas de Gemini](https://docs.google.com/document/d/1OibJ5WDlDCJ8WQYb216uF05P7b9CjareY8nA21EVf4Y/edit?usp=meet_tnfm_calendar)

### **Resumen**

Revisión de precios de proveedores y consolidación de tarifas con BMO

**Gestión de precios provisionales**  
Creación de tabla temporal para registrar proveedores y servicios ante complejidad actual.

**Riesgos de actualización contractual**  
Extracción de precios desde PDF genera riesgos de duplicidad e información desactualizada.

**Consolidación de tarifas BMO**  
Centralización de tarifas y revisión de servicios en SAP mediante sesión vespertina.

### **Decisiones**

## Requiere más debate

* **Evaluación de fuentes de precios de proveedores** Se aplazó la definición de la fuente centralizada y actualización de precios de proveedores para profundizar en la sesión de la tarde.

### **Próximos pasos**

- [ ] \[JONATHAN JESUS ROMERO TORRECILLA, Patricia Santana\] Consolidar Precios: Consolidar la información de costos de servicios de proveedores mediante la revisión de contratos y las tarifas establecidas por la Oficina de Gestión de Proyectos. Mantener actualizada esta base de datos centralizada.

- [ ] \[Patricia Santana\] Investigar SAP: Consultar con el equipo de servicios estratégicos y la Oficina de Gestión de Proyectos para confirmar la disponibilidad de un servicio en SAP que contenga información sobre tarifas.

### **Detalles**

**Gestión de precios de proveedores en la base de datos**: JONATHAN JESUS ROMERO TORRECILLA planteó la necesidad de revisar en la sesión de arquitectura de dónde se obtendrán los precios de los servicios de los proveedores, mencionando como ejemplos el desarrollo front de GAPSI y el desarrollo backend del equipo de Topnivera, debido a la complejidad que esto implica. JONATHAN JESUS ROMERO TORRECILLA explicó que actualmente resolvió esta situación mediante un método provisional (work around) al crear una tabla en la base de datos donde registra los proveedores, sus servicios y los precios. DULCE KESIA VALADEZ GUZMAN preguntó si existía alguna dependencia con alguien más, a lo que JONATHAN JESUS ROMERO TORRECILLA respondió que por el momento no tiene ninguna dependencia.

---

**Extracción de información desde contratos y riesgos de actualización**: Patricia Santana señaló que la información detallada sobre los servicios se encuentra en los contratos de anexos de servicio de cada proyecto por proveedor, los cuales contienen el desglose del desarrollo, la plataforma a utilizar, las horas y el costo total en archivos PDF que se emplean para entregables, facturación y pagos. JONATHAN JESUS ROMERO TORRECILLA expresó su preocupación de que extraer los precios de los archivos pueda provocar que la información esté desactualizada o duplicada. JONATHAN JESUS ROMERO TORRECILLA destacó la importancia de centralizar la información para mantener actualizada la lista de precios, mencionando como ejemplo que hace dos años el servicio de desarrollo front costaba 120,000 pesos y al año siguiente aumentó a 130,000 pesos.

---

**Consolidación de tarifas y revisión en sesión vespertina**: Patricia Santana estuvo de acuerdo con la centralización y sugirió que la BMO cuenta con tarifas establecidas por servicio, consultoría y plataformas, las cuales se pueden consolidar y actualizar. JONATHAN JESUS ROMERO TORRECILLA preguntó sobre la existencia del servicio en SAP, y Patricia Santana respondió que se revisará y detallará con el equipo de servicios estratégicos y la BMO. Finalmente, DULCE KESIA VALADEZ GUZMAN propuso profundizar en estos puntos durante la sesión de la tarde, lo cual fue aceptado por JONATHAN JESUS ROMERO TORRECILLA antes de que DULCE KESIA VALADEZ GUZMAN diera por concluida la reunión.

*Revisa las notas de Gemini para asegurarte de que sean precisas. [Obtén sugerencias y descubre cómo Gemini toma notas](https://support.google.com/meet/answer/14754931)*

*Cómo es la calidad de **estas notas específicas?** [Responde una breve encuesta](https://google.qualtrics.com/jfe/form/SV_5bXzKQfylMIhSXc?confid=HNT4EsXNojsT4UgwyJkjDxISOBEQAjIGCIoCIAAYAQg&detailLevel=standard&hasImages=False&entryPoint=footerMain&isGoogler=False&lang=es-US) para darnos tu opinión; por ejemplo, cuán útiles te resultaron las notas.*