# Premier-League-Player-Stats-API
A Spring Boot REST API that exposes Premier League player statistics stored in a PostgreSQL database.   This project demonstrates backend development fundamentals, including RESTful design, JPA entity mapping to an existing schema, and database integration using Hibernate.

## Tech Stack

- Java 21  
- Spring Boot 4  
- Spring Data JPA (Hibernate)  
- PostgreSQL  
- Maven  
- Embedded Tomcat  

---

## Key Highlights

- Maps an existing PostgreSQL dataset (no auto-generated schema)
- Uses `spring.jpa.hibernate.ddl-auto=validate` to enforce schema correctness
- Clean Controller–Service–Repository architecture
- RESTful endpoints with filtering support
- Production-style connection pooling via HikariCP

---

## API Endpoints

### Get all players
GET /api/v1/player

### Filter players
GET /api/v1/player?team=Arsenal
GET /api/v1/player?position=FW
GET /api/v1/player?nation=England
GET /api/v1/player?name=Salah

### Create a player
POST /api/v1/player

### Update a player
PUT /api/v1/player


Access the API:
http://localhost:8080/api/v1/player

