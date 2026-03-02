Proyecto: Endpoint Hola Mundo – Spring Boot

1️⃣ Creación del proyecto

Se creó el proyecto utilizando Spring Initializr con las siguientes características:

Project: Maven

Language: Java

Spring Boot: última versión estable

Java: 17

Dependencia: Spring Web

2️⃣ Implementación del endpoint

Se creó la clase HolaController con la anotación @RestController.

Se implementó un endpoint GET:

@GetMapping("/hola")
public String hola() {
    return "Hola Mundo!";
}

3️⃣ Ejecución

Para ejecutar el proyecto:

Abrir en IntelliJ o VS Code

Ejecutar la clase principal

Acceder en el navegador:

http://localhost:8080/hola

Resultado mostrado:

Hola Mundo!
