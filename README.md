# Saloon Booking Project - Full Stack Microservices Application

## About the Project
The **Saloon Booking Project** is a full-stack application built with a **microservices architecture**. It allows users to book salon services, while salon owners can manage their services, track bookings, and monitor revenue. The system ensures secure authentication, real-time notifications, and seamless payment integration.

---

## Features

### User Features
- Register and login securely.
- Browse salons and services.
- Book appointments with chosen services.
- Track booking history and payment status.

### Salon Owner Features
- Create and manage salons and service offerings.
- Track bookings by date, customer, or salon.
- Generate revenue reports.
- Manage categories and services efficiently.

### Admin Features
- Manage user roles and permissions using **Keycloak**.
- Monitor overall platform activity.

---

## Technology Stack

### Backend
- **Spring Boot**: Backend microservices.
- **Keycloak**: Authentication and authorization.
- **JWT**: Token-based security.
- **MySQL**: Relational database.
- **RabbitMQ**: Event-driven communication.
- **WebSocket**: Real-time notifications.

### Frontend
- **React.js**: Dynamic user interfaces.
- **TailwindCSS**: Styling.
- **Redux**: State management.
- **Material-UI (MUI)**: UI components.
- **Formik**: Forms and validation.

### Payment Gateway
- **Razorpay**: Payment integration for bookings.

### DevOps & Tools
- **Docker**: Containerization for backend services and Keycloak.
- **IntelliJ IDEA**: Backend development IDE.
- **VS Code**: Frontend development editor.

---

## Project Setup

### Backend
1. Clone the repository.
2. Run all microservices.
3. Install and run Keycloak using Docker:

```bash
docker run -p 8080:8080 -e KC_BOOTSTRAP_ADMIN_USERNAME=admin -e KC_BOOTSTRAP_ADMIN_PASSWORD=admin quay.io/keycloak/keycloak:26.1.0 start-dev

Configure clients, roles (CUSTOMER, SALON_OWNER), and admin in Keycloak.
Update CLIENT_ID, CLIENT_SECRET, and user credentials in the user service configuration.

### Frontend 
