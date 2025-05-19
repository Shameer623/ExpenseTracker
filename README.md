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
 
## ⚙️ Project Structure
 
expense-tracker/ ├── backend/ │ ├── controller/ │ ├── model/ │ ├── repository/ │ ├── service/ │ ├── security/ │ ├── dto/ │ └── application.properties ├── frontend/ │ ├── src/ │ │ ├── components/ │ │ ├── pages/ │ │ ├── services/ │ │ └── App.js └── README.md
 
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
 
🧪 Sample Database Schema (MySQL)
 
CREATE TABLE users (
  id BIGINT AUTO_INCREMENT PRIMARY KEY,
  username VARCHAR(50) UNIQUE NOT NULL,
  password VARCHAR(255) NOT NULL
);
 
CREATE TABLE expenses (
  id BIGINT AUTO_INCREMENT PRIMARY KEY,
  user_id BIGINT NOT NULL,
  amount DECIMAL(10,2),
  category VARCHAR(100),
  description TEXT,
  date DATE,
  FOREIGN KEY (user_id) REFERENCES users(id)
);
 
 
---
 
📂 Postman Collection
 
A Postman collection with sample requests for all APIs is included in the /postman/ExpenseTracker.postman_collection.json file.
 
 
