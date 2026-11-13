# Customers and Orders REST API — Spring Boot + JPA

REST service for customers and their orders, built with Spring Boot, Spring Data JPA (Hibernate) and MySQL.

- Layered architecture: controller → service → repository → entity.
- Full CRUD for customers and orders, with the one-to-many relationship mapped in JPA.
- Proper HTTP status codes and error handling.
- Tests with `mvn test`, plus a script that runs 16 HTTP checks against the running API (`pruebas/pruebas-curl.ps1`).
- Call-stack diagram and technical write-up in `docs/`.

## Run it

1. Start MySQL with Docker (`docker compose up -d` using the compose file from the data-access labs, port 3307).
2. `cd apirest && mvn spring-boot:run`
3. Try the endpoints with the script in `pruebas/` or any HTTP client.

Built during the *Data Access* module (Multiplatform App Development, Nebrija, 2026). Original notes in Spanish: [README.es.md](README.es.md).
