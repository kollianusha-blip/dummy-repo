# Order Processing Service

> A robust microservice responsible for handling customer orders, validating inventory, and coordinating payment processing events in the EliteA ecosystem.

---

## 1. Executive Summary
- **Application Name:** order-processing-service
- **Service Owner:** Anusha Kolli <kolli_anusha@epam.com>
- **Business Impact:** Critical
- **Description:** A high-performance Node.js microservice that ingests customer order requests, validates inventory levels against the database, and publishes event messages to RabbitMQ for asynchronous payment processing.

---

## 2. System Architecture & Tech Stack
| Component | Specification |
| :--- | :--- |
| Language/Runtime | Node.js (v18.x LTS) |
| Frameworks | Express.js (v4.18.2), Sequelize ORM (v6) |
| Primary Database | PostgreSQL |
| Cloud Provider | AWS |
| Infrastructure | Docker, Kubernetes (EKS) |

---

## 3. Integration & Dependencies
- **Upstream Dependencies:** Inventory Service, Authentication Gateway
- **Downstream Consumers:** Notification Service, Analytics Data Pipeline
- **External APIs:** Stripe API (Payment Processing), Twilio (SMS Notifications)

---

## 4. Technical Configuration
- **Main Branch:** `main`
- **Build Tool:** NPM
- **Critical Env Variables:** `PORT`, `DATABASE_URL`, `RABBITMQ_URL`, `STRIPE_API_KEY`
- **Deployment Pipeline:** GitHub Actions

---

## 5. Quality & Compliance
- **Test Frameworks:** Jest, Supertest
- **Code Coverage Goal:** 85%
- **Security Scanning:** Snyk, SonarQube
- **Observation/Logging:** Datadog, Winston

---

## 6. Documentation & Resources
**Maintainers:** Anusha Kolli <kolli_anusha@epam.com> 
- **GitHub Repository:** [https://github.com/elitea-org/order-processing-service](https://github.com/elitea-org/order-processing-service)
- **API Documentation:** [Confluence Swagger Docs Link](#)
- **JIRA Board:** [JIRA CHECKOUT BOARD](#)
- **On-Call Rotation:** [PagerDuty Checkout On-Call](#)

---

## 7. Deployment Status
> **Current Version:** v1.4.2  
> **Last Updated:** 2026-09-22 (via EliteA Automated Sync)
