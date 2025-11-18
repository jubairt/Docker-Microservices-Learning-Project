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
