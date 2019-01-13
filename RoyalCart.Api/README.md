# AspNetCoreIdentity

The fallowing is an authentication and user role management implementation for starting projects. Build using the Identity Framework to implement a user's roles and claims membership service and the Entity Framework to implement a object-relational mapping service.

## How to run:

Before running this API, a database needs to be setup. 
With the help EF Core, using the Code-First approach we will create a migration, and create DB instance in SQL Server using a previously created migration.

1. Edit Connection String from 'appsettings.json' to match your DB instance.
  ```json
  "ConnectionStrings": {
    "AspNetCoreIdentityDb": "Server=Localhost;Database=CoreIdentity;Trusted_Connection=True;MultipleActiveResultSets=true"
  }
  ```
2. Create Migration - from project main directory, using CLI. (Optional if migration already exist)

  ```
  >dotnet ef migrations add initial_migration
  ```
3. Update Database - from project main directory, using CLI.

```
>dotnet ef database update
```
  
4. Run Application using Visual Studio 2017

## SwaggerIO:

in order to access API documentation with the help of SwaggerIO go to:

```
http://localhost:49810/swagger/index.html

```

## Modifying User Model:

## Running from Docker Image:
