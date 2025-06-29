# alx-airbnb-project-documentation

# Airbnb Clone – Backend Requirements Specification

This document outlines the technical and functional requirements for three core backend features:
1. User Authentication
2. Property Management
3. Booking System

---

## 1. User Authentication

### 🔐 Feature Summary
Allow users (hosts or guests) to register, log in, and manage sessions securely.

### 📌 Endpoints
- `POST /api/auth/register`
- `POST /api/auth/login`
- `GET /api/user/profile`
- `PATCH /api/user/profile`

### 📥 Input Specifications
#### `/register`
```json
{
  "email": "user@example.com",
  "password": "strongpassword",
  "role": "guest" | "host"
}
