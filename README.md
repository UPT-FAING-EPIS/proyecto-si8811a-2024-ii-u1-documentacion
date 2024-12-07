

[FD04_Informe SAD_AplicacionMóvil.docx](https://github.com/user-attachments/files/18049447/FD04_Informe.SAD_AplicacionMovil.docx)

![image](https://github.com/user-attachments/assets/834e61cf-320c-4177-8c59-878a86e1c324)

**UNIVERSIDAD PRIVADA DE TACNA**
# **FACULTAD DE INGENIERÍA**
**Escuela Profesional de Ingeniería de Sistemas**


**Proyecto “Aplicativo Movil Juegos Florales”**

**Curso:** Tópicos de Bases de Datos Avanzados

**Docente:** Patrick José Cuadros Quiroga

# **Integrantes:**

Arenas Paz Soldan, Miguel Jesus (2017059282)

Lizárraga Pomareda, Sergio Pedro (2020066921)

Tacna – Perú

2024

|CONTROL DE VERSIONES|
| :-: | :- | :- | :- | :- | :- |
|Versión|Hecha por|Revisada por|Aprobada por|Fecha|Motivo|
|1\.0||||<p></p><p></p><p>12/11/2024</p>|<p></p><p></p><p>Versión 1.0</p>|


# **App Móvil de Juegos Florales**

Documento SAD

Versión 1.0


![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABcAAAASCAYAAACw50UTAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAOxAAADsQBlSsOGwAAAIJJREFUOI3t0qENwgAQRuGvOARBIKipZoAuwCw4FIIwQxfA1RBSU9GRMHgWwFDR1qDa5AQkfcmJS+7en1yOmV9hjzseaPo+jCt2WOKAF9LIgIENPsinLi5GzGR44zlVPia8xDlaDCdUutuHkeCIGuto8QU3rCLFsNV9x3cV0UEzf0YLwtkSIvXVRsUAAAAASUVORK5CYII=)
|CONTROL DE VERSIONES||||||
| :-: | :- | :- | :- | :- | :- |
|Versión|Hecha por|Revisada por|Aprobada por|Fecha|Motivo|
|1\.0|Rene Manchego, Moisés Corrales y Farley Viveros|||<p></p><p></p><p>12/11/2024</p>|<p></p><p></p><p>Versión 1.0</p>|


**ÍNDICE**

1. Introducción	4
   1. Propósito	4
   1. Alcance	4
   1. Definición, siglas y abreviaturas	4
   1. Referencias	4
   1. Visión General	5
1. Representación Arquitectónica	5
   1. Escenarios	5
   1. Vista Lógica	6
   1. Vista del Proceso	6
   1. Vista del desarrollo	6
   1. Vista Física	6
1. Objetivos y limitaciones arquitectónicas	7
   1. Disponibilidad	7
   1. Seguridad	7
   1. Adaptabilidad	7
   1. Rendimiento	7
1. Análisis de Requerimientos	8
   1. Requerimientos funcionales	7
   1. Requerimientos no funcionales	7
1. Vistas de Caso de Uso	9

1. Vista Lógica	17
   1. Diagrama Contextual	17
1. Vista de Procesos	18
   1. Diagrama de Proceso Actual	18
   1. Diagrama de Proceso Propuesto	18
1. Vista de Despliegue	19
   1. Diagrama de Contenedor	19
1. Vista de Implementación	20
   1. Diagrama de Componentes	20
1. Vista de Datos	22
   1. Diagrama Entidad Relación	22
1. Calidad	24
   1. Escenario de Seguridad	25
   1. Escenario de Usabilidad	26
   1. Escenario de Adaptabilidad	27
   1. Escenario de Disponibilidad	28
   1. Otro Escenario	28

**Informe de SAD**

1. ## **Introducción**

1. Propósito:

El propósito de nuestro proyecto es desarrollar un aplicativo móvil que facilite la inscripción y gestión de equipos participantes en los juegos de actividades florales universitarias, optimizando los procesos actuales y promoviendo una mayor participación estudiantil.

1. Alcance:

Desarrollar una solución tecnológica que permita a los equipos universitarios registrarse de manera autónoma, acceder a información relevante de los juegos, y recibir notificaciones sobre eventos, todo ello a través de una plataforma móvil accesible y fácil de usar.

1. Definición, siglas y abreviaturas:

App: Aplicación móvil, un software diseñado específicamente para dispositivos móviles como teléfonos inteligentes y tabletas, que permite a los usuarios interactuar con diversas funcionalidades de manera sencilla y eficiente.

0. UI (Interfaz de Usuario): Es la parte visual del sistema que permite a los usuarios interactuar con la aplicación, incluyendo botones, menús, formularios y otros elementos gráficos diseñados para ofrecer una experiencia intuitiva y accesible.
0. UX (Experiencia de Usuario): Hace referencia a la percepción y satisfacción del usuario al interactuar con la aplicación, englobando aspectos como facilidad de uso, funcionalidad y estética.
0. API (Interfaz de Programación de Aplicaciones): Conjunto de reglas y protocolos que permiten que diferentes aplicaciones o componentes del sistema se comuniquen entre sí, facilitando la integración de servicios externos o funcionalidades adicionales al aplicativo móvil.

1. Referencias:

- Guías de diseño de interfaces móviles (Google Material Design, Human Interface Guidelines).
- Estudios previos de gestión tecnológica en eventos estudiantiles.

- Documentación técnica de herramientas de desarrollo móvil como Flutter y React Native.
  1. Visión General:

- La visión que tenemos de nuestro sistema web, es que va a resultar innovadora al utilizar la APIS como escala, para la inscripción de equipos en los juegos de actividades florales universitarias. Se presentan el propósito, el alcance, los términos clave y las referencias relevantes, así como una visión detallada de los objetivos y características principales del sistema.

1. ## **Representación Arquitectónica**

1. Escenarios:

1. Requerimientos Funcionales

|**ID**|**Requerimiento**|**Descripción**|
| -: | :- | :-: |
|RF1|Autenticación y Usuarios|<p>- Inicio de sesión mediante cuentas Microsoft</p><p>- Roles diferenciados (administrador y usuario estándar)</p><p>- Cierre de sesión seguro</p>|
|RF2|Gestión de Eventos</p>|<p>- Crear, editar, eliminar y visualizar eventos</p><p>- Asignar fechas y ubicaciones a eventos</p><p>- Gestionar estados de eventos</p>|
|RF3|Gestión de Participantes</p>|<p>- Registro y administración de participantes</p><p>- Asignación de participantes a eventos</p><p>- Control de información personal</p>|
|RF4|Gestión de Equipos</p>|<p>- Crear y administrar equipos</p><p>- Asignar participantes a equipos</p><p>- Vincular equipos con eventos</p>|
|RF5|Gestión de Ubicaciones</p>|<p>- Registro de ubicaciones para eventos.</p><p>- Detalles y disponibilidad de espacios.</p><p>- Asignación de ubicaciones a eventos</p>|



1. Requerimientos No Funcionales - Atributos de Calidad



|**ID**|**Requerimiento**|**Descripción**|
| :-: | :-: | :-: |
|<p></p><p></p><p>RNF1</p>|<p></p><p></p><p>Seguridad</p>|<p>- Autenticación segura con Microsoft</p><p>- Protección de datos personales</p><p>- Control de acceso basado en roles</p>|
|<p></p><p></p><p>RNF2</p>|<p></p><p></p><p>Usabilidad</p>|<p>- Interfaz intuitiva y responsive</p><p>- Tiempos de respuesta rápidos</p><p>- Diseño adaptable a diferentes dispositivos</p>|
|<p></p><p></p><p>RNF3</p>|<p></p><p></p><p>Rendimiento</p>|<p>- Carga rápida de datos</p><p>- Optimización de recursos</p><p>- Manejo eficiente de la memoria</p>|
|<p></p><p></p><p>RNF4</p>|<p></p><p></p><p>Mantenibilidad</p>|<p>- Código modular y documentado</p><p>- Facilidad de actualización</p><p>- Gestión de versiones</p>|



1. Restricciones

- Disponibilidad de datos: El sitio depende de la disponibilidad y precisión de los datos sobre lugares, equipos a competir.

- Acceso a internet: Los usuarios deben tener acceso a una conexión a internet para utilizar todas las funcionalidades del sitio, especialmente la visualización de mapas y la búsqueda en tiempo real.
- Precisión de la información: La calidad de la información proporcionada, como horarios de apertura y tarifas, depende de la actualización y precisión de las fuentes de datos utilizadas.
- Integración con servicios externos: La integración con proveedores de servicios externos, como sistemas de transporte público, puede estar sujeta a restricciones técnicas o de colaboración.



1. ## **Representación de la Arquitectura del Sistema**

1. Vista de Caso de Uso:

3\.1.1. Diagramas de Casos de Uso

![image](https://github.com/user-attachments/assets/80829e09-069b-469a-b33d-a72223d08348)


1. Vista Lógica:

1. Diagrama de Subsistemas (paquetes)

1. Diagrama de Secuencia (vista de diseño)

1. Diagrama de Colaboración (vista de diseño)



1. Diagrama de Objetos

1. Diagrama de Clases


1. Diagrama de Base de Datos

1. Vista de Implementación: (vista de desarrollo)

1. Diagrama de Arquitectura de Software

![image](https://github.com/user-attachments/assets/77b0eedd-5379-44b2-a606-96b3a728fbbc)


1. Diagrama	de	Arquitectura	del	Sistema	(diagrama	de componentes)

![image](https://github.com/user-attachments/assets/51f475da-95e6-42f0-9871-5fa597be15ed)


1. Vista de Procesos:

3\.4.1.	Diagrama	de	Procesos	del	Sistema	(diagrama	de actividades)

1. Visto de Despliegue: (vista física)

3\.5.1 Diagrama de Despliegue

![image](https://github.com/user-attachments/assets/89b39d7b-9d2a-4d68-9f10-2e97ec193638)





1. ## **Atributos de Calidad del Software**

Escenario de Funcionalidad:

| Item | Descripcion|
|------------|-------------------------------------------------------------------------|
| Fuente     | Usuario                                                                 |
| Estímulo   | Necesidad de inscribir equipos, consultar información, visualizar ubicaciones y puntajes |
| Artefacto  | Aplicativo móvil (aplicación o software móvil)                           |
| Entorno    | Entorno digital                                                         |
| Respuesta  | El sistema debe permitir la inscripción de equipos, consulta de actividades, visualización de datos, y seguimiento |
| Medición   | Evaluar si la app permite registrar equipos, mostrar actividades, ubicaciones, y estadísticas correctamente y sin errores |



Escenario de Usabilidad:

|**Fuente** |` `Usuario|
| :-: | :- |
|**Estimulo** | |

||
| :- |

|Necesidad de navegar la app de manera intuitiva|
| :- |

||
| :- |

||
| :- |

||
| :- |

|||
| :-: | :- |

||
| :- |

|||
| :-: | :- |
|**Artefacto** | |

|Aplicativo móvil (aplicación o software móvil)|
| :- |

|||
| :-: | :- |

||
| :- |

|||
| :-: | :- |
|**Entorno** ||

||
| :- |

|Dispositivo móvil, en condiciones de uso variadas (luz, ruido, etc.)|
| :- |

||
| :- |

||
| :- |

||
| :- |

|||
| :-: | :- |

||
| :- |

|||
| :-: | :- |
|**Respuesta** | |

||
| :- |

|El sistema debe ser fácil de navegar, con menús y opciones claras y accesibles.|
| :- |

||
| :- |

||
| :- |

||
| :- |

|||
| :-: | :- |

||
| :- |

|||
| :-: | :- |
|**Medición** | |

||
| :- |

|Evaluar si los usuarios sin experiencia técnica pueden completar tareas sin dificultad.|
| :- |

||
| :- |

||
| :- |

||
| :- |

|||
| :-: | :- |

||
| :- |

|||
| :-: | :- |

Escenario de Confiabilidad:

|**Fuente** |` `Usuario|
| :-: | :- |
|**Estimulo** | |

||
| :- |

||
| :- |

|Necesidad de realizar registros, consultas y actualizaciones sin errores|
| :- |

||
| :- |

||
| :- |

||
| :- |

||
| :- |

||
| :- |

||
| :- |

|||
| :-: | :- |

||
| :- |

|||
| :-: | :- |
|**Artefacto** | |

||
| :- |

|Aplicativo móvil (funcionalidades de registro y consulta de datos)|
| :- |

||
| :- |

||
| :- |

||
| :- |

|||
| :-: | :- |

||
| :- |

|||
| :-: | :- |
|**Entorno** ||

||
| :- |

||
| :- |

|Condiciones de evento en tiempo real, con múltiples usuarios activos|
| :- |

||
| :- |

||
| :- |

||
| :- |

||
| :- |

||
| :- |

||
| :- |

|||
| :-: | :- |

||
| :- |

|||
| :-: | :- |
|**Respuesta** | |

||
| :- |

||
| :- |

|El sistema debe registrar y consultar datos sin fallos, incluso en momentos de alta carga de usuarios|
| :- |

||
| :- |

||
| :- |

||
| :- |

||
| :- |

||
| :- |

||
| :- |

|||
| :-: | :- |

||
| :- |

|||
| :-: | :- |
|**Medición** | |

||
| :- |

||
| :- |

|Medir la tasa de errores en el registro, consulta y actualización de datos durante el evento|
| :- |

||
| :- |

||
| :- |

||
| :- |

||
| :- |

||
| :- |

||
| :- |

|||
| :-: | :- |

||
| :- |

|||
| :-: | :- |


Escenario de Rendimiento:

Escenario de Mantenibilidad:




