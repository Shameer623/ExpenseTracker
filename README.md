# Expense Tracker - Full Stack Web Application
 
A modern full-stack **Expense Tracker** web application that helps users manage their finances by tracking daily expenses with category-wise filtering, real-time updates, and an intuitive interface.
 
Built with **Spring Boot (Java)** and **React**, this project follows best practices in RESTful API design, component-based UI development, and clean architecture.
 
---
 
## 🚀 Key Features
 
- **User Authentication** using username (Spring Security)
- **Add / Edit / Delete** expenses with amount, category, and date
- **Monthly and category-wise summaries**
- **Responsive UI** for mobile and desktop
- **Secure REST APIs** with proper request validations
- **Modular architecture** for scalability and maintainability
 
---
 
## 🛠️ Tech Stack
 
| Layer     | Technologies                                      |
|-----------|--------------------------------------------------|
| Frontend  | React, Axios, React Router, Bootstrap/Tailwind   |
| Backend   | Spring Boot, Spring Security, JPA (Hibernate)    |
| Database  | MySQL (production) / H2 (development & testing)  |
| Build     | Maven (Backend), npm (Frontend)                  |
 
---
 

 
## 🔐 Authentication
 
- Login with **username + password**
- Spring Security JWT-based token generation
- Protected endpoints for authenticated users only
 
---
 
## 📡 REST API Endpoints (Sample)
 
| Method | Endpoint              | Description           |
|--------|-----------------------|-----------------------|
| POST   | `/api/auth/login`     | User login            |
| POST   | `/api/expenses`       | Add new expense       |
| GET    | `/api/expenses`       | Get all expenses      |
| GET    | `/api/expenses/{id}`  | Get expense by ID     |
| PUT    | `/api/expenses/{id}`  | Update expense        |
| DELETE | `/api/expenses/{id}`  | Delete expense        |
 
---
 
## ✅ How to Run the Project
 
### 1. Clone the Repository
 
```bash
git clone https://github.com/Shameer623/expense-tracker.git
cd expense-tracker
 
2. Backend Setup (Spring Boot)
 
cd backend
# Update DB credentials in application.properties
mvn clean install
mvn spring-boot:run
 
3. Frontend Setup (React)
 
cd frontend
npm install
npm start
 
Access the app at: http://localhost:3000
 
 
 
---
 
📊 Future Enhancements
 
Income and savings tracking
 
Export to CSV / PDF
 
Pie charts and bar graphs for analytics
 
Dark mode support
 
Mobile App (React Native)
 
 
 
---
 

