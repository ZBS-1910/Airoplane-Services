# Airplane Service

A microservices-based airplane ticketing system that handles flight management, booking, and notifications.

## 🚀 Services

### 1. API Gateway
- **Port**: 3000
- **Description**: Single entry point for all client requests, routes to appropriate microservices
- **Dependencies**: All other services

### 2. Flight Service
- **Port**: 3001
- **Description**: Manages flight information, schedules, and availability
- **Database**: Mysql (flight_db)

### 3. Booking Service
- **Port**: 3004
- **Description**: Handles flight bookings, reservations, and payment processing
- **Database**: Mysql (booking_db)

### 4. Notification Service
- **Port**: 3003
- **Description**: Sends notifications for booking confirmations, flight updates, etc.

## 🛠️ Prerequisites

- Docker
- Docker Compose
- Node.js (for local development without Docker)

## 🚀 Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/ZBS-1910/Airoplane-Services.git
   cd Airoplane-Service
   ```

2. **Start all services**
   ```bash
   docker-compose up --build
   ```

3. **Access the services**
   - API Gateway: http://localhost:3000
   - Flight Service: http://localhost:3001
   - Booking Service: http://localhost:3004
   - Notification Service: http://localhost:3003

## 🔧 Environment Variables

Each service has its own `.env` file. Copy the `.env.example` to `.env` in each service directory and update the values as needed.

## 🌐 API Documentation

API documentation is available at `http://localhost:3000/api-docs` when the API Gateway is running.


## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Made with ❤️ by ZBS
