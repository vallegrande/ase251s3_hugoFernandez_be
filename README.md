🚀 Proyecto: Endpoint “Hola Mundo” con Spring Boot
📌 Descripción

En esta actividad se implementó un endpoint de tipo GET utilizando el framework Spring Boot, el cual muestra el mensaje “Hola Mundo” en el navegador.

🛠 Tecnologías utilizadas

Java 17

Spring Boot

Maven

Spring Web

IDE (IntelliJ IDEA / VS Code)

Git y GitHub

🧱 1️⃣ Creación del Proyecto

El proyecto fue creado utilizando Spring Initializr con las siguientes características:

Project: Maven

Language: Java

Spring Boot: Última versión estable

Packaging: Jar

Java: 17

Dependencia agregada: Spring Web

Una vez descargado el proyecto, se abrió en el IDE y se esperó a que Maven descargara las dependencias necesarias.

💻 2️⃣ Implementación del Endpoint

Se utilizó la clase principal generada automáticamente por Spring Boot y se agregó la anotación @RestController para permitir la creación de un endpoint REST.

Código implementado:
package vallegrande.edu.pe.demo;

import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;
import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RequestParam;
import org.springframework.web.bind.annotation.RestController;

@SpringBootApplication
@RestController
public class HugoFernandezApplication {

    public static void main(String[] args) {
        SpringApplication.run(HugoFernandezApplication.class, args);
    }

    @GetMapping("/Hola")
    public String hello(@RequestParam(value = "name", defaultValue = "Mundo") String name) {
        return String.format("Hola %s!", name);
    }

}
🌐 3️⃣ Prueba del Endpoint

Una vez ejecutada la aplicación, el servidor se inició en el puerto 8080.

Acceso básico:
http://localhost:8080/Hola

Resultado:

Hola Mundo!
