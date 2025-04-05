# SIT323 Task 5.1P – Dockerized Calculator Microservice

This project is a simple calculator microservice built with **Node.js** and **Express**, then containerized using **Docker** and **Docker Compose** as part of SIT323/SIT737 Cloud Native Application Development (Task 5.1P).

---

## 📦 Features

- Supports common arithmetic operations via API:
  - `add`, `subtract`, `multiply`, `divide`
  - `power`, `sqrt`, `mod`
- Provides a general `/calculate` endpoint and dedicated endpoints for each operation.
- Includes logging via Winston for both success and error logs.

---

## 🛠️ Technologies Used

- Node.js
- Express.js
- Winston (logging)
- Docker
- Docker Compose

---

## 🚀 Setup Instructions

### 1. Clone the Repository
### 2. Build and Run with Docker Compose


```
git clone https://github.com/SatyamRaina/sit323-2025-prac5p.git
cd sit323-2025-prac5p

docker-compose up --build
```



The application will start and be accessible at:
➡️ http://localhost:3051

🧪 Example API Usage

1. General Endpoint:
curl "http://localhost:3051/calculate?n1=10&n2=5&operation=add"
2. Dedicated Endpoints:
curl "http://localhost:3051/add?n1=20&n2=15"
curl "http://localhost:3051/subtract?n1=50&n2=30"
curl "http://localhost:3051/sqrt?n1=81"


