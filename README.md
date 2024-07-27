# .NET Developer Task

## Objective
Develop a Financial Transactions Management API using .NET. The API should allow users to perform CRUD (Create, Read, Update, Delete) operations on Transaction entities, and generate a summary report.

## Requirements

### Environment Setup
- Use the latest .NET version
- Use Entity Framework (or other ORM of your choice)
- Use SQL Server for the database

### Entity Definition
A transaction should contain at least the following properties:
- `TransactionId`
- `Amount`
- `TransactionType` (either "Credit" or "Debit")
- `TransactionDate`
- `Description`
- `Status` (Failed, Successful, Voided)
- `CustomerFullName`
- `CustomerMainPhoneNumber`
- `CustomerMainAddress`
- `CustomerMainEmailAddress`

### API Endpoints
Implement the following API endpoints:
- **Create a Transaction**: `POST /api/transactions`
- **Get All Transactions**: `GET /api/transactions` (provide filtering options)
- **Get a Transaction by ID**: `GET /api/transactions/{id}`
- **Update a Transaction**: `PUT /api/transactions/{id}`
- **Delete a Transaction**: `DELETE /api/transactions/{id}`
- **Get Transaction Summary**: `GET /api/transactions/summary`
  - **Response**: A JSON object containing the total number of transactions, total credits, total debits, and net balance. Provide filtering options based on the customer.

### Documentation
Use Swagger to generate API documentation.

## Setup Instructions

1. **Clone the repository**
   ```sh
   git clone https://github.com/your-username/financial-transactions-api.git
   cd financial-transactions-api
