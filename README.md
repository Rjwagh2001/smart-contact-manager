# 📇 Smart Contact Manager

A full-stack Spring Boot web application for managing contacts with user authentication, CRUD operations, pagination, and search functionality.

![Spring Boot](https://img.shields.io/badge/Spring--Boot-3.1+-green)
![Java](https://img.shields.io/badge/Java-17+-orange)
![MySQL](https://img.shields.io/badge/MySQL-8+-blue)
![License](https://img.shields.io/badge/license-MIT-blue)

---

## ✨ Features

**User Management**
- Secure login/logout with Spring Security
- User registration with BCrypt password encryption

**Contact Management**
- Add, edit, and delete contacts
- View all contacts with pagination
- Search contacts by name/email/phone
- Click contact name to view detailed profile

---

## 🛠️ Tech Stack

- **Backend:** Spring Boot, Spring Security, Spring Data JPA
- **Frontend:** Thymeleaf, Bootstrap 5
- **Database:** MySQL
- **Build Tool:** Maven

---

## 🚀 Quick Start

### Prerequisites
- Java 17+, Maven, MySQL 8+

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/smart-contact-manager.git
cd smart-contact-manager
```

2. **Configure MySQL** (`application.properties`)
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/contact_manager
spring.datasource.username=root
spring.datasource.password=yourpassword
spring.jpa.hibernate.ddl-auto=update
```

3. **Run the application**
```bash
mvn spring-boot:run
```

4. **Access:** `http://localhost:8080`

---

## 📁 Project Structure

```
src/main/java/
├── controller/     # MVC Controllers
├── entity/         # JPA Entities (User, Contact)
├── repository/     # Spring Data JPA Repositories
├── service/        # Business Logic Layer
└── config/         # Security Configuration

src/main/resources/
├── templates/      # Thymeleaf HTML pages
├── static/         # CSS, JS, images
└── application.properties
```

---

## 🔐 Security Features

- Spring Security for authentication
- BCrypt password hashing
- CSRF protection
- Session management
- SQL injection prevention via JPA

---

## 📊 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/signup` | Registration page |
| POST | `/do-register` | User registration |
| GET | `/signin` | Login page |
| GET | `/user/dashboard` | User dashboard |
| GET | `/user/add-contact` | Add contact form |
| POST | `/user/process-contact` | Save contact |
| GET | `/user/show-contacts/{page}` | View contacts (paginated) |
| GET | `/user/contact/{id}` | Contact details |
| POST | `/user/update-contact` | Update contact |
| GET | `/user/delete/{id}` | Delete contact |
| GET | `/user/search` | Search contacts |

---

## 🎯 Skills Demonstrated

✅ Spring Boot & Spring MVC architecture  
✅ Spring Security implementation  
✅ Spring Data JPA with Hibernate  
✅ RESTful design patterns  
✅ Server-side pagination  
✅ Thymeleaf templating  
✅ MySQL database design  
✅ Clean code & layered architecture

---

## 📸 Screenshots

Add screenshots in `/screenshots` folder:
- Login page
- Dashboard
- Contact list with pagination
- Add/Edit contact form
- Search functionality

---

## 🚀 Deployment

Deploy easily on:
- **Railway/Render** (Free tier)
- **Heroku**
- **AWS EC2**
- **Docker**

---

## 🤝 Contributing

1. Fork the repo
2. Create feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add feature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open Pull Request

---

⭐ **Star this repo if you found it helpful!**
