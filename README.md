# Manual Tecnico
## 1. Diagrama de Clases

   ### Desarrollo Web
   
```mermaid

classDiagram
    class CountdownTimer {
        +calculateTimeLeft()
        +render()
        -timeLeft: Object
    }
    
    class EventCard {
        +render()
    }
    
    class Footer {
        +render()
    }
    
    class Header {
        +render()
    }
    
    class Home {
        +render()
    }
    
    class Navbar {
        +render()
    }
    
    class Event {
        +nombre: String
        +fechaInicio: String
        +fechaTermino: String
        +facultad: String
    }
    
    class AuthSlice {
        +onChecking()
        +onLogin(payload)
        +onLogout(payload)
    }
    
    class EventSlice {
        +onAddNewEvent(payload)
        +onDeleteEvent()
        +onLoadEvents(payload)
        +onSetActiveEvent(payload)
    }
    
    class Store {
        +configureStore()
    }
    
    class useAuthStore {
        +loginWithGoogle()
        +checkAuthToken()
        +startLogout()
    }
    
    class useEventStore {
        +startLoadingEvents()
    }
    
    class categoriasApi {
        +getCategorias()
    }
    
    class equipoApi {
        +getEquipos()
    }
    
    class eventoApi {
        +getEvents()
    }
    
    class lugaresApi {
        +getLugares()
    }
    
    class participanteApi {
        +getParticipantes()
    }

    Header --> Navbar
    Home --> Header
    Home --> Footer
    Home --> CountdownTimer
    Home --> EventCard
    Home --> Event
    
    EventCard --> Event
    
    AuthSlice --> Store
    EventSlice --> Store
    
    useAuthStore --> AuthSlice
    useEventStore --> EventSlice

    categoriasApi --> Home
    equipoApi --> Home
    eventoApi --> Home
    lugaresApi --> Home
    participanteApi --> Home

    ```
```
Descripción: Este diagrama de clases muestra la estructura de una aplicación web .Consta de tres clases principales: "App", "Login" y "Eventos". La clase "App" es la clase central, con un método render(), y se conecta a las otras dos clases mediante relaciones etiquetadas como "Renders". La clase "Login" tiene métodos para manejar el inicio de sesión (handleLogin()) y renderizar su interfaz. La clase "Eventos" maneja la visualización y carga de eventos, con atributos para eventos, estado de carga y errores, y métodos para renderizar y obtener eventos (fetchEvents()). Esta estructura sugiere una arquitectura de componentes típica de frameworks modernos de desarrollo web, donde cada componente es responsable de su propia lógica y representación visual.

### Desarrollo Movil

   ![image](https://github.com/user-attachments/assets/a6a72dcc-68a4-48c2-b672-2725b587b2e2)
   
   Descripción: Este diagrama de clases muestra la estructura de una aplicación, desarrollada con Flutter, que gestiona equipos, participantes y eventos. La aplicación se compone de una clase principal (MyApp), una página de inicio (MyHomePage), un servicio de autenticación (AuthService), y varias pantallas específicas para diferentes funcionalidades. La estructura incluye modelos de datos (Equipo, Participante, Evento) y utiliza navegación entre pantallas, sugiriendo una aplicación bien organizada para la gestión de torneos o eventos deportivos.

   ![diagrama listo 1](https://github.com/user-attachments/assets/63aaf00b-a2c7-41ae-9d5e-c0e3d4c83514)

Descripción: Este diagrama de clases muestra la estructura de una aplicación con tres clases principales: Main, MyApplication y GeneratedPluginRegistrant. La clase Main contiene el método main(), punto de entrada de la aplicación. MyApplication hereda de GtkApplication y gestiona el ciclo de vida de la aplicación con métodos como OnCreate() y OnDestroy(). También utiliza GeneratedPluginRegistrant para registrar plugins. Esta estructura sugiere una aplicación basada en GTK, posiblemente desarrollada con Flutter para desktop, que maneja plugins y tiene una configuración inicial definida.

   ![diagrama 2 listo](https://github.com/user-attachments/assets/f143cb86-66b7-4f3a-83d9-1b87658960c9)
   
Descripción: Este diagrama de clases muestra la estructura de una aplicación Flutter para Windows. Consta de cuatro clases principales: Main (punto de entrada), Runner (inicializa la aplicación), FlutterWindow (maneja la ventana principal de Flutter) y Win32Window (implementación específica para Windows). La jerarquía ilustra cómo la aplicación Flutter se integra con la plataforma Windows, gestionando el ciclo de vida de la ventana y los eventos del sistema. Esta estructura permite que una aplicación Flutter se ejecute como una aplicación de escritorio nativa en Windows.
   

   ### API EVENTOS
```
```
```mermaid

