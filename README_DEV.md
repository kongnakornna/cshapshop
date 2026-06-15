# ASP.NET Core C# — Clean Architecture, CQRS, Event Sourcing

[![Build](https://github.com/jeangatto/ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing/actions/workflows/dotnet.yml/badge.svg)](https://github.com/jeangatto/ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing/actions/workflows/dotnet.yml)
[![SonarCloud](https://github.com/JeanGatto/ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing/actions/workflows/sonar-cloud.yml/badge.svg)](https://github.com/JeanGatto/ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing/actions/workflows/sonar-cloud.yml)
[![CodeQL](https://github.com/jeangatto/ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/jeangatto/ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing/actions/workflows/codeql-analysis.yml)
[![DevSkim](https://github.com/jeangatto/ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing/actions/workflows/devskim-analysis.yml/badge.svg)](https://github.com/jeangatto/ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing/actions/workflows/devskim-analysis.yml)
[![License](https://img.shields.io/github/license/jeangatto/ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing.svg)](LICENSE)

[![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing&metric=ncloc)](https://sonarcloud.io/summary/new_code?id=ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing)
[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing&metric=coverage)](https://sonarcloud.io/dashboard?id=ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing)
[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing)
[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing)
[![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing&metric=vulnerabilities)](https://sonarcloud.io/dashboard?id=ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing)
[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing&metric=bugs)](https://sonarcloud.io/dashboard?id=ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing)
[![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing&metric=code_smells)](https://sonarcloud.io/dashboard?id=ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing)

## Star History

<a href="https://www.star-history.com/?repos=jeangatto%2FASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing&type=date&legend=bottom-right">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/chart?repos=jeangatto/ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing&type=date&theme=dark&legend=top-left" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/chart?repos=jeangatto/ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing&type=date&legend=top-left" />
   <img alt="Star History Chart" src="https://api.star-history.com/chart?repos=jeangatto/ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing&type=date&legend=top-left" />
 </picture>
</a>

About the repository:
Open source project written in the latest version of ASP.NET Core, implementing the concepts of S.O.L.I.D, Clean Code,
CQRS (Command Query Responsibility Segregation)

## Give it a star! ⭐

If you liked this project, learned something, give it a star. Thank you!

## **Technologies**

- ASP.NET Core 10
- Entity Framework Core 10
- **EF Compiled Queries** (https://learn.microsoft.com/en-us/dotnet/framework/data/adonet/ef/language-reference/compiled-queries-linq-to-entities)
- Unit & Integration Tests + xUnit + FluentAssertions
- xUnit (https://github.com/xunit/xunit)
- FluentAssertions (https://github.com/fluentassertions/fluentassertions)
- Polly (https://github.com/App-vNext/Polly)
- AutoMapper (https://github.com/LuckyPennySoftware/AutoMapper)
- FluentValidator (https://github.com/FluentValidation/FluentValidation)
- MediatR (https://github.com/LuckyPennySoftware/MediatR)
- Result (https://github.com/ardalis/Result)
- ~~Swagger UI~~
- OpenApi
- **Scalar** - Interactive API Reference from OpenAPI/Swagger (https://github.com/scalar/scalar)
- HealthChecks
- Microsoft SQL Server
- MongoDB
- Redis (Cache)
- Docker & Docker Compose
- Distroless .NET Images (https://github.com/dotnet/dotnet-docker/blob/main/documentation/distroless.md)

## **Architecture**

![CQRS Pattern](img/cqrs-pattern.png "CQRS Pattern")

- Full architecture with responsibility separation concerns, SOLID and Clean Code
- Domain Driven Design (Layers and Domain Model Pattern)
- Domain Events
- Domain Notification
- Domain Validations
- CQRS
- Event Sourcing
- Unit of Work
- Repository Pattern
- Result Pattern

## Running the application

After cloning the repository to the desired folder, run the command in the terminal at the root of the project:

```csharp
dotnet clean Shop.slnx --nologo /tl && dotnet build Shop.slnx --nologo /tl
```

Set passwords in the `.env` file:

```yaml
MSSQL_SA_PASSWORD=YOUR_STRONG_!Passw0rd
REDIS_PASSWORD=YOUR_STRONG_!Passw0rd
MSSQL_PORT=1433
MONGO_PORT=27017
REDIS_PORT=6379
ASPNETCORE_ENVIRONMENT=Development
```

Next step, run the command in the terminal:

```csharp
docker-compose up --build
```

Now just open the url in the browser:

```csharp
http://localhost:{port}/scalar/v1
```

## MiniProfiler for .NET

To access the page with the performance indicators and performance:

```csharp
http://localhost:{port}/profiler/results-index
```

## License

- [MIT License](https://github.com/jeangatto/ASP.NET-Core-Clean-Architecture-CQRS-Event-Sourcing/blob/main/LICENSE)


# API
New-NetFirewallRule -DisplayName "Docker API" -Direction Inbound -Protocol TCP -LocalPort 5005 -Action Allow

# SQL Server (host port 1435)
New-NetFirewallRule -DisplayName "Docker SQL" -Direction Inbound -Protocol TCP -LocalPort 1435 -Action Allow

# MongoDB (host port 27016)
New-NetFirewallRule -DisplayName "Docker Mongo" -Direction Inbound -Protocol TCP -LocalPort 27016 -Action Allow

# Redis (host port 6377)
New-NetFirewallRule -DisplayName "Docker Redis" -Direction Inbound -Protocol TCP -LocalPort 6377 -Action Allow


Here's the **full, corrected configuration** that allows any IP access and fixes all port/connection string issues.

---

## 📁 `docker-compose.yml` (complete)

```yaml
services:
  # Microsoft SQL Server
  shop-sql-server:
    image: mcr.microsoft.com/mssql/server:2022-latest
    restart: unless-stopped
    environment:
      ACCEPT_EULA: "Y"
      MSSQL_SA_PASSWORD: ${MSSQL_SA_PASSWORD}
      MSSQL_PID: Express
      MSSQL_COLLATION: SQL_Latin1_General_CP1_CI_AS
    ports:
      - "${MSSQL_HOST_PORT}:1433"          # host:container (internal fixed 1433)
    volumes:
      - sql_data:/var/opt/mssql
    networks:
      - shop-network
    logging:
      driver: "json-file"
      options:
        max-size: "10m"
        max-file: "3"

  # MongoDB
  shop-mongo-server:
    image: mongo:latest
    restart: unless-stopped
    ports:
      - "${MONGO_HOST_PORT}:27017"         # host:container (internal fixed 27017)
    volumes:
      - mongo_data:/data/db
    networks:
      - shop-network
    logging:
      driver: "json-file"
      options:
        max-size: "10m"
        max-file: "3"

  # Redis Cache
  shop-redis-server:
    image: redis:latest
    restart: unless-stopped
    command: redis-server --requirepass ${REDIS_PASSWORD}
    ports:
      - "${REDIS_HOST_PORT}:6379"          # host:container (internal fixed 6379)
    volumes:
      - redis_data:/data
    networks:
      - shop-network
    logging:
      driver: "json-file"
      options:
        max-size: "10m"
        max-file: "3"

  # Shop API Container (NET Core)
  shop-api:
    build:
      context: .
      dockerfile: src/Shop.PublicApi/Dockerfile
    image: shop-api:latest
    restart: on-failure
    env_file:
      - ./.env
    environment:
      ASPNETCORE_ENVIRONMENT: ${ASPNETCORE_ENVIRONMENT}
      # Internal connections (inside Docker network) use service names + internal ports
      ConnectionStrings__SqlConnection: "Server=shop-sql-server,1433;Database=ShopContext;User Id=sa;Password=${MSSQL_SA_PASSWORD};TrustServerCertificate=True;"
      ConnectionStrings__NoSqlConnection: "mongodb://shop-mongo-server:27017"
      ConnectionStrings__CacheConnection: "shop-redis-server:6379,password=${REDIS_PASSWORD},abortConnect=false"
    ports:
      - "5005:80"                          # API exposed on host port 5005
    depends_on:
      - shop-sql-server
      - shop-mongo-server
      - shop-redis-server
    networks:
      - shop-network
    logging:
      driver: "json-file"
      options:
        max-size: "10m"
        max-file: "3"

volumes:
  sql_data:
  redis_data:
  mongo_data:

networks:
  shop-network:
    driver: bridge
```

---

## 📄 `.env` file (complete)

```env
# SQL Server
MSSQL_SA_PASSWORD=root
MSSQL_HOST_PORT=1435        # external port for SQL Server (any free port)

# Redis
REDIS_PASSWORD=root
REDIS_HOST_PORT=6377        # external port for Redis

# MongoDB
MONGO_HOST_PORT=27016       # external port for MongoDB

# API
ASPNETCORE_ENVIRONMENT=Development
```

> **Note**: The API itself is exposed on host port `5005` (fixed in compose file). You can change that by editing the `ports:` section of `shop-api`.

---

## 🔥 Windows Firewall – allow external IP access

Run **PowerShell as Administrator**:

```powershell
# API (port 5005)
New-NetFirewallRule -DisplayName "Docker API 5005" -Direction Inbound -Protocol TCP -LocalPort 5005 -Action Allow

# SQL Server (host port 1435)
New-NetFirewallRule -DisplayName "Docker SQL 1435" -Direction Inbound -Protocol TCP -LocalPort 1435 -Action Allow

# MongoDB (host port 27016)
New-NetFirewallRule -DisplayName "Docker Mongo 27016" -Direction Inbound -Protocol TCP -LocalPort 27016 -Action Allow

# Redis (host port 6377)
New-NetFirewallRule -DisplayName "Docker Redis 6377" -Direction Inbound -Protocol TCP -LocalPort 6377 -Action Allow
```

> If your Windows network profile is **Public**, change it to **Private** (Settings → Network & Internet → Ethernet/Wi-Fi → click your network → set to Private).

---

## 🚀 Deploy and test

```bash
# Stop old containers and remove volumes (if you want a clean slate)
docker compose down -v

# Build and start
docker compose up -d --build

# Check all containers are running
docker compose ps
```

### Test from another device on the same network

Replace `192.168.1.41` with your Windows host's actual IP (`ipconfig` → IPv4 address).

- **API**:  
  `curl http://192.168.1.41:5005/health` (or any endpoint)

- **Redis** (requires `redis-cli`):  
  `redis-cli -h 192.168.1.41 -p 6377 -a root ping`  
  Expected: `PONG`

- **SQL Server** (using `sqlcmd` or SSMS):  
  Server: `192.168.1.41,1435`  
  Login: `sa`  
  Password: `root`

- **MongoDB** (using `mongosh`):  
  `mongosh "mongodb://192.168.1.41:27016"`

---

## ✅ What "full" means now

You have:
- **Full external IP access** (any device on your LAN can connect).
- **Correct internal port mappings** (containers listen on their default ports, host uses your chosen external ports).
- **Proper connection strings** inside the API container.
- **Firewall rules** to let traffic through.

If you still have issues, verify:
- No VPN blocking local traffic.
- Windows Defender Firewall is **not** blocking Docker processes (allow `vpnkit.exe` or `com.docker.backend` if needed).

Now your shop services are fully accessible from anywhere on your network.