
# Basic Travel Microservices
Este proyecto es una REST API desarrolada en Spring Boot y ha sido creado como parte de la formación "Master Java"

## Descripción del Proyecto
Este proyecto es una API REST que proporciona servicios para gestionar vuelos, hotels y reservas.
Los vuelos tienen información como id, compañia, fecha de vuelo e plazas.
Los hotels tiene información como id, nombre, categoria y disponibilidad.
Las reservas tiene información como id, idHotel, idVuelo y personas.

La API permite realizar operaciones CRUD a todos los modelos. A crear una reserva es verificado si hay plazas suficientes en el vuelo y si el hotel esta disponible.

Todos los microservicios tiene la dependencia OPENAPI Swagger que permiti visualisar en el browser toda la API e sus endpoints.

## Tecnologias Utilizadas
- Spring Boot
- Java
- RESTful API
- Maven
- Swagger

## Configuración del Proyecto
1. Asegúrate de tener instalado un MySQL Server
1.1. Script -> Crear base de dados
``Semana04_06_03_FinalProject_Reservas/src/main/resources/CREATE_SCHEMA.sql``
1.2. Script -> Crear table **hotels**
``Semana04_06_01_FinalProject_Hotel/src/main/resources/CREATE_TABLE_HOTELS.sql``
1.3. Script -> Crear table **vuelos**
``Semana04_06_02_FinalProject_Vuelos/src/main/resources/CREATE_TABLE_VUELOS.sql``
1.4. Script -> Crear table **reservas**
``Semana04_06_03_FinalProject_Reservas/src/main/resources/CREATE_TABLE_RESERVAS.sql``

2. Asegúrate de tener instalado Java y Maven en tu sistema antes de ejecutar el proyecto.
2.1. Clona este repositorio en tu máquina local:
   ``git clone https://github.com/tiago0liveira77/BasicTravelMicroservices.git``
2.2. Navega al directorio de todos los microservicios:
2.3. Ejecuta la aplicación Spring Boot:
``mvn *microservicio*:run``

Documentacion de API (usando las mismas ports):
*De acuerdo con la **Puerta utilizada**:*
- Hotels API: http://localhost:8080/swagger-ui/index.html
- Vuelos API: http://localhost:9000/swagger-ui/index.html
- Reservas API http://localhost:9001/swagger-ui/index.html
