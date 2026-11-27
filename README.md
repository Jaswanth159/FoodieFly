# 🍔 FoodieFly - Full-Stack Food Delivery Web App

**FoodieFly** is a full-stack web application designed to streamline the food delivery process. It offers a seamless experience for customers to browse menus, place orders, and manage preferences, along with powerful tools for admins to manage orders and menu items.

---

## 🚀 Features

* **User Authentication**: Secure sign-up/login for customers.
* **Browse Menu**: Dynamic food listings with descriptions, images, and pricing.
* **Order Management**: Add to cart, customize orders, and track real-time order status.
* **Admin Dashboard**: Manage menu items, view customer orders, and oversee delivery status.
* **Responsive Design**: Mobile-friendly and desktop-optimized UI.
* **Real-time Updates**: Instant status updates for ongoing orders.

---

## 💻 Technologies Used

### Frontend

* **HTML5**: Semantic structure.
* **CSS3**: Styling and responsive design.
* **JavaScript (ES6+)**: Dynamic user interactions.

### Backend

* **Java (JSE, JEE)**: Core application logic.
* **Spring MVC**: Framework for building robust web applications.
* **Hibernate**: ORM for efficient database communication.
* **JavaMail API**: Sends order confirmations and notifications.

### Database

* **MySQL**: Stores user data, menu items, and orders.

---

## ⚙️ Installation & Setup

### Prerequisites

* Java JDK 11+
* Apache Tomcat 9+
* MySQL Server
* Maven

### Steps

1. **Clone the Repository**

   ```bash
   git clone https://github.com/yourusername/tap-foods.git
   cd tap-foods
   ```

2. **Set Up MySQL Database**

   * Create a database named `tap_foods`.
   * Run the SQL script from the `/db` folder to create tables.

3. **Configure Application**
   Update `src/main/resources/application.properties` with your DB credentials:

   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/tap_foods
   spring.datasource.username=yourUsername
   spring.datasource.password=yourPassword
   ```

4. **Build and Run**

   ```bash
   mvn clean install
   mvn spring-boot:run
   ```

5. **Access the Application**

   * Open [http://localhost:8080](http://localhost:8080) in your browser.

---

## 🗂️ Project Structure

```
tap-foods/
├── src/
│   ├── main/
│   │   ├── java/com/tapfoods/
│   │   │   ├── DAO/
│   │   │   ├── DAOImpl/
│   │   │   ├── model/
│   │   │   ├── servlets/
│   │   │   └── utility/
│   │   ├── resources/
│   │   │   ├── static/         # CSS, JS, images
│   │   │   ├── templates/      # Thymeleaf or JSP views
│   │   │   └── application.properties
│   │   └── webapp/             # Web assets (if any)
│   └── test/                   # Unit & integration tests
├── db/                         # SQL scripts
├── pom.xml                     # Maven dependencies
├── README.md
└── .gitignore
```

---

## 🌟 Future Improvements

* 🔄 **Automation**: Daily deals, scheduled promotions.
* 🤖 **AI Integration**: Personalized dish suggestions.
* 💳 **Payment Gateway**: Secure payment integration.
* 🔔 **Push Notifications**: Real-time order alerts.

---

## 🤝 Contributions

We welcome contributions!
Fork the repo, make your changes, and submit a pull request.
For major changes, please open an issue first to discuss what you'd like to do.
