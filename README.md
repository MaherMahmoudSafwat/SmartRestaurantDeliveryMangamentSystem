# 🍽️ Smart Restaurant Management System

A production-ready, scalable restaurant delivery management system built with Spring Boot 3.x and PostgreSQL.

[![Java](https://img.shields.io/badge/Java-17-007396)](https://adoptium.net/)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.2.0-6DB33F)](https://spring.io/projects/spring-boot)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16-336791)](https://www.postgresql.org/)
[![License](https://img.shields.io/badge/License-MIT-blue)](LICENSE)

## 📋 Features

### 🔐 Authentication & Authorization
- JWT-based authentication with role-based access control
- User registration, login, profile management
- Password reset functionality
- OAuth2 Google login (optional)

### 🍽️ Menu Management
- Category management with image upload
- Menu item CRUD with pricing, stock, and availability
- Item types: REGULAR, WEIGHT_BASED, SEASONAL
- Bulk import/export capabilities

### 🎯 Customization Engine
- Modifiers (Extra Cheese, No Onions, etc.)
- Group options with pricing models
- Multi-level customization hierarchy
- Real-time price calculation

### 🧾 Order Management
- Complete order lifecycle (PENDING → DELIVERED)
- Order item tracking with price snapshots
- Modifier selection at order time
- Order status tracking with audit trail
- Order cancellation with stock restoration

### 💳 Payment Processing
- Multiple payment methods (Cash, Card, Wallet)
- Secure payment processing
- Refund management
- Transaction history

### 🏷️ Discount Engine
- Multiple discount types (Percentage, Fixed, BOGO)
- Date-range activation
- Minimum order amount validation
- Loyalty points integration
- Discount status management (ACTIVE, EXPIRED, DISABLED)

### 📊 Reporting & Analytics
- Daily sales reports
- Revenue tracking
- Top-selling items analysis
- Customer feedback aggregation
- Order performance metrics

### ⭐ Customer Engagement
- Feedback & rating system
- Loyalty points accumulation
- Order history
- Real-time order tracking

## 🛠️ Tech Stack

| Component | Technology |
|-----------|------------|
| Language | Java 17 |
| Framework | Spring Boot 3.2.0 |
| Security | Spring Security + JWT |
| ORM | Spring Data JPA (Hibernate) |
| Database | PostgreSQL 16 |
| Migrations | Flyway |
| API Docs | SpringDoc OpenAPI 2.0 |
| Testing | JUnit 5, Mockito, Testcontainers |
| Build Tool | Maven / Gradle |
| Container | Docker / Docker Compose |
| CI/CD | GitHub Actions |

## 🚀 Quick Start

### Prerequisites
- JDK 17+
- Docker & Docker Compose
- PostgreSQL 16 (or use Docker)
- Maven 3.9+

### Local Development

```bash
# 1. Clone the repository
git clone https://github.com/your-org/smart-restaurant-management-system.git
cd smart-restaurant-management-system

# 2. Start PostgreSQL with Docker
docker-compose up -d postgres

# 3. Run database migrations
./mvnw flyway:migrate

# 4. Build and run the application
./mvnw spring-boot:run

# 5. Access the application
http://localhost:8080/api/v1
http://localhost:8080/swagger-ui.html
