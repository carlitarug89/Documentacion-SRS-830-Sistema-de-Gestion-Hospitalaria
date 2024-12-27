# Documentación SRS-830
## Sistema de Gestión Hospitalaria


### Introducción

La pandemia dejó al descubierto distintas deficiencias en el sistema de salud del país.
Entre éstas, podemos mencionar la falta de instrumentación como también falta de
infraestructura hospitalaria. Ante esta situación, surge la necesidad de dar soluciones a
distintos procesos habituales del área de la salud, como la reserva de turnos, el control
de pacientes, médicos, historias clínicas e internaciones.
El desarrollo del sistema de gestión hospitalaria, tiene como objetivo principal brindar a
los distintos hospitales del país de un sistema de gestión que cubra sus distintos
procesos y transacciones diarios.
Se propone el desarrollo de un sistema de gestión que abarque los distintos
requerimientos antes mencionados a través de la elaboración de una Especificación de
Requisitos de Software (ERS). Dicho documento se encuentra desarrollado y
estructurado basado en el estándar Práctica Recomendada para ERS ANSI IEEE 830,
1998.


#### Propósito

El propósito de este documento es realizar la captura de requerimientos funcionales y
requerimientos no funcionales para el desarrollo de un sistema de gestión hospitalaria.
Se presentará la especificación de éstos, buscando proporcionar claridad sobre el
funcionamiento del sistema para los usuarios del mismo.
Los usuarios del sistema de gestión a desarrollar serán las personas encargadas del área
de administración, como también el personal médico.


#### Ámbito del Sistema

El sistema de gestión hospitalaria se encuentra diseñado y desarrollado para su uso
exclusivo en los distintos hospitales del país. Presenta las funcionalidades principales de
gestión habitual en dicho ámbito: gestión de turnos, de médicos, pacientes, historias
clínicas e internaciones. Está destinado a los siguientes usuarios: personal del área de
administración del hospital y personal médico.


#### Definiciones, acrónimos y abreviaturas

| Nombre             | Descripción                                                                                               |
|--------------------|-----------------------------------------------------------------------------------------------------------|
| Estándar IEEE 830-1998 | Conjunto de recomendaciones para la especificación de los requerimientos o requisitos de software. Como producto final, obtiene la documentación de los acuerdos entre el cliente y el grupo de desarrollo, para cumplir con la totalidad de exigencias estipuladas. |
| ERS/SRS           | Especificación de Requerimientos de Software                                                              |
| RF                | Requerimiento Funcional                                                                                   |
| RNF               | Requerimiento No Funcional                                                                                |
| Usuario           | Persona que utiliza el sistema. No está interesado en los requerimientos detallados, sino en validar los objetivos del sistema y la descripción de alto nivel de la funcionalidad. |
| TB                | Terabytes                                                                                                |


#### Referencias

| Título del Documento  | Referencia |
|-----------------------|------------|
| Standard IEEE 830-1998 | IEEE       |


#### Visión general del documento

El presente documento mantiene la siguiente estructura: inicia con una descripción
general del sistema a desarrollar y su perspectiva del producto. Luego se presenta una
descripción de los requerimientos funcionales y requerimientos no funcionales
capturados, sus características, restricciones y suposiciones. Por último, se desarrollan
los requerimientos específicos necesarios para la correcta implementación de las
funcionalidades requeridas por los usuarios del sistema.


### Descripción general


#### Perspectiva del producto

El sistema de gestión hospitalaria se basa en una aplicación diseñada con el fin de cubrir
el cumplimiento de los requerimientos fundamentales para los procesos que se llevan a
cabo en hospitales. Este sistema abarcará el registro, consulta, modificación, listado y
baja de turnos, pacientes, médicos, historias clínicas e internaciones. De este modo, se
cubren todas las áreas críticas que estaban pendientes producto de la pandemia y las
deficiencias en instrumentación e infraestructura hospitalaria.
El sistema desarrollado garantiza la optimización de los procesos y transacciones, como
así también, su usabilidad para el usuario y una mejora en la atención en el servicio
hospitalario.


#### Funciones del producto

