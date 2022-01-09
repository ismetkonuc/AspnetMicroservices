Overall picture of implementations on microservices with .NET tools on real-world e-commerce microservices project:

![Uygulama Ekran Görüntüsü](https://i.imgur.com/LOkOvxA.png)

  There is a couple of microservices which implemented e-commerce modules over Catalog, Basket, Discount and Ordering microservices with NoSQL (MongoDB, Redis) and Relational databases (PostgreSQL, Sql Server) with communicating over RabbitMQ Event Driven Communication and using Ocelot API Gateway.

  ## Whats Including In This Repository

This project is under development. It currently includes the following features:

Catalog microservice which includes;

 - ASP.NET Core Web API application
 - REST API principles, CRUD operations
 - MongoDB database connection and containerization
 - Repository Pattern Implementation
 - Swagger Open API implementation


## Run The Project

You will need the following tools:

 - Visual Studio 2019
 - .NET (Core) 5 or later
 - Docker Desktop

### Installing

Follow these steps to get your development environment set up: (Before Run Start the Docker Desktop)

- Clone the repository
- Once Docker for Windows is installed, go to the Settings > Advanced option, from the Docker icon in the system tray, to configure the minimum amount of memory and CPU like so:
    - Memory: 4 GB
    - CPU: 2
- At the root directory which include docker-compose.yml files, run below command:

```bash
  docker-compose -f docker-compose.yml -f docker-compose.override.yml up -d
```

- You can launch microservices as below urls:
    - Catalog API -> http://host.docker.internal:8000/swagger/index.html

  