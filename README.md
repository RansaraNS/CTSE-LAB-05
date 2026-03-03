# SE4010 – Microservices Lab  
### Docker • API Gateway • MongoDB Atlas

This project demonstrates a **microservices-based architecture** using **Docker Compose**, an **API Gateway**, and **MongoDB Atlas** for data persistence.  
Each microservice is containerized and all client requests are routed through a **single API Gateway**.

---

## 📌 Project Overview

The system consists of **three independent microservices** and **one API Gateway**:

- **Item Service** – Manages items
- **Order Service** – Handles customer orders
- **Payment Service** – Processes payments
- **API Gateway** – Central access point for all services

> ⚠️ Microservices do **not communicate directly** with each other.  
> All communication is handled via the **API Gateway**.

---

## 🧩 Architecture & Ports

| Component        | Description                          | Port |
|------------------|--------------------------------------|------|
| Item Service     | Item management operations           | 8081 |
| Order Service    | Order creation & retrieval           | 8082 |
| Payment Service  | Payment processing                   | 8083 |
| API Gateway      | Routes requests to services          | 8080 |

---

## 🗄️ Database Configuration

- **Database Type:** MongoDB Atlas (Cloud)
- **Database Name:** `Lab05`

### Example MongoDB Connection String
```env
mongodb+srv://<username>:<password>@myatlasclusteredu.dubkafb.mongodb.net/
