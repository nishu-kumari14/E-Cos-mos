
# 🌟 Cosmos E-commerce Platform
*Everything available here*

[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.5.3-brightgreen.svg)](https://spring.io/projects/spring-boot)
[![Java](https://img.shields.io/badge/Java-17-orange.svg)](https://www.oracle.com/java/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/nishu-kumari14/E-Cos-mos.svg)](https://github.com/nishu-kumari14/E-Cos-mos/stargazers)

A modern, responsive e-commerce web application built with Spring Boot featuring a beautiful UI, comprehensive product management, and seamless shopping experience.

![Cosmos Logo](https://img.shields.io/badge/🛍️-Cosmos-purple?style=for-the-badge&logoColor=white)

## 🚀 Live Demo
Access the application: **http://localhost:8081** (when running locally)

## ✨ Features

### 🔐 Authentication & Security
- **Secure User Registration & Login** with Spring Security
- **Role-based Access Control** (Admin, Seller, Customer)
- **Session Management** with automatic logout
- **Password Encryption** using BCrypt

### 🛍️ Product Management
- **Dynamic Product Catalog** with image uploads
- **Category-based Filtering** with sidebar navigation
- **Real-time Stock Management** with quantity tracking
- **Product Search & Browse** functionality
- **Seller Dashboard** for inventory management

### 🛒 Shopping Experience
- **Interactive Shopping Cart** with quantity updates
- **Wishlist Management** for favorite products
- **Seamless Checkout Process** with order confirmation
- **Order History Tracking** with status updates
- **Responsive Design** for mobile and desktop

### 🎨 Modern UI/UX
- **Beautiful Gradient Design** with modern aesthetics
- **Responsive Layout** that works on all devices
- **Font Awesome Icons** for enhanced visual experience
- **Smooth Animations** and hover effects
- **Professional Typography** and color scheme

## 🛠️ Technologies Used

| Technology | Version | Purpose |
|------------|---------|---------|
| **Java** | 17 | Core programming language |
| **Spring Boot** | 3.5.3 | Application framework |
| **Spring Security** | 6.x | Authentication & authorization |
| **Spring Data JPA** | 3.x | Data persistence layer |
| **Hibernate** | 6.x | ORM framework |
| **H2 Database** | 2.3.232 | In-memory database |
| **Thymeleaf** | 3.x | Template engine |
| **Maven** | 3.x | Build automation |
| **Font Awesome** | 6.0.0 | Icons library |
| **HTML5/CSS3** | Latest | Frontend technologies |

## 📋 Prerequisites

Before running this application, make sure you have:

- ☕ **Java JDK 17** or higher
- 📦 **Maven 3.6+** for dependency management
- 🌐 **Web Browser** (Chrome, Firefox, Safari, Edge)
- 💻 **IDE** (IntelliJ IDEA, Eclipse, VS Code)

## 🔧 Setup and Installation

### 1. Clone the Repository
```bash
git clone https://github.com/nishu-kumari14/E-Cos-mos.git
cd E-Cos-mos
```

### 2. Configure Application Properties
The application uses H2 in-memory database by default. Configuration in `application.properties`:

```properties
# Server Configuration
server.port=8081

# H2 Database Configuration
spring.datasource.url=jdbc:h2:mem:testdb
spring.datasource.driverClassName=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=

# JPA Configuration
spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
spring.jpa.hibernate.ddl-auto=create-drop
spring.jpa.show-sql=true
spring.h2.console.enabled=true

# File Upload Configuration
spring.servlet.multipart.enabled=true
spring.servlet.multipart.max-file-size=5MB
spring.servlet.multipart.max-request-size=5MB

# Static Resources
spring.web.resources.static-locations=classpath:/static/,file:uploads/
```

### 3. Build and Run
```bash
# Clean and build the project
./mvnw clean package -DskipTests

# Run the application
java -jar target/E-commerce-0.0.1-SNAPSHOT.jar --server.port=8081
```

### 4. Access the Application
Open your browser and navigate to: **http://localhost:8081**

## 📱 Usage Guide

### For Customers:
1. **Register** a new account or **Login** with existing credentials
2. **Browse Products** on the homepage or filter by categories
3. **Add Products** to cart or wishlist
4. **View Cart** and update quantities as needed
5. **Checkout** to place orders
6. **Track Orders** in the order history section

### For Sellers/Admins:
1. **Login** with seller/admin credentials
2. **Add New Products** with images and descriptions
3. **Manage Inventory** by updating stock quantities
4. **Remove Products** that are no longer available
5. **Monitor Sales** through the dashboard

## 📁 Project Structure

```
src/
├── main/
│   ├── java/com/ecommerce/E_commerce/
│   │   ├── 🎮 controller/          # REST controllers
│   │   │   ├── AuthController.java
│   │   │   ├── CartController.java
│   │   │   ├── HomeController.java
│   │   │   ├── OrderController.java
│   │   │   ├── ProductController.java
│   │   │   └── WishlistController.java
│   │   │
│   │   ├── 🏗️ entity/             # JPA entities
│   │   │   ├── User.java
│   │   │   ├── Product.java
│   │   │   ├── Cart.java
│   │   │   ├── Order.java
│   │   │   └── Wishlist.java
│   │   │
│   │   ├── 💾 repository/         # Data repositories
│   │   │   ├── UserRepository.java
│   │   │   ├── ProductRepository.java
│   │   │   ├── CartRepository.java
│   │   │   └── OrderRepository.java
│   │   │
│   │   ├── 🔧 service/            # Business logic
│   │   │   ├── UserService.java
│   │   │   ├── ProductService.java
│   │   │   ├── CartService.java
│   │   │   └── OrderService.java
│   │   │
│   │   └── ⚙️ config/             # Configuration
│   │       ├── SecurityConfig.java
│   │       └── WebConfig.java
│   │
│   └── resources/
│       ├── 🎨 templates/          # Thymeleaf templates
│       │   ├── home.html
│       │   ├── login.html
│       │   ├── cart.html
│       │   └── wishlist.html
│       │
│       ├── 📱 static/css/         # Stylesheets
│       │   └── style.css
│       │
│       └── 📋 application.properties
│
└── uploads/images/                # Product images storage
```

## 🌟 Key Highlights

### 🎨 Modern Design System
- **Gradient Backgrounds**: Beautiful purple-to-blue gradients
- **Card-based Layout**: Clean, modern product cards
- **Responsive Grid**: Adapts to different screen sizes
- **Hover Effects**: Interactive elements with smooth transitions

### 🔒 Security Features
- **CSRF Protection**: Built-in security against cross-site requests
- **SQL Injection Prevention**: Parameterized queries with JPA
- **XSS Protection**: Template engine prevents script injection
- **Secure Authentication**: BCrypt password hashing

### 📊 Performance Optimizations
- **Connection Pooling**: HikariCP for database connections
- **Lazy Loading**: Efficient data fetching strategies
- **Static Resource Caching**: Optimized CSS and JS delivery
- **Image Optimization**: Proper image handling and storage

## 🚀 Future Enhancements

### 🔮 Planned Features
- [ ] **Payment Gateway Integration** (Razorpay, Stripe)
- [ ] **Email Notifications** for order confirmations
- [ ] **Advanced Search** with filters and sorting
- [ ] **Product Reviews & Ratings** system
- [ ] **Admin Analytics Dashboard**
- [ ] **Multi-language Support** (i18n)
- [ ] **Progressive Web App** (PWA) capabilities
- [ ] **Real-time Chat Support**

### 🏗️ Technical Improvements
- [ ] **Redis Caching** for better performance
- [ ] **Elasticsearch** for advanced search
- [ ] **Docker Containerization**
- [ ] **CI/CD Pipeline** setup
- [ ] **API Rate Limiting**
- [ ] **Monitoring & Logging** (Prometheus, Grafana)

## 🤝 Contributing

We welcome contributions! Here's how you can help:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/AmazingFeature`)
3. **Commit** your changes (`git commit -m 'Add some AmazingFeature'`)
4. **Push** to the branch (`git push origin feature/AmazingFeature`)
5. **Open** a Pull Request

### 📝 Contribution Guidelines
- Follow Java coding standards
- Add unit tests for new features
- Update documentation as needed
- Ensure responsive design compliance

## 📞 Support

Need help? We're here for you!

- 📧 **Email**: nishukumari14@example.com
- 🐛 **Issues**: [GitHub Issues](https://github.com/nishu-kumari14/E-Cos-mos/issues)
- 💬 **Discussions**: [GitHub Discussions](https://github.com/nishu-kumari14/E-Cos-mos/discussions)

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Spring Boot Team** for the amazing framework
- **Font Awesome** for the beautiful icons
- **H2 Database** for the lightweight database solution
- **Thymeleaf Team** for the excellent template engine

---

<div align="center">

**Made with ❤️ by [nishukumari14](https://github.com/nishu-kumari14)**

*If you found this project helpful, please consider giving it a ⭐!*

[![GitHub stars](https://img.shields.io/github/stars/nishu-kumari14/E-Cos-mos.svg?style=social&label=Star)](https://github.com/nishu-kumari14/E-Cos-mos/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/nishu-kumari14/E-Cos-mos.svg?style=social&label=Fork)](https://github.com/nishu-kumari14/E-Cos-mos/network)

</div>
