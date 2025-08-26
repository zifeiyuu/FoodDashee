# FoodDashee - Online Food Delivery Platform

**FoodDashee** is a food delivery application built with **Spring Boot + Maven**, providing complete workflows for customers, merchants, and delivery drivers.  
The system supports browsing restaurants, placing orders, managing menus, and real-time order tracking.

---

## Features

### Customer App
- User registration & login
- Browse restaurants and menus
- Add items to cart and place orders
- Online payment

### Merchant App
- Manage restaurant profile and menus
- Handle orders (accept / reject / in progress)
- Sales & order reports

### Delivery App
- Accept / grab delivery orders
- Update delivery status in real-time
- Confirm completed deliveries

### Admin Dashboard
- Manage users
- Manage categories and menu items
- Order management
- System configuration

---

## Tech Stack

- **Backend**: Spring Boot, Spring MVC, MyBatis, Maven  
- **Database**: MySQL, Redis  
- **Authentication**: JWT  
- **Frontend**:  
  - Customer & Merchant apps: Vue.js (can extend to React/Flutter)  
  - Admin dashboard: Vue.js + Element UI  
- **Tools**: Git, Maven, Docker (optional)  

---

## Project Structure

```
sky-take-out/
├── pom.xml             # Maven configuration
├── sky-common          # Common utilities and global exception handling
├── sky-pojo            # POJO entities
├── sky-server          # Main backend service (Spring Boot)
```

---

## Getting Started

### 1. Clone Repository
```bash
git clone https://github.com/zifeiyuu/FoodDashee.git
cd FoodDashee
```

### 2. Configure Database
1. Create MySQL database:
   ```sql
   CREATE DATABASE fooddashee DEFAULT CHARACTER SET utf8mb4 COLLATE utf8mb4_general_ci;
   ```
2. Update `application.yml` with your DB connection info.

### 3. Run Backend Service
```bash
mvn clean package
cd sky-server
mvn spring-boot:run
```

### 4. Run Frontend (if available)
```bash
cd frontend
npm install
npm run serve
```

### 5. Access
- Customer App: http://localhost:8080  
- Admin Dashboard: http://localhost:8080/admin  
---

## License
MIT License © 2025 [zifeiyuu](https://github.com/zifeiyuu)