| Requerimientos Funcionales     | Requerimientos No Funcionales                              |
|---------------------------------|------------------------------------------------------------|
| RF001: Registrar médico        | RNF001: Debe ser capaz de soportar 3000 transacciones por hora |
| RF002: Consultar médico        | RNF002: Debe funcionar en el sistema operativo Windows      |
| RF003: Modificar médico        | RNF003: Requiere un almacenamiento mínimo de los discos rígidos de 1 TB. |
| RF004: Listar médicos          | RNF004: Debe tener impresoras láser por la velocidad de las transacciones |
| RF005: Dar de baja médico      | RNF005: Se debe brindar una interfaz gráfica de uso predecible y amigable para el usuario |
| RF006: Registrar paciente      | RNF006: El sistema debe estar disponible para su uso las 24 horas de todos los días de la semana. |
| RF007: Consultar paciente      | RNF007: El sistema debe asegurar la seguridad y privacidad de los datos almacenados. |
| RF008: Modificar paciente      | RNF008: El sistema estará desarrollado con los lenguajes HTML y Java. |
| RF009: Listar pacientes        | RNF009: La interfaz debe usarse con Internet.              |
| RF010: Dar de baja paciente    | RNF010: El sistema se diseña según un modelo cliente/servidor. |
| RF011: Seleccionar especialidad médica | RNF011: El tiempo de respuesta de las transacciones no debe superar los 4000 milisegundos. |
| RF012: Seleccionar médico especialista |                                                             |
| RF013: Registrar turno         |                                                             |
| RF014: Consultar turno         |                                                             |
| RF015: Modificar turno         |                                                             |
| RF016: Listar turnos           |                                                             |
| RF017: Dar de baja turno       |                                                             |
| RF018: Registrar historia clínica |                                                           |
| RF019: Consultar historia clínica |                                                           |
| RF020: Modificar historia clínica |                                                           |
| RF021: Listar historias clínicas |                                                           |
| RF022: Dar de baja historia clínica |                                                         |
| RF023: Consultar camas existentes en internación |                                                  |
| RF024: Registrar internación   |                                                             |
| RF025: Consultar internación   |                                                             |
| RF026: Modificar internación   |                                                             |
| RF027: Listar internaciones    |                                                             |
| RF028: Dar de baja internación |                                                             |
| RF029: Registrar paciente internado |                                                          |
| RF030: Consultar paciente internado |                                                          |
| RF031: Modificar paciente internado |                                                          |
| RF032: Listar pacientes internados |                                                         |
| RF033: Dar de baja paciente internado |                                                       |


Diagrama de Caso de Uso:


