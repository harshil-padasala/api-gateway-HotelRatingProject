# API Gateway Service 🌐

Welcome to the API Gateway Service! This service acts as the central entry point for the microservices in our system, providing a unified interface to access various functionalities.

## Quick Start 🚀

1. **Clone Repository:**
   ```bash
   git clone https://github.com/yourusername/apigateway.git

2. **Run API Gateway Service:**
   ```bash
   cd apigateway
    ./mvnw clean package
    java -jar target/apigateway-1.0.0.jar

3. **Access API Gateway:**
  - Visit http://localhost:8080 to interact with the API Gateway Service.

## Microservices Integration 🔄

The API Gateway Service integrates with the following microservices:

  - User Service: http://localhost:8081
  - Hotel Service: http://localhost:8082
  - Rating Service: http://localhost:8083

## API Endpoints 🛣️

### User Service
  - **Create User:**
    ```bahs
    POST http://localhost:8080/users

  - **Get User by ID:**
    ```bash
    GET http://localhost:8080/users/{userId}
    
  - **Get All Users:**
    ```bash
    GET http://localhost:8080/users

  - **Delete User:**
    ```bash
    DELETE http://localhost:8080/users/{userId}

  - **Update User:**
    ```bash
    PUT http://localhost:8080/users/{userId}
    
### Hotel Service
  - **Create Hotel:**
    ```bash
    POST http://localhost:8080/hotels

  - **Get Hotel by ID:**
    ```bash
    GET http://localhost:8080/hotels/{hotelId}

  - **Get All Hotels:**
    ```bash
    GET http://localhost:8080/hotels

  - **Delete Hotel:**
    ```bash
    DELETE http://localhost:8080/hotels/{hotelId}

  - **Update Hotel:**
    ```bash
    PUT http://localhost:8080/hotels/{hotelId}

### Rating Service
  
  - **Create Rating:**
    ```bash
    POST http://localhost:8080/ratings

  - **Get All Ratings:**
    ```bash
    GET http://localhost:8080/ratings

  - **Get Ratings by User ID:**
    ```bash
    GET http://localhost:8080/ratings/user-id/{userId}

  - **Get Ratings by Hotel ID:**
    ```bash
    GET http://localhost:8080/ratings/hotel-id/{hotelId}

  - **Delete Rating by ID:**
    ```bash
    DELETE http://localhost:8080/ratings/{ratingId}
