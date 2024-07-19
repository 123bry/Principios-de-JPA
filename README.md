# Principios-de-JPA


## Parte 1: Configuración del Proyecto
1.   Crear un Proyecto Spring Boot:

      •   Visita Spring Initializr.

      •   Configura el proyecto con los siguientes detalles:

             •   Project: Maven

             •   Language: Java

             •   Spring Boot: 2.5.4 (o la versión más reciente)

             •   Group: com.ejemplo

             •   Artifact: jpa-tutorial

             •   Name: jpa-tutorial

             •   Package name: com.ejemplo.jpa-tutorial

             •   Packaging: Jar

             •   Java: 8 o superior

      •   Añade las dependencias:

             •   Spring Web

             •   Spring Data JPA

             •   Base de datos relacional

## Parte 2: Crear la Entidad y el Repositorio


1.   Crear la Entidad Producto:

      •   Crea un paquete llamado model.

      •   Dentro del paquete model, crea una clase Producto.

![image](https://github.com/user-attachments/assets/78e96219-1446-4275-b5c4-620371dc384a)
![image](https://github.com/user-attachments/assets/8318ad83-535f-423a-b82b-c4e5bcf5cbcf)



3.   Crear el Repositorio ProductoRepository:

      •   Crea un paquete llamado repository.

      •   Dentro del paquete repository, crea una interfaz ProductoRepository.

![image](https://github.com/user-attachments/assets/f43926f6-8855-4997-a2bd-1a2223041eae)



## Parte 3: Crear el Servicio

 

1.   Crear la Clase ProductoService:

      •   Crea un paquete llamado service.

      •   Dentro del paquete service, crea una clase ProductoService.

![image](https://github.com/user-attachments/assets/152fec96-b351-415e-be18-d39682c6a246)



## Parte 4: Crear el Controlador

 
1.   Crear la Clase ProductoController:

      •   Crea un paquete llamado controller.

      •   Dentro del paquete controller, crea una clase ProductoController.

 ![image](https://github.com/user-attachments/assets/0e0435ee-31b4-4050-badf-969e1935b292)


## Parte 5: Inicializar la Base de Datos

 
1.   Cargar Datos de Prueba:

      •   Crea una clase de configuración para inicializar algunos objetos Producto al inicio de la aplicación.

          ![image](https://github.com/user-attachments/assets/95b30619-bc58-4ef1-a40c-aa0d651b0e17)


## Parte 6: Ejecutar y Probar la Aplicación

1.   Ejecutar la Aplicación:

      •   Ejecuta tu aplicación desde tu IDE o desde la línea de comandos con mvn spring-boot:run.

   ![image](https://github.com/user-attachments/assets/22dbbcfd-d3b5-42c5-bbda-469e679548e8)


3.   Probar los Endpoints:

      •   Usa herramientas como Postman o cURL para probar los endpoints REST que has creado:

             •   GET /api/productos
 
   ![image](https://github.com/user-attachments/assets/cdc1aeb3-2ff2-4ef8-8cbb-052eb0b1c415)


             •   GET /api/productos/{id}
  
   ![image](https://github.com/user-attachments/assets/e9a290ba-be85-4790-a0b0-dc20fdbda9ef)


             •   GET /api/productos/search?nombre={nombre}

   ![image](https://github.com/user-attachments/assets/af6e31b1-2531-4218-b0bb-fc170ef9481f)


            •.   GET /api/productos/searchByPrecio?preciomin={preciomin }&preciomax={ preciomax}

 ![image](https://github.com/user-attachments/assets/5b1bcf81-b665-46a8-82f2-8a8d867c0d39)

