# Employee Management System (EMS)

A full-stack **Employee Management System (EMS)** built using **Spring Boot** for the backend and **React.js** for the frontend. This system is designed to efficiently manage employee details, including the ability to create, update, view, and delete employee records.

## Features

- **Employee Creation**: Allows users to create new employee records with essential details.
- **Employee View**: View employee details with all relevant information.
- **Employee Update**: Modify or update existing employee details.
- **Employee Deletion**: Delete employee records from the system.

## Technologies Used

### Backend:
- **Spring Boot**: Framework for building the backend REST API.
- **JPA / Hibernate**: For database interaction.
- **MySQL**: Relational database to store employee data.
- **Spring Data JPA**: For easy database access.

### Frontend:
- **React.js**: For building a dynamic and responsive user interface.
- **Axios**: For making HTTP requests from React to the backend API.
- **Bootstrap**: For styling and responsive design.
- **React Router**: For handling client-side routing.

## Setup & Installation

### Prerequisites
- **Java** 11 or higher (for the backend).
- **Node.js** and **npm** (for the frontend).
- **MySQL** or any other compatible database (ensure the database is set up and configured).

### Backend Setup
1. Clone the repository.
2. Navigate to the backend directory and configure the `application.properties` for your MySQL database connection:
    ```properties
    spring.datasource.url=jdbc:mysql://localhost:3306/ems
    spring.datasource.username=root
    spring.datasource.password=password
    ```
3. Build and run the backend application using Maven:
    ```bash
    mvn clean install
    mvn spring-boot:run
    ```
4. The backend should be running on `http://localhost:8080`.

### Frontend Setup
1. Navigate to the frontend directory.
2. Install dependencies:
    ```bash
    npm install
    ```
3. Start the React application:
    ```bash
    npm start
    ```
4. The frontend should be running on `http://localhost:3000`.

## API Endpoints

- **GET** `/api/employees`: Retrieve a list of all employees.
- **GET** `/api/employees/{id}`: Retrieve details of a specific employee by ID.
- **POST** `/api/employees`: Create a new employee record.
- **PUT** `/api/employees/{id}`: Update an existing employee record by ID.
- **DELETE** `/api/employees/{id}`: Delete an employee record by ID.