![image](https://github.com/user-attachments/assets/3d8fc3a8-7623-41c9-8b80-e7cf77194c8b)


#### Características de los usuarios

| Tipo de Usuario | Formación        | Actividades                              |
|------------------|------------------|------------------------------------------|
| Administrador    | Administración  | Gestión de turnos y gestión de historias clínicas |


| Tipo de Usuario | Formación | Actividades                              |
|------------------|-----------|------------------------------------------|
| Médico           | Medicina  | Gestión de pacientes y gestión de internaciones |


#### Restricciones

Para el desarrollo del sistema de gestión hospitalaria se considerarán las siguientes
restricciones:

- El sistema debe ser capaz de soportar 3000 transacciones por hora.

- Debe funcionar en el sistema operativo Windows.

- Requiere un almacenamiento mínimo de los discos rígidos de 1 TB.

- Debe tener impresoras láser por la velocidad de las transacciones.

- Se debe brindar una interfaz gráfica de uso predecible y amigable para el
usuario.

- El sistema debe estar disponible para su uso las 24 horas de todos los días de la
semana.

- El tiempo de respuesta de las transacciones no debe superar los 4000
milisegundos.

- El sistema debe asegurar la seguridad y privacidad de los datos almacenados.

- El sistema estará desarrollado con los lenguajes HTML y Java.

- La interfaz debe usarse con Internet.

- El sistema se diseña según un modelo cliente/servidor.


#### Suposiciones y dependencias

- El sistema de gestión hospitalaria debe proveer las herramientas necesarias para
generar la migración de los sistemas de información existentes en los hospitales.

- Se tiene la suposición de que los usuarios habilitados para el acceso al sistema
de gestión hospitalaria tienen conocimientos básicos en informática.


#### Requisitos futuros

El sistema de gestión hospitalaria deberá ser escalable y permitir la adición de nuevas
funcionalidades en el futuro que pueden ser extraídas de la lista de requerimientos
candidatos que posean.


### Requisitos específicos

| Identificación de Requerimiento | RF013                                            |
|----------------------------------|-------------------------------------------------|
| Nombre del Requerimiento         | Registrar turno                                 |
| Características                  | El usuario (encargado de Administración) debe poder registrar turnos de los pacientes en el hospital. |
| Descripción del Requerimiento    | El usuario (encargado de Administración) ingresa a la interfaz del sistema. Escoge del menú la opción Registrar turno. <br> Datos que debe ingresar obligatoriamente: Nombre, Apellido, DNI, Médico, Especialidad, Fecha, Hora. <br> El usuario tiene la opción de guardar el turno o cancelarlo. |
| Requerimiento No Funcional       | RNF001, RNF002, RNF003, RNF004, RNF005, RNF006, RNF007, RNF011 |
| Prioridad del Requerimiento      | Alta                                            |


| Identificación de Requerimiento | RF014                                            |
|----------------------------------|-------------------------------------------------|
| Nombre del Requerimiento         | Consultar turno                                 |
| Características                  | El usuario (encargado de Administración) debe poder consultar los turnos de los pacientes en el hospital. |
| Descripción del Requerimiento    | El usuario (encargado de Administración) ingresa a la interfaz del sistema. Escoge del menú la opción Consultar turnos. <br> Datos que debe ingresar obligatoriamente: Nombre, Apellido, DNI. <br> El sistema le devuelve al usuario los turnos registrados para el paciente ingresado. |
| Requerimiento No Funcional       | RNF001, RNF002, RNF003, RNF004, RNF005, RNF006, RNF007, RNF011 |
| Prioridad del Requerimiento      | Media                                           |


| Identificación de Requerimiento | RF015                                            |
|----------------------------------|-------------------------------------------------|
| Nombre del Requerimiento         | Modificar turno                                 |
| Características                  | El usuario (encargado de Administración) debe poder modificar turnos de los pacientes en el hospital. |
| Descripción del Requerimiento    | El usuario (encargado de Administración) ingresa a la interfaz del sistema. Escoge del menú la opción Modificar turno. <br> Datos que debe ingresar obligatoriamente: Nombre, Apellido, DNI, Médico, Especialidad, Fecha, Hora. <br> El usuario tiene la opción de guardar las modificaciones realizadas o cancelarlo. |
| Requerimiento No Funcional       | RNF001, RNF002, RNF003, RNF004, RNF005, RNF006, RNF007, RNF011 |
| Prioridad del Requerimiento      | Alta                                            |


| Identificación de Requerimiento | RF016                                            |
|----------------------------------|-------------------------------------------------|
| Nombre del Requerimiento         | Listar turnos                                   |
| Características                  | El usuario (encargado de Administración) debe poder mostrar el listado de turnos de los pacientes en el hospital. |
| Descripción del Requerimiento    | El usuario (encargado de Administración) ingresa a la interfaz del sistema. Escoge del menú la opción Listar turnos. <br> Datos que se muestran: Nombre, Apellido, DNI, Médico, Especialidad, Fecha, Hora. <br> El usuario puede filtrar el listado de turnos por especialidad y por médico registrado. |
| Requerimiento No Funcional       | RNF001, RNF002, RNF003, RNF004, RNF005, RNF006, RNF007, RNF011 |
| Prioridad del Requerimiento      | Media                                           |


| Identificación de Requerimiento | RF017                                            |
|----------------------------------|-------------------------------------------------|
| Nombre del Requerimiento         | Dar de baja turno                               |
| Características                  | El usuario (encargado de Administración) debe poder dar de baja los turnos de los pacientes en el hospital. |
| Descripción del Requerimiento    | El usuario (encargado de Administración) ingresa a la interfaz del sistema. Escoge del menú la opción Dar de baja turno. <br> Datos que debe ingresar obligatoriamente: Nombre, Apellido, DNI, Médico, Especialidad, Fecha, Hora. <br> El usuario tiene la opción de dar de baja el turno o cancelar la baja. |
| Requerimiento No Funcional       | RNF001, RNF002, RNF003, RNF004, RNF005, RNF006, RNF007, RNF011 |
| Prioridad del Requerimiento      | Alta                                            |


#### Interfaces externas

![image](https://github.com/user-attachments/assets/8475d8d7-868f-46e0-b36f-67241b0dc27d)


#### Funciones

El sistema de gestión hospitalaria cubrirá las siguientes funciones:

- Autenticación de usuarios (personal administrativo y personal médico) para el
acceso al sistema.

- Registro de turnos con los datos de los pacientes (Nombre, Apellido y DNI),
especialidad médica, médico (Nombre y Apellido), fecha y hora del turno.

- Consulta de turnos agendados con los datos del paciente (Nombre, Apellido y
DNI).

- Modificación de turnos agendados con los datos del turno registrado.
  
- Listado de turnos agendados. El usuario accederá a él desde el menú. Se
mostrarán todos los datos de los turnos agendados y se podrán filtrar por
especialidad y por médico.

- Baja de turnos agendados con el ingreso de los datos del turno registrado.


#### Requisitos de Rendimiento

- El sistema debe ser capaz de soportar 3000 transacciones por hora.
- El tiempo de respuesta de las transacciones no debe superar los 4000
milisegundos.
- El sistema debe estar disponible para su uso las 24 horas de todos los días de la
semana.


#### Restricciones de Diseño

- El sistema debe ser compatible con el sistema operativo Windows.
- El sistema requiere un almacenamiento mínimo de los discos rígidos de 1 TB.
- Se debe tener impresoras láser por la velocidad de las transacciones.


#### Atributos del Sistema


![image](https://github.com/user-attachments/assets/b782a0fe-3cd0-48c9-927b-dcb42f5fa47e)


#### Otros requisitos

- El sistema debe brindar una interfaz gráfica de uso predecible y amigable para el
usuario.
- El sistema debe asegurar la seguridad y privacidad de los datos almacenados.
- Se requiere un entrenamiento para el uso del sistema por parte de los usuarios.
