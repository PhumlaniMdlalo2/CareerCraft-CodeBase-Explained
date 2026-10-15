# Glossary

## Backend (Spring Boot)
- **Controller**: REST endpoint layer; maps HTTP requests to service calls
- **Service**: Business logic layer (interfaces + implementations)
- **Repository**: Data access layer via Spring Data JPA
- **Entity/Domain**: JPA-mapped classes representing database tables
- **DTO**: Data transfer object (backend shapes returned as JSON)
- **Dependency Injection**: Spring wires components (constructor injection preferred)
- **@RestController**: Combines @Controller and @ResponseBody
- **JpaRepository**: Generic repo with CRUD and query methods
- **@Transactional**: Manages transaction boundaries

## Frontend (Angular)
- **Component**: UI building block (standalone in this codebase)
- **Service**: Injectable class for logic/data access (HttpClient calls)
- **HttpClient**: Angular's HTTP client for REST calls
- **Observable/RxJS**: Async streams for HTTP responses
- **Signal**: Angular reactive primitive for state
- **Guard**: Route protection logic
- **Model/Interface**: TypeScript types for data shapes

## Integration
- **API Base URL**: Root for backend REST endpoints (/api)
- **CORS**: Cross-Origin Resource Sharing; controllers use @CrossOrigin
- **Mapping**: Converting backend DTOs to UI models
- **Request Flow**: End-to-end path from UI action to DB and back
