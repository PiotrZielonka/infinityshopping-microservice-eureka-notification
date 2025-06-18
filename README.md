# InfinityShopping Eureka Microservice – Notification 

This is the **Notification** eureka microservice from the **microservices-based concept** of the [InfinityShopping](https://github.com/PiotrZielonka/infinityshopping) e-commerce shop generator, originally implemented as a **monolithic JHipster application**.

The purpose of this repository is to **learn and demonstrate microservices architecture** using **JHipster**, **Spring Boot**, and **Eureka**, while offering a solid base for scaling the monolith into a full microservices solution.

If you want to run the entire application, you must run all microservices described in the main README here:  
👉 [InfinityShopping Microservices Eureka Product Concept](https://github.com/PiotrZielonka/infinityshopping-microservices-eureka-product-concept)

---

## 🧪 Running the Application Locally

### Prerequisites

| Tool       | Version           |
| ---------- | ----------------- |
| Docker     | 28.0.4 (Desktop)  |
| Java       | OpenJDK 17        |
| Maven      | 3.8.1             |
| Node.js    | 22.15.1 (x64)     |
| PostgreSQL | Installed locally |

* This project has been tested with Docker Desktop version 28.0.4, but it should work with any newer release.
* Node.js 22.15.1 (x64) is verified to work, but other versions may also be compatible.
* PostgreSQL must be installed locally for database setup and connection.

### Database Setup Instructions

> By default, JHipster configures PostgreSQL in Docker, but **this version connects to a locally installed PostgreSQL instance**.

To make sure you are running with the correct setup:

1. Start Docker (required for some JHipster containers).
2. **Delete any PostgreSQL Docker containers** after startup.

    * This avoids conflict since **local DB connection is used** (not Docker).
3. Make sure the local DB configuration matches these commits or manually configure the connection:

    * [Gateway DB Config](https://github.com/PiotrZielonka/infinityshopping-eureka-gateway/commit/bf30ce3824937c221e938ee39328437feeded7e7)
    * [Notification DB Config](https://github.com/PiotrZielonka/infinityshopping-microservice-eureka-notification/commit/3dd595672cc547f5b26cce4060eaa4c719684582)

### Launch only this microservice

1. Start the Gateway  [Gateway Repository](https://github.com/PiotrZielonka/infinityshopping-eureka-gateway)   
2. Start the Notification Microservice on `localhost:8082`  
3. In each project directory (gateway and notification), run the following command:

   ```bash
   ./mvnw
````
> 🧭 This microservice runs on **localhost:8082**
````
> ⚠️ This setup runs only the **Notification** microservice. The **Store** microservice will not be available.
> For a full setup, see:
> 👉 [InfinityShopping Microservices Eureka Product Concept](https://github.com/PiotrZielonka/infinityshopping-microservices-eureka-product-concept)

---

## 📫 Questions?

If you have questions or want to connect:

* Check out the monolith version: [InfinityShopping Monolith](https://github.com/PiotrZielonka/infinityshopping) 
* Open an issue on this repository

---

## 🔭 Project Scope

This is a **learning playground** but also a **powerful concept prototype** for real-world microservice systems.

---