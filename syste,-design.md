# 📐 System Design Interview Notes

---

## 1️⃣ What is Microservices?

**Microservices architecture** is a design approach where an application is built as a collection of small, independent services.

Each service:
- Focuses on a single business capability
- Runs independently
- Communicates via APIs (HTTP/REST, gRPC, messaging)

### 🔹 Key Characteristics
- Independent deployment
- Decentralized data management
- Scalable individually
- Fault isolation

### 🔹 Example
Instead of one monolithic app:
- User Service
- Payment Service
- Order Service
- Notification Service

Each runs separately and communicates via APIs.

---

## 2️⃣ Patterns to Consider While Designing Microservices

### 🔹 1. API Gateway Pattern
- Single entry point for clients
- Handles authentication, routing, rate limiting

### 🔹 2. Service Discovery Pattern
- Services dynamically discover each other

### 🔹 3. Circuit Breaker Pattern
- Prevents cascading failures

### 🔹 4. Database per Service
- Each microservice owns its database

### 🔹 5. Event-Driven Architecture
- Services communicate using events (Kafka, RabbitMQ)

### 🔹 6. Saga Pattern
- Manages distributed transactions

---

## 3️⃣ What is CDN?

A **Content Delivery Network (CDN)** is a globally distributed network of servers that delivers static content faster.

### 🔹 Benefits
- Faster loading (low latency)
- Reduced server load
- Improved availability
- Better security (DDoS protection)

### 🔹 Examples
- :contentReference[oaicite:0]{index=0}  
- :contentReference[oaicite:1]{index=1}  
- :contentReference[oaicite:2]{index=2} (CloudFront)

---

## 4️⃣ How SSL Certificate Works in ACM?

:contentReference[oaicite:3]{index=3} (ACM) is a service by :contentReference[oaicite:4]{index=4} to provision and manage SSL/TLS certificates.

### 🔹 How It Works:
1. Request certificate in ACM
2. Validate domain (DNS or Email validation)
3. Attach certificate to:
   - Load Balancer
   - CloudFront distribution
4. ACM automatically renews it

### 🔹 Benefits
- Free SSL
- Auto-renewal
- Easy integration with AWS services

---
