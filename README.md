# Login & Signup Demo (Spring Boot + MySQL)

A simple **Login and Signup web application** built using **Spring Boot**, **Spring Data JPA**, and **MySQL** with a lightweight **HTML/CSS frontend**.  
This mini project demonstrates how to create and manage user authentication endpoints for signup and login functionality.

---

## 🚀 Features

- User registration (Signup)
- Secure login with authentication
- REST API for handling user data
- Database persistence using MySQL
- Lightweight and responsive frontend (HTML + CSS)
- Organized backend using Spring Boot and JPA

---

## 🛠️ Tech Stack

### **Backend**
- **Java 17**
- **Spring Boot 3.2.4**
- **Spring Web**
- **Spring Data JPA**
- **Spring Security**
- **MySQL Database**
- **Lombok** (for cleaner code)

### **Frontend**
- **HTML5**
- **CSS3**
- **Vanilla JavaScript (Fetch API)**

---

## 🧩 Project Structure

LoginSignupDemo/
├── src/main/java/com/example/
│ ├── LoginSignupDemoApplication.java # Main entry point
│ ├── model/User.java # Entity class
│ ├── controller/UserController.java # REST Controller
│ ├── repository/UserRepository.java # JPA Repository
├── src/main/resources/
│ ├── application.properties # Database config
│ ├── static/
│ │ ├── login.html # Login Page
│ │ ├── signup.html # Signup Page
│ │ ├── styles.css # Styling
│ └── templates/ # (optional)
├── pom.xml # Maven dependencies

yaml
Copy code

---

## ⚙️ Setup Instructions

### **1. Clone the repository**
```bash
git clone https://github.com/<your-username>/login-signup-demo.git
cd login-signup-demo
2. Configure MySQL Database
Create a new database named my_app_db

Update application.properties with your MySQL credentials:

properties
Copy code
spring.datasource.url=jdbc:mysql://localhost:3306/my_app_db
spring.datasource.username=root
spring.datasource.password=yourpassword
3. Run the Application
bash
Copy code
mvn spring-boot:run
The app runs on http://localhost:8080

4. Access Frontend
Open:

Login page: http://localhost:8080/login.html

Signup page: http://localhost:8080/signup.html

📬 API Endpoints
Method	Endpoint	Description
POST	/api/auth/signup	Register a new user
POST	/api/auth/login	Authenticate user

🧠 Future Enhancements
Add JWT-based authentication

Encrypt passwords using BCrypt

Add role-based access (Admin/User)

Build a dashboard after login
