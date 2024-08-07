# Project Overview

This project is a Spring Boot application that includes various functionalities such as employee management, validation, and global exception handling. The project uses Maven for dependency management.

## Technologies Used

- **Java**
- **Spring Boot**
- **Maven**

## Project Structure

### DTOs

#### `EmployeeDTO.java`

This class represents the Data Transfer Object for an employee and includes various validation annotations to ensure data integrity.

### Exception Handling

#### `GlobalExceptionHandler.java`

This class handles exceptions globally across the application. It includes handlers for:

- `ResourceNotFoundException`
- `Exception`
- `MethodArgumentNotValidException`

### Response Handling

#### `GlobalResponseHandler.java`

This class implements `ResponseBodyAdvice` to wrap all responses in a consistent format using the `ApiResponse` class.

## Validation Annotations

- `@NotBlank`
- `@Size`
- `@Email`
- `@NotNull`
- `@Max`
- `@Min`
- `@PositiveOrZero`
- `@Digits`
- `@DecimalMin`
- `@DecimalMax`
- `@PastOrPresent`
- `@AssertTrue`
- `@Positive`
- `@FutureOrPresent`
- `@CreditCardNumber`
- `@Range`
- `@AssertFalse`
- `@PasswordValidation`
- `@EmployeeRoleValidation`
- `@PrimeNumberValidation`

## API Endpoints

### Employee Management

- **Create Employee**
    - **URL**: `/api/employees`
    - **Method**: `POST`
    - **Request Body**: `EmployeeDTO`
    - **Response**: `ApiResponse<EmployeeDTO>`
    - **Description**: Creates a new employee.

- **Get Employee by ID**
    - **URL**: `/api/employees/{id}`
    - **Method**: `GET`
    - **Response**: `ApiResponse<EmployeeDTO>`
    - **Description**: Retrieves an employee by their ID.

- **Update Employee**
    - **URL**: `/api/employees/{id}`
    - **Method**: `PUT`
    - **Request Body**: `EmployeeDTO`
    - **Response**: `ApiResponse<EmployeeDTO>`
    - **Description**: Updates an existing employee.

- **Delete Employee**
    - **URL**: `/api/employees/{id}`
    - **Method**: `DELETE`
    - **Response**: `ApiResponse<Void>`
    - **Description**: Deletes an employee by their ID.

### Exception Handling

- **Resource Not Found**
    - **Status**: `404`
    - **Response**: `ApiResponse<ApiError>`
    - **Description**: Returned when a requested resource is not found.

- **Internal Server Error**
    - **Status**: `500`
    - **Response**: `ApiResponse<ApiError>`
    - **Description**: Returned when an internal server error occurs.

- **Method Argument Not Valid**
    - **Status**: `400`
    - **Response**: `ApiResponse<ApiError>`
    - **Description**: Returned when input validation fails.

## How to Run

1. Clone the repository.
2. Navigate to the project directory.
3. Run `mvn spring-boot:run`.


## 🚀 About Me

Tech-savvy learner/programmer pushing boundaries of online tech. Passionate about new tools, seeking challenges to advance skills.

## 🔗 Social Links

![Name](https://img.shields.io/badge/Name-Francis%20Rudra%20D%20Cruze-yellowgreen?style=for-the-badge)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rudradcruze)
[![twitter](https://img.shields.io/badge/twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/rudradcruze)
[![Facebook](https://img.shields.io/badge/facebook-4267B2?style=for-the-badge&logo=facebook&logoColor=white)](https://facebook.com/rudradcruze)
[![francisrudra@gmail.com](https://img.shields.io/badge/gmail-4267B2?style=for-the-badge&logo=gmail&logoColor=white)](mailto:francisrudra@gmail.com)