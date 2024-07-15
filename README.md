# Banking Application

This is a Spring Boot-based banking application that provides RESTful APIs for managing bank accounts. The application allows users to perform various operations such as creating accounts, retrieving account details, depositing money, withdrawing money, and deleting accounts.

## Features

1. **Create Account**: Add a new bank account.
2. **Get Account**: Retrieve details of an account by its ID.
3. **Deposit Money**: Deposit a specified amount into an account.
4. **Withdraw Money**: Withdraw a specified amount from an account.
5. **Get All Accounts**: Retrieve a list of all bank accounts.
6. **Delete Account**: Delete a specified account.

## Technologies Used

- **Spring Boot**: Framework for building Java applications.
- **Spring MVC**: For designing and implementing RESTful web services.
- **Spring Data JPA**: For data persistence and database interaction.
- **H2 Database**: In-memory database for development and testing.
- **Maven**: For project management and dependency management.

## Getting Started

### Prerequisites

- Java Development Kit (JDK) 8 or higher
- Maven

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/banking-app.git
   cd banking-app
2. Build the project:
mvn clean install

3.Run the application:

mvn spring-boot:run

API Endpoints
Create Account

Endpoint: POST /api/accounts
Request Body: AccountDto
Response: AccountDto
Get Account by ID

Endpoint: GET /api/accounts/{id}
Response: AccountDto
Deposit Money

Endpoint: PUT /api/accounts/{id}/deposit
Request Body: { "amount": double }
Response: AccountDto
Withdraw Money

Endpoint: PUT /api/accounts/{id}/withdraw
Request Body: { "amount": double }
Response: AccountDto
Get All Accounts

Endpoint: GET /api/accounts
Response: List<AccountDto>
Delete Account

Endpoint: DELETE /api/accounts/{id}
Response: String

## Example Request and Response
Create Account

Request
POST /api/accounts
{
  "accountHolderName": "John Doe",
  "balance": 1000.0
}
Response

{
  "id": 1,
  "accountHolderName": "John Doe",
  "balance": 1000.0
}
Get Account by ID

Response
GET /api/accounts/1
{
  "id": 1,
  "accountHolderName": "John Doe",
  "balance": 1000.0
}
Contributing
Contributions are welcome! Please open an issue or submit a pull request for any improvements or new features.

License
This project is licensed under the MIT License. See the LICENSE file for details.







