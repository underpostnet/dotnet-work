### CRUD REST Service using ASP.NET CORE with JWT Token Authentication

This repository contains the CRUD REST service, built with ASP.NET Core and Entity Framework to illustrate creating REST API to performing CRUD actions and, how to create JWT token and secure API.

#### Prerequisites

- Visual Studio
- [ASP.NET Core](https://dotnet.microsoft.com/en-us/download)
- [SQL Server](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)

#### Usage

- create new webapi project `dotnet new webapi`
- install jwt package `dotnet add package Microsoft.AspNetCore.Authentication.JwtBearer`
- Checkout this project to a location in your disk.
- Open the solution file using the Visual Studio.
- Restore the NuGet packages by rebuilding the solution `dotnet restore`.
- Change the connection string in the appsettings.json file that points to your SQL Server
- Run the project `dotnet run`.
- View jwts users commands `dotnet user-jwts`
- Create test jwt token `dotnet user-jwts create`
- Test secret Path `curl -i -H "Authorization: Bearer {token}" https://localhost:{port}/secret`
- View Swagger docs `http://localhost:5273/swagger`

#### Doc

- https://learn.microsoft.com/en-us/nuget/consume-packages/install-use-packages-dotnet-cli

- https://learn.microsoft.com/en-us/aspnet/core/security/authentication/jwt-authn?view=aspnetcore-7.0&tabs=windows

- https://github.com/SyncfusionExamples/inventory-management-rest-service-asp-dotnet-core
