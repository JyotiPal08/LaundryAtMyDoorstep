# Laundry at My Doorstep

## Overview
**Laundry at My Doorstep** is a web application designed to bridge the gap between customers and laundry service providers. The platform offers a seamless and user-friendly interface for requesting laundry services, enhancing convenience and efficiency for users.

## Key Features
- **User Roles:**
  - **Customers:**
    - Register and log in to the platform.
    - View available laundry services.
    - Place and manage laundry orders.
    - Track the status of orders in real time.
  - **Service Providers:**
    - Register and log in to the platform.
    - Manage orders from customers.
    - Update order statuses (e.g., picked up, in process, delivered).
- **Authentication:** Secure authentication using JWT.
- **Responsive Design:** Fully responsive UI for optimal usability on both desktop and mobile devices.

## Technology Stack
- **Frontend:** React.js with Material-UI for a polished and modern design.
- **Backend:** Spring Boot to handle the business logic and API endpoints.
- **Database:** MySQL for data storage and management.
- **Authentication:** JWT for secure user authentication and role management.

## Installation Guide

### Prerequisites
- **Node.js** (for running the React.js application)
- **Java JDK 11 or higher** (for Spring Boot)
- **MySQL** (for database)

### Steps to Run
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/laundry-at-my-doorstep.git
   cd laundry-at-my-doorstep
   ```

2. **Backend Setup:**
   - Navigate to the backend folder:
     ```bash
     cd backend
     ```
   - Configure the database connection in `application.properties`:
     ```properties
     spring.datasource.url=jdbc:mysql://localhost:3306/laundry_db
     spring.datasource.username=your_username
     spring.datasource.password=your_password
     ```
   - Run the Spring Boot application:
     ```bash
     ./mvnw spring-boot:run
     ```

3. **Frontend Setup:**
   - Navigate to the frontend folder:
     ```bash
     cd ../frontend
     ```
   - Install dependencies:
     ```bash
     npm install
     ```
   - Start the React.js application:
     ```bash
     npm start
     ```

4. **Access the Application:**
   - Open your browser and go to `http://localhost:3000`.

## API Endpoints
- **Authentication:**
  - `POST /api/auth/login`: Log in user.
  - `POST /api/auth/register`: Register user.
- **Customers:**
  - `GET /api/orders`: Fetch customer orders.
  - `POST /api/orders`: Place a new order.
- **Service Providers:**
  - `GET /api/orders/all`: View all orders.
  - `PUT /api/orders/{id}`: Update order status.

## Contribution
Contributions are welcome! Follow these steps:
1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add your message here"
   ```
4. Push to the branch:
   ```bash
   git push origin feature/your-feature-name
   ```
5. Open a pull request.

## License
This project is licensed under the [MIT License](LICENSE).

## Contact
For queries, feel free to reach out:
- **Name:** Jyoti Pal
- **Email:** [26jyotipal@gmail.com](mailto:26jyotipal@gmail.com)

