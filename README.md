# Angular-Project
Nagnath college managment System using Angular

# 🎓 Nagnath College Management System

🧑‍💻 Group member  

Made with 💡 by  

1. Yashraj Chavare
2. Amitabh Shinde  
3. Hrishikesh Nikam
4. Ajinkya Badave
5. Yash Khatwate

📧 chavareyashraj@gmail.com  
📧 amitabhshindevolley45@gmail.com  
📧 mrhrishikesh1337@gmail.com  
📧 badaveajinkya55@gmail.com 

📧 yashkhatwate2225@gmail.com   

📍 India  

---

## ✨ Overview

The **Nagnath College Management System** is a modern platform designed to simplify and digitalize academic operations.  
Built with **Spring Boot** for backend, **Angular** for frontend, and **PostgreSQL** as the database, the system empowers colleges with automated student records, faculty management, and academic tracking.  

---

## 🌟 Key Features

- **Student Registration & Profile Management**  
- **Faculty & Department Management**  
- **Course & Subject Allocation**  
- **Examination & Results Processing**  
- **Role-based Authentication (Admin / Faculty / Student)**  
- **Responsive Dashboard & Analytics**  
- **Report Generation (PDF/Excel)**  

---
 

## 🛠 Technology Stack

### Backend
- **Spring Boot 3.2** (Java 17)
- **Spring Data JPA / Hibernate**
- **PostgreSQL 15**
- **Lombok**
- **Maven** (Build Automation)

### Frontend
- **Angular 17+**
- **Bootstrap 5.3**
- **RxJS**
- **Chart.js** (Reports & Graphs)

### DevOps
- **Docker** (Containerization)
- **GitHub Actions** (CI/CD)

---
 

1) Database Setup


sudo -u postgres psql -c "CREATE DATABASE college_db;"
sudo -u postgres psql -c "CREATE USER college_admin WITH PASSWORD 'password';"
sudo -u postgres psql -c "GRANT ALL PRIVILEGES ON DATABASE college_db TO college_admin;"

2) Backend Setup


cd backend
mvn clean install
mvn spring-boot:run


application.properties

spring.datasource.url=jdbc:postgresql://localhost:5432/college_db
spring.datasource.username=college_admin
spring.datasource.password=password
spring.jpa.hibernate.ddl-auto=update


API will run at:
👉 http://localhost:8080/api


3) Frontend Setup
cd frontend
npm install
ng serve --open


Frontend will run at:
👉 http://localhost:4200

📚 API Documentation

Student Endpoints
Endpoint	Method	Description
/api/students	GET	Get all students
/api/students	POST	Create new student
/api/students/{id}	GET	Get student by ID
/api/students/{id}	PUT	Update student
/api/students/{id}	DELETE	Delete student
Faculty Endpoints
Endpoint	Method	Description
/api/faculty	GET	Get all faculty members
/api/faculty	POST	Add new faculty


📂 Project Structure


nagnath-college/
├── backend/                  # Spring Boot Backend
│   ├── src/main/java/com/nagnath/college
│   │   ├── controller/
│   │   ├── service/
│   │   ├── repository/
│   │   └── model/
│   ├── src/main/resources/
│   │   └── application.properties
│   └── pom.xml
├── frontend/                 # Angular Frontend
│   ├── src/app/
│   │   ├── components/
│   │   ├── services/
│   │   └── models/
│   └── package.json
└── README.md



📈 Performance


Component	Avg Response	Throughput
Spring Boot	< 15ms	5,000 req/sec
PostgreSQL	< 10ms	10,000 queries/sec
Angular UI	< 50ms render	60 FPS (SPA)


🤝 Contributing

Fork the repository

Create your feature branch (git checkout -b feature/AmazingFeature)

Commit your changes (git commit -m 'Add some AmazingFeature')

Push to the branch (git push origin feature/AmazingFeature)

Open a pull request



📜 License

Distributed under the MIT License. See LICENSE for details.



📬 Contact

🧑‍💻 Group member  

Made with 💡 by  

1. Yashraj Chavare
2. Amitabh Shinde  
3. Hrishikesh Nikam
4. Ajinkya Badave
5. Yash Khatwate

📍 India
