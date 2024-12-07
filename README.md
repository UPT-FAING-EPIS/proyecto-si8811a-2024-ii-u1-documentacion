

**UNIVERSIDAD PRIVADA DE TACNA**

**FACULTAD DE INGENIERIA**

**Escuela Profesional de Ingeniería de Sistemas**


**Proyecto *“Aplicativo Móvil Juegos Florales”***

Curso: *Construcción de Software I*

Docente: *Patrick José Cuadros Quiroga*

Integrantes:

***Arenas Paz Soldan, Miguel Jesus	(2017059282)***

***Lizárraga Pomareda, Sergio Pedro	(2020066921)***






**Tacna – Perú**

***2024***


![ref1]![ref2]![ref3]

|CONTROL DE VERSIONES||||||
| :-: | :- | :- | :- | :- | :- |
|Versión|Hecha por|Revisada por|Aprobada por|Fecha|Motivo|
|1\.0|MAPS|SPLP|SPLP|31/08/2024|Versión Original|








**Sistema *“Aplicativo Móvil Juegos Florales”***

**Documento de Visión**

**Versión *1.2***



**INDICE GENERAL**

1. [Introducción**	5](#_bookmark0)
   1. [**Propósito**	5](#_bookmark1)
   1. [**Alcance**	5](#_bookmark2)
   1. [**Definiciones, Siglas y Abreviaturas**	6](#_bookmark3)
   1. [**Visión General**	6](#_bookmark4)
1. [**Posicionamiento**	7](#_bookmark5)
   1. [**Oportunidad de negocio**	7](#_bookmark6)
   1. [**Definición del problema**	8](#_bookmark7)
1. [**Descripción de los interesados y usuarios**	9](#_bookmark8)
   1. [**Resumen de los interesados**	9](#_bookmark9)
   1. [**Resumen de los usuarios**	10](#_bookmark10)
   1. [**Entorno de usuario**	10](#_bookmark11)
   1. [**Perfiles de los interesados**	10](#_bookmark12)
   1. [**Perfiles de los usuarios**	10](#_bookmark13)
   1. [**Necesidades de los interesados y usuarios**	12](#_bookmark14)
1. [**Vista General del Producto**	13](#_bookmark15)
   1. [**Perspectiva del producto**	13](#_bookmark16)
   1. [**Resumen de capacidades**	13](#_bookmark17)
   1. [**Suposiciones y dependencias**	14](#_bookmark18)
   1. [**Costos y precios**	15](#_bookmark19)
   1. [**Licenciamiento e instalación**	15](#_bookmark20)
1. [**Características del producto**	15](#_bookmark21)
   1. [**Gestión y control de los usuarios**	15](#_bookmark22)
   1. [**Gestión y control de participantes y competencias**	16](#_bookmark23)
   1. [**Seguimiento y control de actividades**	16](#_bookmark24)
1. [**Restricciones**	16](#_bookmark25)
1. [**Rangos de calidad**	16](#_bookmark26)
1. [**Precedencia y Prioridad**	16](#_bookmark27)
1. [**Otros requerimientos del producto**	17](#_bookmark28)
   1. [**Estándares legales**	17](#_bookmark29)
   1. [**Estándares de comunicación**	17](#_bookmark30)
   1. [**Estándares de cumplimiento de la plataforma**	18](#_bookmark31)
   1. [**Estándares de calidad y seguridad**	18](#_bookmark32)
1. [**CONCLUSIONES**	18](#_bookmark33)
1. [**RECOMENDACIONES**	18](#_bookmark34)
1. [**WEBGRAFIA**	18](#_bookmark35)



1. # <a name="1. introducción"></a><a name="_bookmark0"></a>**Introducción**

1. # <a name="1.1. propósito"></a><a name="_bookmark1"></a>**Propósito**

El propósito del proyecto es desarrollar e implementar un Aplicativo Móvil para la Gestión de los Juegos Florales en la comunidad universitaria, con el objetivo de optimizar los procesos de registro y seguimiento, garantizar la seguridad en el almacenamiento de la información y permitir un seguimiento, garantizar la seguridad en el almacenamiento de la información, y permitir un seguimiento eficiente de las actividades deportivas y culturales. Además, el sistema utilizará tecnologías modernas para automatizar la creación de calendarios y la gestión de eventos a partir de las inscripciones y categorías participantes, mejorando la organización y la planificación de actividades dentro del evento. Con este proyecto, se busca modernizar la gestión administrativa de los juegos florales, aumentar la transparencia en los resultados, y reducir los tiempos operativos, proporcionando una solución tecnológica avanzada que responda a las necesidades actuales de la comunidad universitaria.
1. # <a name="1.2. alcance"></a><a name="_bookmark2"></a>**Alcance**

El proyecto incluye el diseño, desarrollo e implementación de una app móvil para la gestión de los Juegos Florales. El sistema permitirá las diferentes áreas de trabajo y abordará los siguientes procesos:

0. **Eficiencia en el Tiempo de Acceso a la Información**: Optimización de la rapidez y facilidad de acceso a la información de participantes, resultados y cronogramas de competencias, mejorando la eficiencia operativa del evento
0. **Gestión de Registros y Participantes**: Implementación de mecanismos efectivos para el registro y seguimiento de participantes en las diferentes disciplinas, garantizando la disponibilidad continua de la información de las competencias.
0. **Organización y Control de Eventos**: Centralización y organización de la información para evitar la duplicación de registros, superposición de horarios y mejorar la calidad en la gestión de las diferentes actividades deportivas y culturales.


1. # <a name="1.3. definiciones, siglas y abreviaturas"></a><a name="_bookmark3"></a>**Definiciones, Siglas y Abreviaturas**

0. **Kanban**: Un enfoque de gestión de flujo de trabajo que utiliza un sistema visual para optimizar y gestionar tareas continuas, promoviendo la eficiencia y la flexibilidad en el desarrollo de proyectos.
0. **Encriptación**: Proceso de codificación de datos para proteger la información de accesos no autorizados, asegurando su confidencialidad y seguridad.
0. **API**: La Interfaz de Programación de Aplicaciones es un conjunto de subrutinas, funciones y procedimientos que ofrece una biblioteca para ser utilizada por otro software, proporcionando una capa de abstracción.
0. **Sistemas de Información**: (Espino, 2018) Define la informática como la ciencia que estudia la transmisión, almacenamiento y análisis de datos. Estos datos, al ser procesados, se convierten en información que puede realizar diversas funciones con ayuda de un dispositivo automático.
1. # <a name="1.4. visión general"></a><a name="_bookmark4"></a>**Visión General**

El presente documento mostrará un análisis detallado de la visión del proyecto “Aplicativo Móvil Juegos Florales”, organizada de forma en la que el lector podrá encontrar la descripción de los diferentes aspectos del sistema, las cuales están distribuidos de la siguiente manera: descripción general del proyecto, objetivos, alcance, análisis de requerimientos, factibilidad técnica y operativa, diseño de la solución. Desarrollo e implementación, plan de pruebas y calendario de actividades, asegurando una comprensión completa de la solución propuesta para optimizar la gestión de los juegos florales en la comunidad universitaria.

0. Sección 1. Introducción, una vista general de lo que tratará la documentación del sistema.
0. Sección 2 Representación Arquitectónica, describe qué arquitectura de Software será utilizada para el desarrollo del sistema y cómo será representada.
0. Sección 3 Objetivos y Limitaciones Arquitectónicas, muestra como la disponibilidad, seguridad, adaptabilidad y rendimiento que impactan en la arquitectura de software seleccionada.
0. Sección 4 Análisis de requerimientos, describen los requerimientos del sistema, y también muestra el análisis de requerimientos no funcionales.
0. Sección 5 Vista de Casos de Uso, contiene los casos de uso del sistema.

0. Sección 6 Vista Lógica, tiene una descripción de las partes más importantes de la arquitectura.
0. Sección 7 Vista de Procesos, muestra los respectivos diagramas de secuencia de los casos de uso del sistema.
0. Sección 8 Vista de Despliegue, describe la arquitectura de tecnología en la que será desplegada la aplicación.
0. Sección 9 Vista de Implementación, incluirá especificaciones del sistema y de la interfaz de usuario, es decir, los diferentes componentes que conforman el sistema.
0. Sección 10 Calidad, muestra los atributos de calidad que son tenidos en cuenta.
1. # <a name="2. posicionamiento"></a><a name="_bookmark5"></a>**Posicionamiento**

1. # <a name="2.1. oportunidad de negocio"></a><a name="_bookmark6"></a>**Oportunidad de negocio**

Actualmente, la universidad carece de un sistema integral para gestionar los juegos florales de forma eficiente. Los organizadores y participantes no disponen de una plataforma centralizada, ni de una solución integrada para la gestión de las diferentes actividades deportivas y culturales que forman parte del evento.

Dado el avance de las tecnologías de información, muchas de las cuales son de código abierto y de bajo coste, es esencial implementar un sistema moderno que mejore el registro y seguimiento de participantes, optimice la gestión de resultados y facilite la planificación de eventos mediante herramientas digitales. Este enfoque permitirá a la comunidad universitaria modernizar sus procesos y aumentar la eficiencia operativa en la organización de los juegos florales, respondiendo a las necesidades actuales de transparencia y gestión efectiva de competencias.

**Tabla de Oportunidad de Negocio**

|**El problema de**|<p>La falta de control en el registro y seguimiento de participantes, la ausencia de un sistema centralizado para resultados y la falta de automatización en la creación de calendarios</p><p>de competencias y eventos culturales.</p>|
| :- | - |
|**Afecta a**|Estudiantes que necesitan registrarse en las diferentes	disciplinas,	organizadores	que|


||<p>requieren gestionar las competencias de manera eficiente y jurados que necesitan registrar resultados de forma segura y tener una visualización eficiente de los eventos en</p><p>su calendario</p>|
| :- | - |
|**El impacto negativo es**|<p>Pérdida de información de participantes, retrasos en la publicación de resultado, duplicidad de registros y desorganización en la planificación de eventos deportivos y culturales lo que genera confusión y malestar</p><p>en la comunidad universitaria.</p>|
|**Una solución adecuada sería**|Implementar un sistema integral que incluya un seguimiento de participantes con respaldo automático, gestión de resultados en tiempo real mejorando la experiencia de todos los involucrados en los juegos florales.|


**Fuente: Elaboración Propia**

**Descripción:** La tabla de Oportunidad de Negocio presenta un análisis estructurado del problema y su solución propuesta para un sistema de gestión de los Juegos Florales universitarios identificando el problema principal de la falta de un sistema centralizado para la gestión de competencias, los actores afectados (estudiantes, organizadores y jurados), el impacto negativo en la organización del evento, y propone como solución la implementación de un sistema integral que automatice el registro, seguimiento y gestión de las actividades deportivas y culturales.
1. # <a name="2.2. definición del problema"></a><a name="_bookmark7"></a>**Definición del problema**

La comunidad universitaria enfrenta serias limitaciones en la gestión de sus juegos florales debido a la falta de un sistema centralizado para registrar, administrar y dar seguimiento a las diferentes competencias y actividades culturales. Los datos de participantes y resultados se gestionan de manera ineficiente utilizando hojas de cálculo y documentos físicos, lo que incrementa el riesgo de pérdida, duplicación de información y compromete la transparencia del evento.

Además, la ausencia de una solución digital integrada para el registro de participantes y la falta de un sistema automatizado para la creación y gestión de calendarios de competencias agravan la situación. Esta deficiencia afecta la coordinación entre organizadores y participantes, retrasa la publicación de resultados y desorganiza la planificación de eventos, comprometiendo el desarrollo eficiente de los juegos florales. Es urgente implementar un sistema web integral que aborde estos problemas, garantice el correcto registro y seguimiento de participantes, facilite la gestión de resultados y automatice la programación de competencias, optimizando así los procesos del evento.
1. # <a name="3. descripción de los interesados y usua"></a><a name="_bookmark8"></a>**Descripción de los interesados y usuarios**

1. # <a name="3.1. resumen de los interesados"></a><a name="_bookmark9"></a>**Resumen de los interesados**

**Tabla Resumen de los Interesados**

|**Nombre**|**Descripción**|
| :- | :- |
|Estudiante Participante|Permite registrarse en las diferentes disciplinas, consultar calendarios de competencias y ver resultados en tiempo real.|
|Organizador|Gestiona el registro de participantes, administra las competencias, publica resultados y coordina los eventos deportivos y culturales.|
|Jurado|Evalúa las competencias, registra puntajes y resultados y gestiona la calificación de las diferentes disciplinas|
|Administrador|Supervisa todo el sistema, gestiona usuarios y permisos, y garantiza el correcto funcionamiento de la plataforma.|


**Fuente:** Elaboración Propia

**Descripción:** Esta tabla de Resumen de los Interesados presenta los principales actores del sistema de Juegos Florales, definiendo las funciones específicas de cada uno: estudiantes participantes, organizadores, jurados y administradores, sintetizando sus roles e interacciones en la plataforma.

1. # <a name="3.2. resumen de los usuarios"></a><a name="_bookmark10"></a>**Resumen de los usuarios**

**Tabla Resumen de los usuarios**

|**Nombre**|**Descripción**|
| :- | :- |
|Administrador|Usuario que tendrá todos los privilegios en la aplicación.|
|Organizador|Usuario que gestionar las competencias, registrar resultados y administrar el calendario de eventos deportivos y culturales.|
|Jurado|Usuario que podrá evaluar y registrar resultados de las competencias asignadas según su especialidad|
|Participante|Usuario que podrá registrarse en competencias, ver calendarios y consultar sus resultados en los diferentes eventos.|


**Fuente: Elaboración Propia**

**Descripción:** Esta tabla de resumen de los usuarios define los diferentes roles y niveles de acceso en el sistema de Juegos Florales, estableciendo cinco tipos de usuarios: desde el Administrador con privilegios totales hasta el Visitante con acceso limitado, garantizando una gestión organizada y segura de los permisos dentro de la plataforma.
1. # <a name="3.3. entorno de usuario"></a><a name="_bookmark11"></a>**Entorno de usuario**

Los usuarios podrán usar el sistema web mediante cualquier navegador desde su computadora o teléfono móvil, requiriendo conexión a internet estable.
1. # <a name="3.4. perfiles de los interesados"></a><a name="_bookmark12"></a>**Perfiles de los interesados**

Perfil principal: No se vería afectado si el usuario final no tiene un grado de estudios, el perfil requerido, es de un usuario con conocimientos básicos en informática.
1. # <a name="3.5. perfiles de los usuarios"></a><a name="_bookmark13"></a>**Perfiles de los usuarios**

0. Administrador: Este usuario tiene el control total del sistema de juegos florales, pudiendo configurar todos los aspectos como gestión de usuarios, asignación de roles y accesos, supervisar todas las funcionalidades de la plataforma.

0. Organizador: Este usuario representa al personal encargado de gestionar las competencias, con las funcionalidades de registrar participantes, programar eventos, administrar resultados y coordinar las diferentes actividades deportivas y culturales.
0. Jurado: Este usuario tiene acceso a las funcionalidades específicas de evaluación y calificación de las competencias que le han sido asignadas según su especialidad, pudiendo registrar puntajes y resultados.
0. Participante: Este usuario representa a los estudiantes que participan en las competencias, con acceso a las funcionalidades de inscripción, consulta de calendarios y visualización de los resultados.

1. # <a name="3.6. necesidades de los interesados y us"></a><a name="_bookmark14"></a>**Necesidades de los interesados y usuarios**

**Tabla de Necesidades de los Interesados y Usuarios**

|**Nombre**|**Descripción**|**Prioridad**|
| :- | :- | :- |
|Capacitación en el uso del sistema|Asegura que los usuarios comprendan y utilicen todas las funcionalidades del sistema de juegos florales.|Alta|
|Registro segur de participantes|Implementa medidas para proteger la integridad y seguridad de los datos de los participantes registrados.|Alta|
|Gestión	de resultados|Facilita el registro y publicación de resultados en tiempo real para todas las competencias.|Alta|
|<p>Gestión automatizada	de calendarios		y</p><p>eventos</p>|Automatiza la planificación de competencia y actividades culturales basados en las inscripciones.|Alta|
|<p>Acceso	a	la</p><p>información centralizada</p>|<p>Facilita	el	acceso	a	información	de</p><p>competencias	mediante	una	plataforma centralizada.</p>|Alta|
|Generación	de reportes|<p>Implementa	mecanismos	para	generar</p><p>informes y estadísticas de participación y resultados</p>|Alta|
|Seguimientos	de competencias|Permite el monitoreo en tiempo real del desarrollo de las diferentes disciplinas|Alta|

**Fuente:** Elaboración Propia

**Descripción:** Esta tabla de Necesidades de los Interesados y Usuarios presenta los requerimientos fundamentales del sistema de Juegos Florales, todos con prioridad Alta, definiendo las funcionalidades esenciales para garantizar una gestión eficiente del evento deportivo y cultural
1. # <a name="4. vista general del producto"></a><a name="_bookmark15"></a>**Vista General del Producto**

1. # <a name="4.1. perspectiva del producto"></a><a name="_bookmark16"></a>**Perspectiva del producto**

El Aplicativo Móvil para la gestión de Juegos Florales será una plataforma web avanzada diseñada para la comunidad universitaria. Este sistema centralizará y asegurará la gestión de participantes, permitiendo el registro eficiente y el seguimiento de las diferentes competencias mediante una interfaz intuitiva.

Incorporará un módulo robusto para el registro y seguimiento de actividades deportivas y culturales, y utilizará tecnologías modernas para automatizar la gestión de eventos basados en las inscripciones de los participantes.

La plataforma mejorará la eficiencia operativa, reducirá la dependencia de métodos manuales y físicos, y ofrecerá una solución moderna y escalable que facilitará una administración más ágil y efectiva de los juegos florales universitarios.
1. # <a name="4.2. resumen de capacidades"></a><a name="_bookmark17"></a>**Resumen de capacidades**

**Tabla Resumen de Capacidades**

|**Beneficio	de cliente**|**Características de soporte**|
| :- | :- |
|Gestión	de usuarios|El aplicativo móvil debe permitir a los usuarios registrarse, iniciar sesión y gestionar sus perfiles según su rol (administrador, organizador, jurado o participante)|
|Eficiencia Operativa|El aplicativo móvil debe permitir a los participantes acceder a la información de competencias y resultados de manera rápida y centralizada.|


|Facilitación de la Colaboración|<p>Mejora en la comunicación entre organizadores, jurados y</p><p>participantes, permitiendo una coordinación más efectiva de los eventos.</p>|
| :- | :- |
|Gestión	de Competencias|El sistema debe permitir registrar participantes en las diferentes disciplinas, gestionar resultados y generar reportes de las competencias.|
|Seguimiento	de Actividades|El sistema debe permitir rastrear el estado de las competencias a lo largo de su desarrollo, incluyendo inscripciones, desarrollo y resultados finales.|
|Gestión	de Recursos|El sistema debe permitir la administración de espacios y equipamiento necesario para cada disciplina deportiva y cultural.|


**Fuente:** Elaboración Propia

**Descripción:** La siguiente tabla de Resumen de Capacidades presenta seis funcionalidades principales del sistema: gestión de usuarios para accesos, eficiencia operativa para el manejo de información, colaboración entre usuarios, gestión de competencias, seguimiento de actividades deportivas y culturales, y administración del recurso.
1. # <a name="4.3. suposiciones y dependencias"></a><a name="_bookmark18"></a>**Suposiciones y dependencias**

0. Capacitación y Conocimientos: Se supone que los usuarios recibirán capacitación adecuada y tienen el nivel de conocimientos necesario para utilizar eficientemente el sistema de aplicativo móvil. El buen uso del software dependerá en gran medida de esta capacitación.
0. Recursos Disponibles: Se asume que se contarán con los recursos necesarios para el desarrollo y la implementación del proyecto, tanto en términos de tecnología como de personal.
0. Capacidad Técnica y Administrativa: El proyecto contará con la capacidad técnica y administrativa necesaria para llevar a cabo el desarrollo y la implementación del sistema con éxito.

0. Conexión a Internet: Se requiere que los usuarios dispongan de una conexión a internet estable y sepan utilizar la aplicación web para aprovechar todas las funcionalidades del sistema.
0. Dispositivos Compatibles: Los usuarios deberán contar con un dispositivo móvil o de escritorio compatible para hacer uso de la aplicación
1. # <a name="4.4. costos y precios"></a><a name="_bookmark19"></a>**Costos y precios**

**Tabla de Costos y precios**

|**COSTOS DE DEL DESARROLLO DEL SISTEMA**||
| :- | :- |
|Tipo|Costo|
|Costos generales|S/. 200.00|
|Costos operativos|S/. 840.00|
|Costos del ambiente|S/. 0.00|
|Costos del personal|S/. 8,200.00|
|Total|S/. 9240.00|

**Fuente:** Elaboración Propia

**Descripción:** La tabla detalla el presupuesto del sistema que suma S/9,240.00, distribuido principalmente en costos de personal (S/8,200.00), seguido por costos operativos (S/840.00), costos generales (S/200.00) y sin costos de ambiente.
1. # <a name="4.5. licenciamiento e instalación"></a><a name="_bookmark20"></a>**Licenciamiento e instalación**

La instalación, configuración y despliegue del sistema se realizará en base a la guía de instalación.
1. # <a name="5. características del producto"></a><a name="_bookmark21"></a>**Características del producto**

1. # <a name="5.1. gestión y control de los usuarios"></a><a name="_bookmark22"></a>**Gestión y control de los usuarios**

Permite el registro y administración de la información de los usuarios, incluyendo la asignación de roles y permisos para asegurar el acceso adecuado a las diferentes funcionalidades del sistema de juegos florales.

1. # <a name="5.2. gestión y control de participantes "></a><a name="_bookmark23"></a>**Gestión y control de participantes y competencias**

Permite registrar, modificar o eliminar inscripciones en las diferentes disciplinas según las necesidades. Incluye la funcionalidad de registro de resultados, así como la generación de reportes y estadísticas de participación.
1. # <a name="5.3. seguimiento y control de actividade"></a><a name="_bookmark24"></a>**Seguimiento y control de actividades**

Automatiza el seguimiento de las diferentes competencias y eventos culturales, permitiendo la visualización de avances y resultados en tiempo real. Los organizadores también pueden gestionar el desarrollo de las actividades según sea necesario.
1. # <a name="6. restricciones"></a><a name="_bookmark25"></a>**Restricciones**

- Se tiene como fecha límite de entrega del proyecto el día 14 de diciembre del 2024.
- El sistema sólo admitirá el ingreso a los usuarios registrados en la universidad.

1. # <a name="7. rangos de calidad"></a><a name="_bookmark26"></a>**Rangos de calidad**

- SEGURIDAD: El sistema debe mantener la información de forma protegida mediante registro de usuarios.
- ESCALABILIDAD: El sistema debe trabajar con diferentes cantidades de trabajo, como cambios en el volumen de datos.
- DISPONIBILIDAD: El Sistema deberá ser accesible el 90% del tiempo.
- EFICIENCIA: El sistema debe demorar lo mínimo en responder 05 segundos.
- USABILIDAD: El sistema deberá mostrar una interfaz dinámica para que el usuario pueda adecuarse al sistema fácilmente.
1. # <a name="8. precedencia y prioridad"></a><a name="_bookmark27"></a>**Precedencia y Prioridad**

El proyecto propuesto pretende poder tener acceso remoto, seguridad, respaldo de la información.

El desarrollo de los módulos del proyecto está ordenado según su prioridad, siendo la más alta la más importante y la más baja la menos importante.

**Tabla de Precedencia y Prioridad**

|**Descripción**|**Prioridad**|
| :- | :- |
|Módulo de Inicio de Sesión y Registro|Alta|
|Módulo de Registro de Participantes|Alta|
|Módulo de Gestión de Competencias|Alta|
|Módulo de Seguimiento de Resultados|Alta|
|Módulo de Notificaciones|Alta|
|Módulo de Reportes|Alta|


**Fuente: Elaboración Propia**

**Descripción:** La tabla de Precedencia y Prioridad muestra los módulos principales del sistema de Juegos Florales, todos categorizados con prioridad Alta para garantizar la funcionalidad integral de la plataforma
1. # <a name="9. otros requerimientos del producto"></a><a name="_bookmark28"></a>**Otros requerimientos del producto**

1. # <a name="9.1. estándares legales"></a><a name="_bookmark29"></a>**Estándares legales**

0. Ser estudiante activo de la universidad donde se utilizará el sistema.
0. Aceptar los términos y condiciones del uso del sistema y política de privacidad de datos.
0. Cumplir con los reglamentos internos de participación en juegos florales establecidos por la universidad.
1. # <a name="9.2. estándares de comunicación"></a><a name="_bookmark30"></a>**Estándares de comunicación**

0. Brindar a los usuarios administradores un número de contacto con el cual poder brindarle soporte e incluso una cuenta exclusiva para el administrador

1. # <a name="9.3. estándares de cumplimiento de la pl"></a><a name="_bookmark31"></a>**Estándares de cumplimiento de la plataforma**

La plataforma debe cumplir con los estándares mínimos de funcionamiento tales como:

0. Las capacidades del sistema.
0. Las características del sistema.
0. Los objetivos del proyecto.

1. # <a name="9.4. estándares de calidad y seguridad"></a><a name="_bookmark32"></a>**Estándares de calidad y seguridad**

Seguridad:

0. La confidencialidad de los datos ingresados por los usuarios.
0. El uso de contraseñas para las cuentas de los usuarios.

Calidad:

0. Que se use contraseñas encriptadas SHA256.
0. Que el sistema no permita el ingreso de usuarios bloqueados.

1. # <a name="10. conclusiones"></a><a name="_bookmark33"></a>**CONCLUSIONES**

El documento expuesto hace referencia al plan del proyecto de desarrollo del sistema Juegos Florales universitarios, el cual expone y hace uso de las herramientas que nos brinda la ingeniería de software para llevar de buena manera el ciclo de vida del desarrollo. Por tanto, lo aquí expuesto contribuye a la realización eficiente y eficaz de una plataforma que optimizará la gestión de las competencias deportivas y culturales, mejorando significativamente la experiencia de todos los usuarios involucrados.
1. # <a name="11. recomendaciones"></a><a name="_bookmark34"></a>**RECOMENDACIONES**

- Tener conocimiento básico en informática.
- Para mejorar el funcionamiento, el usuario con roles debe ser guiado por los usuarios administradores al menos una primera vez para enseñarle el aplicativo.
- No disponer a cualquier persona la cuenta o los datos del usuario administrador.

1. # <a name="12. webgrafia"></a><a name="_bookmark35"></a>**WEBGRAFIA**
