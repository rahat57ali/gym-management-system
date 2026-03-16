# Gym Management System

A full-stack gym management system with React frontend and Spring Boot backend.

---

## Project Structure
gym-management-system/
├── frontend/ # React app
├── backend/ # Spring Boot app (Maven)
└── README.md # This file


---

## Prerequisites

- **Node.js** (v18+)
- **npm** (v9+)
- **Java** (17+)
- **Maven** (v3.8+)
- **MySQL** (v8+)

---

## 1. Setup MySQL Database

1. Create a database named `gym_management`.
2. Run the provided SQL schema (see Deliverable 1) to create tables and seed data.
mysql -u <username> -p gym_management < backend/schema.sql


---

## 2. Run Backend (Spring Boot)

1. Navigate to the backend folder:
cd backend

2. Edit `src/main/resources/application.properties`:

- Set your MySQL username/password.
- Set a JWT secret (any random string).
spring.datasource.username=YOUR_DB_USERNAME
spring.datasource.password=YOUR_DB_PASSWORD
jwt.secret=YOUR_JWT_SECRET_KEY


3. Build and start the backend:
mvn clean install
mvn spring-boot:run

- Backend runs at: [http://localhost:8080](http://localhost:8080)

---

## 3. Run Frontend (React)

1. Navigate to the frontend folder:
cd ../frontend

2. Install dependencies:
npm install

3. Start the frontend:
npm start

- Frontend runs at: [http://localhost:3000](http://localhost:3000)

---

## 4. Login Credentials

- **Admin:**  
  Email: `admin@gym.com`  
  Password: `adminhashedpassword` (replace with actual hash or set a new password in DB)

- **Member:**  
  Email: `bob@gym.com`  
  Password: `memberhashedpassword` (replace with actual hash or set a new password in DB)

---

## 5. Features

- **Admin:** Manage members, plans, payments, trainers, classes.
- **Member:** View profile, plan, trainer, enroll in classes.

---

## 6. API Endpoints

See backend source for full REST API.

---

## 7. Styling

- Tailwind CSS for modern, responsive UI.

---

## 8. Troubleshooting

- Ensure MySQL is running and accessible.
- Check backend logs for errors.
- JWT secret must match in backend config.

---

## 9. License

MIT

---

**Setup complete!**