# Azure SQL Database CRUD Application

A Spring Boot application for demonstrating CRUD operations with Azure SQL Database.

## Features

- Create, Read, Update, Delete operations for products
- Simple web interface
- Azure SQL Database integration
- Automatic database schema creation

## Prerequisites

- Java 17 or higher
- Maven 3.6+
- Azure subscription
- Azure CLI

## Quick Start

1. Set up Azure resources (see deployment guide)
2. Configure environment variables
3. Run the application:
   ```bash
   mvn spring-boot:run
   ```

## Environment Variables

- `DB_SERVER`: Azure SQL server name
- `DB_NAME`: Database name (SampleDB)
- `DB_USERNAME`: Database username
- `DB_PASSWORD`: Database password

## Local Development

For local development, you can override the environment variables in `application.properties`:

```properties
spring.datasource.url=jdbc:sqlserver://your-server.database.windows.net:1433;database=SampleDB;encrypt=true;
spring.datasource.username=your-username
spring.datasource.password=your-password
```

## Deployment

See the deployment guide for detailed instructions on deploying to Azure App Service.

## Testing

Access the application at `http://localhost:8080` (local) or your Azure App Service URL.

The application provides a simple web interface to:
- Add new products
- View all products
- Edit existing products
- Delete products