classDiagram
    class Evento {
        +String? Id
        +String Nombre
        +DateTime FechaInicio
        +DateTime FechaTermino
        +String Facultad
        +String Resultado
        +String Descripcion
    }

    class MongoDBSettings {
        +String ConnectionString
        +String DatabaseName
    }

    class EventoService {
        +List<Evento> GetAsync()
        +Evento GetByIdAsync(String id)
        +Evento CreateAsync(Evento nuevoEvento)
        +Evento UpdateAsync(String id, Evento evento)
        +void DeleteAsync(String id)
    }

    class EventoController {
        +ActionResult<IEnumerable<Evento>> GetEventos()
        +ActionResult<Evento> GetEvento(String id)
        +ActionResult<Evento> CreateEvento(Evento evento)
        +ActionResult<Evento> UpdateEvento(String id, Evento evento)
        +ActionResult DeleteEvento(String id)
    }

    EventoController --> EventoService : uses
    EventoService --> Evento : manages
    EventoService --> MongoDBSettings : configures

```

- Clase `Evento`: La clase `Evento` representa la estructura de un evento en el sistema, conteniendo propiedades como el identificador, nombre, fechas de inicio y término, facultad asociada, resultado y una descripción del evento. Esta clase se utiliza para almacenar y transferir datos relacionados con los eventos en la aplicación.

- Clase `MongoDBSettings`: La clase `MongoDBSettings` encapsula la configuración necesaria para conectarse a una base de datos de MongoDB, incluyendo la cadena de conexión y el nombre de la base de datos. Proporciona una forma de gestionar y acceder a estos parámetros de configuración de manera estructurada.

- Clase `EventoService`: La clase `EventoService` se encarga de la lógica de negocio relacionada con la gestión de eventos. Se encarga de interactuar con la base de datos de MongoDB, facilitando operaciones de lectura y escritura sobre los documentos de eventos y asegurando que la lógica del sistema se mantenga separada de los detalles de la base de datos.

- Clase `EventoController`: El `EventoController` actúa como intermediario entre las solicitudes HTTP y el servicio de eventos. Se encarga de recibir y procesar las solicitudes relacionadas con los eventos, delegando la lógica de negocio al `EventoService` y devolviendo las respuestas adecuadas al cliente.

   API LUGARES

```mermaid
classDiagram
    class Lugar {
        +String id_lugar
        +String nombre_lugar
        +String direccion_id
        +int capacidad
        +String descripcion
        +float latitud
        +float longitud
        +String id_categoria
        +int estado
    }

    class Direccion {
        +String direccion_id
        +String calle
        +String numero
        +String ciudad
        +String codigo_postal
        +String pais
        +int estado
    }

    class Categoria {
        +String id_categoria
        +String nombre_categoria
        +int estado
    }

    class LugarCreate {
        +String nombre_lugar
        +String direccion_id
        +int capacidad
        +String descripcion
        +float latitud
        +float longitud
        +String id_categoria
    }

    class DireccionCreate {
        +String calle
        +String numero
        +String ciudad
        +String codigo_postal
        +String pais
    }

    class CategoriaCreate {
        +String nombre_categoria
    }

    Lugar <|-- LugarCreate
    Direccion <|-- DireccionCreate
    Categoria <|-- CategoriaCreate

