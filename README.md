# FAAPS Backend

Spring Boot API using Java 21 and MySQL.

## Local development

Create a MySQL database named `faaps`. Set `DB_PASSWORD` and optionally `DB_URL` and `DB_USERNAME` as environment variables. See `.env.example` for example values; the application does not read `.env` files automatically.

The default JDBC URL is for local development and permits MySQL public key retrieval when TLS is disabled. For a remote or production database, set `DB_URL` to a TLS-enabled connection URL instead of using the local default.

```powershell
mvn spring-boot:run
```

The health endpoint is `http://localhost:8080/api/health`. The current backend is a stack scaffold; authentication and academic modules are not implemented yet.
