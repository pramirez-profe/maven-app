# API Simple de Spring Boot

Esta es una aplicación simple de Spring Boot que expone un único endpoint GET en `/hello`.

## Requisitos previos

- Java 21
- Maven

## Ejecutar la aplicación localmente

1.  **Construir el proyecto:**
    ```bash
    mvn package
    ```

2.  **Ejecutar la aplicación:**
    ```bash
    java -jar target/maven-app-0.0.1-SNAPSHOT.jar
    ```

La aplicación estará disponible en `http://localhost:8080`.

## Construir y ejecutar con Docker

1.  **Construir la imagen de Docker:**
    ```bash
    docker build -t maven-app .
    ```

2.  **Ejecutar el contenedor de Docker:**
    ```bash
    docker run -p 8080:8080 maven-app
    ```

## Endpoint

-   **GET /hello**

    Devuelve una respuesta JSON:
    ```json
    {
      "message": "hello!"
    }
    ```