```
- Clase Lugar: Representa un lugar en el sistema, con propiedades que incluyen el identificador, nombre, dirección, capacidad, descripción, coordenadas geográficas y estado. Esta clase es fundamental para la gestión de lugares dentro de la API, permitiendo operaciones relacionadas con su creación y consulta.

- Clase Direccion: Define la estructura de una dirección, con atributos como identificador, calle, número, ciudad, código postal y país. Incluye un estado que permite gestionar su validez y asociación con los lugares.

- Clase Categoria: Representa la categoría a la que pertenece un lugar, con propiedades que incluyen un identificador y nombre de la categoría. Su estado permite organizar los lugares según diferentes clasificaciones.

- Clase LugarCreate: Extiende la clase Lugar, proporcionando un modelo simplificado para la creación de nuevos lugares. Incluye las propiedades necesarias sin el identificador y estado, facilitando la entrada de datos.

- Clase DireccionCreate: Similar a Direccion, esta clase proporciona un modelo para la creación de nuevas direcciones, omitiendo el identificador y estado para simplificar la entrada de datos.

- Clase CategoriaCreate: Proporciona un modelo para la creación de nuevas categorías, incluyendo solo el nombre de la categoría, lo que permite la adición sencilla de nuevas clasificaciones a la API.

## 2. Arquitectura del Sistema

Desarrollo web

![image](https://github.com/user-attachments/assets/20590a30-b605-4251-ad2b-f80df775d2cc)



Descripción Este diagrama muestra la arquitectura del proyecto de desarrollo web, probablemente utilizando React y Vite. La estructura se divide en carpetas 'public' y 'src', con 'index.html' como punto de entrada. El archivo 'main.jsx' inicializa la aplicación, que renderiza componentes como 'eventos.jsx' y 'login.jsx'. Se incluyen archivos de configuración para herramientas como ESLint, PostCSS y Tailwind, así como archivos de gestión de paquetes y documentación. Esta organización refleja una arquitectura moderna de desarrollo frontend con separación clara de componentes y configuraciones.

Desarrollo Movil

![image](https://github.com/user-attachments/assets/e2ff1da5-5913-4aa1-a881-24c3ecad2228)

API eventos

![image](https://github.com/user-attachments/assets/3820c1ea-801f-4044-8c49-703d98af396f)

Descripción: La estructura sigue un patrón MVC (Model-View-Controller) con capas adicionales de Servicios y Configuración. El núcleo es 'Program.cs', que interactúa con componentes como 'EventoController.cs', 'EventoService.cs', y 'Evento.cs' (modelo). La configuración incluye 'MongoDBSettings.cs' y 'launchSettings.json'. El proyecto parece estar preparado para despliegue con Docker, como lo indica la presencia del 'Dockerfile'.

API Lugares

![image](https://github.com/user-attachments/assets/1a0cc968-7120-4765-805b-93633b92ff1f)

Descripción: Se divide en dos carpetas principales: 'app' y 'tests'. La carpeta 'app' contiene los archivos core de la aplicación (main.py, models.py, crud.py, schemas.py), mientras que 'tests' incluye archivos para pruebas unitarias. El proyecto utiliza Docker para el despliegue (Dockerfile y docker-compose.yml) y maneja dependencias con requirements.txt. Esta estructura sugiere una API bien organizada con separación clara entre código de producción y pruebas.

## 3. Diagrama de Despliegue
Obtenido del Repositorio de Api back donde uso terraform como infraestructura
https://github.com/UPT-FAING-EPIS/proyecto-si8811a-2024-ii-u1-desarrollo-api-back/tree/main

Infraestructura 

![image](https://github.com/user-attachments/assets/f74bf3a0-662c-4dc8-9a89-13dc59a5fad5


Descripción: Este diagrama representa la infraestructura de un sistema de aplicación distribuida. Muestra un grupo de recursos principal que contiene tres módulos clave: Backend API, Web App y Mobile App. Cada módulo tiene su propia configuración interna, referenciando variables y recursos específicos. Fuera del grupo de recursos principal, se observa una definición del propio grupo de recursos y un módulo adicional que se divide en tres submódulos correspondientes a los componentes principales. La estructura del diagrama sugiere el uso de Infrastructure as Code (IaC) para definir y gestionar los recursos de manera declarativa, posiblemente utilizando herramientas como Terraform.

Backend_api 

![image](https://github.com/user-attachments/assets/495c7c73-6392-4fb8-9be8-e697661165ea)

mobile_app infraestructura

![image](https://github.com/user-attachments/assets/5b5da772-c1b8-4c67-85c3-3819846f86fb)

web_app Infraestructura

![image](https://github.com/user-attachments/assets/fc87ebc4-1524-4fd0-83d3-a033a319bf37)
