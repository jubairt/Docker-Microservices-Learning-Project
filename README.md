# 🚀 FastAPI Microservices – Simple Learning Project

This repository is a **beginner-friendly microservices setup** built using **FastAPI**, **Docker**, and **Docker Compose**.  
It is created only for **learning purposes** — to understand how multiple services run independently, communicate with each other, and work together inside Docker.

---

## 📦 What This Project Includes

### **🔹 User Service (Port 5001)**
Handles simple user-related operations.

### **🔹 Product Service (Port 5002)**
Manages product information and responses.

### **🔹 Order Service (Port 5003)**
Interacts with user-service and product-service to simulate order creation.

Each service:
- Has its own FastAPI application  
- Runs inside its own container  
- Exposes a unique port  
- Communicates through Docker service names  

---

## 🔗 Service Communication

Inside Docker Compose, services can talk to each other using:

- **User Service**  
  ↳ `http://user-service:5001`

- **Product Service**  
  ↳ `http://product-service:5002`

- **Order Service**  
  ↳ `http://order-service:5003`

### ▶️ How to Run the Project

Follow these steps to start all microservices using Docker Compose:

1. Make sure **Docker** and **Docker Compose** are installed on your system.

2. Open your terminal or PowerShell and navigate to the **root folder** of the project  
   (the directory where `docker-compose.yaml` is located).

3. Run the following command to build and start all services:
   ```bash
   docker-compose up --build

### 🔗 Accessing the Services

Once the containers are running, you can access each service at:

- **User Service:**  
  👉 http://localhost:5001

- **Product Service:**  
  👉 http://localhost:5002

- **Order Service:**  
  👉 http://localhost:5003

### ✅ Conclusion

This project is a simple learning setup showing how multiple FastAPI services run independently and communicate using Docker Compose.  
It provides a clear foundation for understanding microservices and can be easily extended as your learning grows.
