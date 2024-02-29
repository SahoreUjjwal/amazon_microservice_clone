# Amazon Clone Backend

This repository contains the backend services for an Amazon clone application. The backend is built using Node.js and follows a microservices architecture. Here's an overview of the different microservices and their responsibilities:

1. **Customer Service**:
   - Handles all user-related events.
   - Manages user authentication, registration, and profile information.
   - Communicates with the front end to provide user-specific data.

2. **Product Service**:
   - Responsible for product-related events.
   - Manages product catalog, inventory, and details.
   - Supports product search, filtering, and recommendations.

3. **Shopping Microservice**:
   - Handles order-related events.
   - Manages shopping cart, checkout process, and order history.
   - Integrates with payment gateways for secure transactions.

## Event-Driven Architecture

The communication between microservices is based on an event-driven architecture. We use RabbitMQ as the message broker to facilitate asynchronous communication. Events are published and consumed by the relevant services, ensuring loose coupling and scalability.

## Technologies Used

- **Node.js**: Backend services are written in Node.js for their flexibility and performance.
- **Express.js**: A lightweight web application framework for building APIs.
- **MongoDB**: Used for data storage (user profiles, product details, orders).
- **RabbitMQ**: The message broker for event communication.
- **Docker**: Each microservice is containerized using Docker for easy deployment and scalability.
- **Nginx**: Configured as a reverse proxy to handle incoming requests and distribute them to the appropriate microservices.

## Getting Started

1. **Clone the Repository**:

git clone https://github.com/your-username/amazon-clone-backend.git


2. **Install Dependencies**:

install docker on your system

cd amazon-clone-backend

run: docker-compose build
run: docker-compose up

## Contributing
Contributions are welcome! Feel free to open issues or submit pull requests.
