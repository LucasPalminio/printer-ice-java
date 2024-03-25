# Proyecto Printer - Hola Mundo de ZeroC Ice para Java

Este proyecto es una implementación del "Hola Mundo" de ZeroC Ice para Java, siguiendo la guía proporcionada en la documentación oficial de ZeroC, pero con correcciones para resolver errores y mejorar la claridad del código.

## Descripción

El proyecto Printer es una aplicación de ejemplo que utiliza ZeroC Ice para demostrar la comunicación distribuida en Java. Consiste en dos subproyectos: `client` y `server`, que interactúan para imprimir mensajes en una impresora virtual.

Este proyecto se basa en el tutorial oficial de ZeroC Ice para Java: [Writing an Ice Application with Java](https://doc.zeroc.com/ice/3.7/hello-world-application/writing-an-ice-application-with-java).

## Correcciones y Mejoras

Para garantizar que el código sea preciso y funcional, se realizaron las siguientes correcciones y mejoras con respecto a la documentación original:

- Corrección de errores en la configuración de Gradle.
- Adecuación de la estructura del proyecto para una mejor organización.
- Ajustes en la configuración del servidor y cliente para asegurar la comunicación adecuada.
- Mejoras en la documentación y comentarios del código para una comprensión más clara.

## Requisitos

- Java Development Kit (JDK) versión 8 o superior.
- Gradle para compilar y construir el proyecto.

## Configuración

1. Clona este repositorio en tu máquina local:

```bash
git clone https://github.com/LucasPalminio/printer-ice-java.git
```
2. Navega al directorio del proyecto:
```bash 
cd printer
```
3. Ejecuta el comando de compilación para construir los subproyecto `client` y `server`
```bash
gradlew :server:build
gradlew :client:build
```
4. Ejecuta el comando de ejecución de los proyectos, primero el `server` y luego `client` 
```bash
java -jar server/build/libs/server.jar
java -jar client/build/libs/client.jar
```

Como resultado en la terminal del server mostrara en pantalla un "Hola Mundo" cada vez que se ejecuta el Cliente