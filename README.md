# Mobile Phone E-Commerce Website - Java Spring Boot Project

## 📋 Project Overview
A comprehensive e-commerce platform for selling mobile phones, developed as a Java Spring Boot application for the university course project. The system provides full-featured online shopping functionality with separate interfaces for customers and administrators.

## 🏗️ Technical Architecture

### Backend Stack
- **Framework**: Spring Boot 3.x
- **Language**: Java 17+
- **Database**: Microsoft SQL Server
- **Build Tool**: Maven
- **IDE**: IntelliJ IDEA Community Edition 2024.1.1 / Spring Tool Suite 4

### Frontend Stack
- **Templates**: Thymeleaf
- **Styling**: HTML, CSS
- **JavaScript**: For interactive components

## 🎯 Core Features

### 👤 Customer Features
- **User Registration & Authentication**: Secure sign-up/login with role-based access
- **Product Browsing**: View products with filtering by category, price, brand
- **Advanced Search**: Find products using various criteria
- **Shopping Cart**: Add/remove items, manage quantities
- **Order Management**: Place orders, view order history, track status
- **Wishlist**: Save favorite products for later
- **Product Reviews**: Rate and comment on purchased products
- **Account Management**: Update personal information, addresses

### 👨‍💼 Admin Features
- **Dashboard**: Overview of sales, statistics, and metrics
- **Product Management**: CRUD operations for products with images
- **Category Management**: Organize products into categories
- **Order Management**: Process orders, update statuses
- **User Management**: Manage customer and admin accounts
- **Feedback Management**: Monitor and respond to customer feedback
- **Reporting**: Sales statistics, revenue analysis by month/year

## 🗃️ Database Design

### Key Entities
- **Accounts**: User credentials and personal information
- **Products**: Phone details, pricing, images, stock
- **Categories**: Product classification
- **Orders & OrderDetails**: Transaction records
- **Comments**: Product reviews
- **Feedbacks**: System feedback
- **Authorities & Roles**: Role-based access control

### Database Features
- Relational design with proper foreign key constraints
- Data integrity with NOT NULL constraints
- Scalable structure for future enhancements

## 🚀 Setup & Installation

### Prerequisites
- Java JDK 17 or higher
- Microsoft SQL Server
- Maven 3.6+
- IDE (IntelliJ IDEA or STS)

### Configuration Steps
1. Clone the repository
2. Configure database connection in `application.properties`:
```properties
spring.datasource.url=jdbc:sqlserver://localhost:1433;databaseName=WebShop
spring.datasource.username=your_username
spring.datasource.password=your_password
```
3. Build the project: `mvn clean install`
4. Run the application: `mvn spring-boot:run`
5. Access at: `http://localhost:8080`

### Default Accounts
- **Admin**: Admin privileges for full system management
- **Customer**: Regular user for shopping functionality

## 📊 Project Structure
```
src/main/java/
├── controller/     # MVC Controllers
├── model/         # Entity classes
├── repository/    # Data access layer
├── service/       # Business logic
└── config/        # Configuration classes

src/main/resources/
├── static/        # CSS, JS, images
├── templates/     # Thymeleaf templates
└── application.properties
```

## 🔐 Security Features
- Spring Security integration
- Password encryption
- Session management
- Role-based authorization (Admin/User)
- CSRF protection

## 📱 Key Interfaces

### Customer Pages
- **Homepage**: Featured products, categories, promotions
- **Product Listing**: Filterable grid view of phones
- **Product Detail**: Full specifications, images, reviews
- **Cart & Checkout**: Multi-step ordering process
- **Account Dashboard**: Personal info, order history

### Admin Panels
- **Product Management**: Add/edit/delete products
- **Order Processing**: Update order statuses
- **User Management**: Customer account oversight
- **Analytics Dashboard**: Sales reports and statistics
- **Feedback System**: Customer interaction management

## 🛠️ Development Notes

### Implemented Successfully
- ✅ Complete MVC architecture with separation of concerns
- ✅ Database integration with proper ORM mapping
- ✅ Responsive and user-friendly interface
- ✅ Full CRUD operations for all major entities
- ✅ Role-based access control system
- ✅ Shopping cart with session management
- ✅ Order processing workflow

### Technical Highlights
- **Spring Boot**: Rapid development with auto-configuration
- **Spring Data JPA**: Simplified database operations
- **Thymeleaf**: Server-side templating with natural templates
- **Bootstrap**: Responsive design framework
- **Maven**: Dependency management and build automation

## 📈 Future Enhancements

### Planned Features
- **AI/ML Integration**: Personalized product recommendations
- **Payment Gateway**: Integration with Visa, Mastercard, PayPal
- **Mobile App**: Native iOS/Android applications
- **Advanced Analytics**: Predictive sales forecasting
- **Inventory Management**: Automated stock alerts
- **Marketing Tools**: Email campaigns, loyalty programs
- **Multi-language Support**: Internationalization
- **API Development**: RESTful APIs for third-party integration

### Performance Optimizations
- Caching implementation with Redis
- Database query optimization
- Image compression and CDN integration
- Lazy loading for product listings

## 👥 Development Team
- **Lê Huỳnh Trọng Nhân** - Database design, UI components, authorization
- **Nguyễn Hoàng Phúc** - Authentication, registration, Q&A system
- **Võ Quang Huy** - Comment system, cart management, account management
- **Ngô Quốc Trọng** - Order history, product search, product details

## 📚 Learning Outcomes
This project demonstrates practical application of:
- Java Spring Boot framework
- MVC design pattern
- Database design and optimization
- Frontend-backend integration
- User experience design
- Team collaboration and version control
- Software documentation

## 📄 License
University Project - Academic Use

## 🤝 Acknowledgments
- Instructor: ThS. Nguyễn Huy Cường
- HUTECH University - Faculty of Information Technology
- Spring Boot community and documentation

---

**Note**: This is a university project developed for educational purposes. The system is designed to be scalable and can be extended for commercial use with additional security and payment gateway implementations.