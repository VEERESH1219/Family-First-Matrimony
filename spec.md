# ⚙️ Technical Specifications: Family-First Matrimony

This document outlines the technical architecture, database schema, and security protocols for the Family-First Matrimony application.

## 1. Technology Stack
We are using a **Backend-Heavy** approach to ensure security, scalability, and strict data validation.

| Layer | Technology | Description |
| :--- | :--- | :--- |
| **Runtime Environment** | **Node.js** | Non-blocking I/O for handling concurrent requests. |
| **Framework** | **Express.js** | Implements REST API with MVC Architecture. |
| **Database** | **MongoDB** | NoSQL database for flexible yet structured profile data. |
| **ORM/ODM** | **Mongoose** | Strictly enforces Schema validation (Age, Enums). |
| **Authentication** | **JWT (JSON Web Token)** | Stateless authentication for secure sessions. |
| **Task Scheduling** | **Node-Cron** | Executes the "Auto-Termination" logic nightly. |
| **File Storage** | **AWS S3 / Cloudinary** | Secure storage for ID proofs and profile photos. |

---

## 2. Project Architecture (MVC Pattern)
The project follows a clean **Model-View-Controller** separation.

```text
matrimony-backend/
│
├── config/             # Database connection & Environment variables
├── controllers/        # Business logic (handle requests, send responses)
├── models/             # Database Schemas (Data strictness lives here)
├── routes/             # API Endpoints definition
├── middlewares/        # Security checks (Auth, Verification, Admin)
├── utils/              # Helper functions (Cron Jobs, Email Services)
├── validations/        # Joi/Zod validation schemas
└── server.js           # Application entry point
