# Integrantes

- Guerra, Lucio
- Lanzzavecchia Cespedes, Ignacio
- Quiroz, Zoe
- Wacelinka, Ariana

# Alcance

El sistema a desarrollar estará orientado a brindar una solución integral para la gestión de turnos, rutinas y ejercicios en el ámbito de un gimnasio, contemplando tanto las necesidades de los administradores como de los usuarios. La aplicación se concibe como una **herramienta digital centralizada que permita organizar de forma clara y accesible las actividades**, a la vez que promueva la comunicación y la motivación de quienes participan de ellas.

En primer lugar, el proyecto abordará la **gestión de turnos**, que constituye el eje central del sistema. Se implementará un calendario interactivo que permitirá visualizar las actividades disponibles en distintas fechas y horarios, pudiendo filtrarlas según su tipo o categoría. Los administradores tendrán la capacidad de crear turnos individuales o periódicos, configurando rangos temporales y asignando instructores responsables. Los usuarios, por su parte, podrán reservar turnos de manera sencilla, y el sistema almacenará dicha información para garantizar que no existan conflictos de disponibilidad. Asimismo, se contemplará el registro de asistencia: cada turno contará con la posibilidad de marcar la presencia de los participantes, lo que permitirá generar un historial individual y rachas de asistencia.

En segundo lugar, se incluye la **gestión de rutinas y ejercicios**, diseñada para complementar el entrenamiento de los usuarios. A través de esta funcionalidad, será posible consultar rutinas predefinidas creadas por los administradores o instructores, organizadas por nivel de dificultad o grupo muscular. Cada ejercicio estará acompañado de un recurso visual —en formato gif— que mostrará de manera clara cómo debe realizarse el movimiento. Este enfoque busca mejorar la comprensión técnica de los ejercicios y reducir el riesgo de lesiones, al mismo tiempo que facilita a los usuarios seguir sus entrenamientos incluso fuera del ámbito presencial del gimnasio.

Otro componente fundamental del alcance es el **sistema de notificaciones**, que servirá como medio de comunicación directa entre el gimnasio y sus usuarios. Las notificaciones se emplearán para recordar turnos previamente reservados, avisar sobre modificaciones de horarios o cancelaciones, y difundir anuncios relevantes relacionados con la organización. Los administradores podrán programar mensajes de alcance general o dirigidos a determinados grupos de usuarios, lo que brindará flexibilidad y mejorará la interacción.

El sistema también incorporará la **gestión de usuarios y perfiles**, asegurando que cada persona pueda acceder a la aplicación con credenciales seguras. Se establecerán roles diferenciados, siendo los principales el de administrador e instructor —con permisos para crear y gestionar actividades, editar rutinas y publicar anuncios—, y el de usuario común —con permisos para reservar turnos, consultar rutinas y recibir notificaciones. Cada perfil incluirá información básica, con la posibilidad de modificar datos personales y actualizar la imagen de perfil, manteniendo validaciones en los formularios para garantizar consistencia y seguridad en el registro de información.

Adicionalmente, el alcance contempla la posibilidad de integrar funcionalidades que fortalezcan la experiencia general. Entre ellas, se prevé la opción de gestionar **paquetes de actividades**, permitiendo que los administradores asocien a cada usuario un conjunto de “tokens” que podran utilizar para sus turnos de actividades con fecha de vencimiento, brindando un mayor control sobre la planificación de la asistencia.

De esta manera, el alcance del proyecto se configura como una solución digital completa y escalable, que en su etapa inicial permitirá organizar turnos, comunicar novedades y facilitar rutinas de entrenamiento enriquecidas con recursos visuales. Con el tiempo, se prevé su expansión hacia funciones más avanzadas que aporten valor agregado tanto a la gestión interna como a la experiencia de quienes participan en el gimnasio.

---

# Objetivo General

La organización de turnos y rutinas de entrenamiento suele gestionarse de manera manual, lo que provoca desorden, pérdida de información y falta de seguimiento de las actividades realizadas.

Frente a esta problemática, se propone el desarrollo de una aplicación móvil que centralice la gestión de turnos, notificaciones, rutinas y ejercicios, incluyendo recursos multimedia que ayuden a mejorar la experiencia de uso y el cumplimiento de los planes de entrenamiento.

De esta manera, el objetivo general del proyecto es:

> **Desarrollar una aplicación móvil que permita reservar turnos en actividades del gimnasio, recibir notificaciones, acceder a rutinas personalizadas y visualizar ejercicios mediante gifs explicativos que incluyan información sobre el músculo trabajado.**
> 

---

# Objetivos Específicos

### Primera etapa de desarrollo

- Implementar un sistema de registro e inicio de sesión seguro.
- Ofrecer la posibilidad de **reservar turnos** en las distintas actividades disponibles.
- Incorporar un sistema de **notificaciones** para recordar turnos y comunicar cambios o novedades.
- Diseñar un módulo de **rutinas y ejercicios** accesible desde la aplicación.
- Asociar a cada ejercicio un **gif demostrativo** y la descripción del músculo principal trabajado.
- Establecer roles diferenciados entre **administradores** (creación y gestión de actividades, anuncios, paquetes) y **usuarios** (acceso a rutinas, turnos y notificaciones).
- Registrar la **asistencia a los turnos** y generar un historial accesible para cada usuario.
- Incorporar un sistema de **racha de asistencia** para motivación y seguimiento del progreso.
- Permitir la **creación y edición de actividades** con horarios recurrentes y asignación de instructores.
- Gestionar **paquetes de actividades** con vencimiento y renovaciones.

# Recursos que se prevee utilizar

## Lenguajes y frameworks

Java 21 - Quarkus (Última LTS)

TypeScript - Angular 20 (Utilizando Electron)

## Recursos cloud y posible utilizacion

Colas de mensajeria (SQS o PUB/SEC) → Para la gestion de las notificaciones

Functions o Lambdas → Posible scheduler para la creacion automatica de turnos segun una plantilla predefinida

Storage S3 → Para el guardado de GIF de ejercicios

Cognito o IAM → Para login simplificado para los usuario (login por google similar)
