# T2_Barrantes

# Alquiler de Películas

Aplicación web de gestión de alquiler de películas desarrollada con Spring Boot, Thymeleaf y MySQL.

## Características

- Gestión de clientes, películas y alquileres.
- Registro y devolución de alquileres.
- Listado de alquileres activos y retrasados.
- Interfaz web moderna y responsiva con Thymeleaf.
- Persistencia de datos en MySQL.

## Requisitos

- Java 17+
- Maven 3.6+
- MySQL 5.7/8.0

## Configuración

1. **Base de datos:**  
   Crea una base de datos llamada `BD_T2_BARRANTES` en tu servidor MySQL.

2. **Configura las credenciales en** [`src/main/resources/application.properties`](src/main/resources/application.properties):

   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/BD_T2_BARRANTES?useSSL=false&serverTimezone=UTC
   spring.datasource.username=(tu usuario)
   spring.datasource.password=(tu password)
   ```

   Ajusta el usuario y contraseña según tu entorno.

3. **Puerto del servidor:**  
   La aplicación corre por defecto en el puerto `8085`. Puedes cambiarlo en el mismo archivo de application.properties.

## Ejecución

1. Compila el proyecto:

   ```sh
   ./mvnw clean package
   ```

2. Ejecuta la aplicación:

   ```sh
   ./mvnw spring-boot:run
   ```

3. Accede a la aplicación en [http://localhost:8085](http://localhost:8085).

## Estructura del Proyecto

- `src/main/java/com/cibertec/blockbuster/` — Código fuente Java (controladores, modelos, repositorios)
- `src/main/resources/templates/` — Vistas Thymeleaf (`.html`)
- `src/main/resources/application.properties` — Configuración de la aplicación

## Créditos

Proyecto para el curso de Lenguaje de Programación II.

## Autor

Carlos Jonathan Barrantes Angulo

---
