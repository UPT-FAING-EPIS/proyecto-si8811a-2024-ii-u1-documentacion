Manual de Usuario - Inicio de Sesión
1. historia de usuario

   Desarrollo Web

   Activar filtro de eventos

   https://youtu.be/HW3N5lUZK30



   | **Filtrar Eventos**           | **Descripción**                                                                                                                                                                   |
|---------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Como:**                       | Usuario del sistema de juegos florales                                                                                                                                           |
| **Quiero:**                     | Usar un filtro para visualizar los eventos vigentes                                                                                                                              |
| **Para que:**                   | Pueda ver solo los eventos actuales que se encuentran activos y programados                                                                                                       |
| **Criterios de Aceptación**     | - El usuario debe poder ver solo los eventos vigentes una vez aplicado el filtro.<br> - El filtro debe mostrar eventos organizados por fecha y categoría.                          |
| **Pantalla de Inicio de Sesión:** | La pantalla inicial debe solicitar al usuario su correo institucional para acceder al sistema. El usuario tiene opción de iniciar sesión manualmente o automáticamente.             |
| **Redirección a Microsoft:**    | Si el usuario selecciona autenticarse con su cuenta institucional, el sistema lo redirige a la página de inicio de sesión de Microsoft para autenticar sus credenciales.           |
| **Autenticación:**              | Una vez autenticado, el sistema debe validar las credenciales y verificar que el usuario esté autorizado a ingresar al sistema de juegos florales. En caso de éxito, el usuario es redirigido al dashboard principal. |
| **Inicio de Sesión Automático:** | Si el usuario ya ha iniciado sesión previamente en el sistema, el inicio de sesión automático permite que acceda directamente sin necesidad de introducir nuevamente las credenciales. |
| **Infraestructura:**            | El sistema debe estar integrado con Azure Active Directory para la autenticación, y debe contar con filtros dinámicos que permitan al usuario seleccionar y visualizar los eventos vigentes. También debe contar con un sistema de seguridad robusto para proteger los datos de autenticación y la información de los eventos. |


   Filtrar Eventos por Escuela entre otros

   https://youtu.be/kVukoFvcdJc

   https://youtu.be/39KIQJcTtpM

   https://youtu.be/37J0TCnbiII

   https://youtu.be/Iy6awq4nASg

   https://youtu.be/h_f-CLEEn5Y

   https://youtu.be/St7qzknR9_A

   https://youtu.be/akh48sIgeqU

   
3. Especificaciones

   
   2.1 Inicio de Sesión

      Requisitos del Sistema
   
     - Pagina Web: React librería necesaria para construir la interfaz de usuario
     - App Mobile: Flutter framework utilizado para crear aplicaciones móviles, web y de escritorio
     - Backend: Python lenguaje de programación de alto nivel, interpretado y de propósito general, conocido por su 
       simplicidad y legibilidad.
   
   2.2 Listar Eventos
  
     Requisitos del Sistema
  
   - Pagina Web: React librería necesaria para construir la interfaz de usuario
   - App Mobile: Flutter framework utilizado para crear aplicaciones móviles, web y de escritorio
   - Backend: C# para el codigo donde se uso MongoDB.Driver



Manual Tecnico - Inicio de Sesion y Listar Eventos
1. Diagrama de Clases

   Desarrollo Web

   ![image](https://github.com/user-attachments/assets/b9c2f3b1-4d0b-4a67-9573-a62e1772ec2d)


   Desarrollo Movil

   ![image](https://github.com/user-attachments/assets/a6a72dcc-68a4-48c2-b672-2725b587b2e2)

   ![diagrama listo 1](https://github.com/user-attachments/assets/63aaf00b-a2c7-41ae-9d5e-c0e3d4c83514)

   ![diagrama 2 listo](https://github.com/user-attachments/assets/f143cb86-66b7-4f3a-83d9-1b87658960c9)



3. Arquitectura del Sistema

Desarrollo web

![image](https://github.com/user-attachments/assets/da713d72-7f61-430b-973e-4600453d52ba)

Desarrollo Movil

![image](https://github.com/user-attachments/assets/e2ff1da5-5913-4aa1-a881-24c3ecad2228)


4. Diagrama de Componentes
5. Diagrama de Despliegue

![image](https://github.com/user-attachments/assets/c5c7cde7-e325-4921-91e2-2de372012335)

