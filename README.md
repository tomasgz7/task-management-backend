# Task Management Service - Spring Boot

REST API desarrollada para gestionar tareas mediante operaciones CRUD, diseñada con una arquitectura en capas que favorece la separación de responsabilidades y la mantenibilidad del sistema.

El proyecto refleja buenas prácticas en la construcción de servicios backend, priorizando claridad estructural, trazabilidad de datos y una base preparada para evolucionar hacia escenarios más robustos.

Este servicio fue concebido como una base estructural para comprender cómo diseñar APIs organizadas, priorizando legibilidad, desacople y facilidad de evolución en contextos reales de desarrollo.


---

## Arquitectura

El servicio está organizado bajo un enfoque en capas:

**Controller → Service → Repository**

Esta estructura permite desacoplar la lógica de negocio del acceso a datos, facilitando la escalabilidad y futuras extensiones.

---

## Stack tecnológico

- Java 17  
- Spring Boot 3  
- Spring Web  
- Spring Data JPA  
- H2 Database  
- Maven  

---

## Modelo de dominio

**Task**

- id  
- title  
- description  
- completed  

---

## Endpoints principales

| Método | Endpoint | Descripción |
|--------|------------|---------------|
| GET | /api/tasks | Obtener todas las tareas |
| GET | /api/tasks/{id} | Obtener tarea por ID |
| POST | /api/tasks | Crear tarea |
| PUT | /api/tasks/{id} | Actualizar tarea |
| DELETE | /api/tasks/{id} | Eliminar tarea |

---

## Enfoque

El objetivo principal fue construir un servicio backend priorizando organización interna, claridad en la lógica de negocio y una estructura preparada para escalar sin comprometer la mantenibilidad.


## Ejecución local

```bash
mvn spring-boot:run
http://localhost:8080/api/tasks
