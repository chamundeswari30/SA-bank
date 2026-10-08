# SOFTWARE REQUIREMENTS SPECIFICATION (SRS)

## Project Name: SA Bank

### 1. Introduction

#### 1.1 Purpose
The purpose of the **SA Bank** system is to provide a simple and secure banking application that allows customers to manage their bank accounts and perform basic banking operations electronically.

#### 1.2 Scope
The SA Bank system provides the following services:

- Customer registration and login
- Account management
- Balance enquiry
- Deposit money
- Withdraw money
- Money transfer
- Transaction history
- Customer profile management
- Secure logout

#### 1.3 Objectives

- To provide easy access to banking services.
- To reduce manual banking work.
- To provide secure customer account management.
- To allow customers to view their transactions.
- To provide quick and convenient banking operations.

---

# 2. Overall Description

## 2.1 Product Perspective

SA Bank is a banking management application that can be used by customers to perform basic banking activities through a computer or web-based system.

## 2.2 Users

### Customer
The customer can:
- Register an account.
- Login securely.
- Check account balance.
- Deposit money.
- Withdraw money.
- Transfer money.
- View transaction history.
- Update profile details.

### Bank Administrator
The administrator can:
- Manage customer accounts.
- View customer information.
- Monitor transactions.
- Activate or deactivate accounts.

---

# 3. Functional Requirements

## FR1 – Customer Registration

The system shall allow a new customer to create a bank account by entering:

- Name
- Date of birth
- Address
- Phone number
- Email
- Password
- Account details

## FR2 – Customer Login

The system shall allow registered customers to login using:

- Username/Account number
- Password

The system shall reject invalid login details.

## FR3 – Account Management

The customer shall be able to:

- View account details.
- View account number.
- Update personal information.
- Change password.

## FR4 – Balance Enquiry

The system shall display the current account balance of the customer.

## FR5 – Deposit

The customer shall be able to deposit money into the account.

The system shall:

1. Accept the deposit amount.
2. Validate the amount.
3. Add the amount to the account balance.
4. Record the transaction.

## FR6 – Withdrawal

The customer shall be able to withdraw money.

The system shall:

1. Accept the withdrawal amount.
2. Check the available balance.
3. Reject the transaction if sufficient balance is not available.
4. Deduct the amount from the balance.
5. Record the transaction.

## FR7 – Money Transfer

The customer shall be able to transfer money to another bank account.

The system shall:

- Accept the receiver's account number.
- Accept the transfer amount.
- Check the sender's balance.
- Deduct the amount from the sender.
- Credit the receiver.
- Record the transaction.

## FR8 – Transaction History

The system shall display previous transactions including:

- Date
- Transaction type
- Amount
- Account details
- Transaction status

## FR9 – Profile Management

The customer shall be able to update personal details such as:

- Address
- Phone number
- Email

## FR10 – Logout

The system shall provide a logout option.

After logout, the user session shall be terminated securely.

---

# 4. Non-Functional Requirements

## 4.1 Security

- User passwords shall be protected.
- Only authenticated users can access account information.
- Users shall not be able to access another customer's account.
- The system shall provide secure logout.

## 4.2 Performance

- The system should respond quickly to user requests.
- Transactions should be processed without unnecessary delay.

## 4.3 Reliability

- The system should operate correctly without losing transaction information.
- Banking transactions should be recorded accurately.

## 4.4 Usability

- The system should have a simple and user-friendly interface.
- Menus and buttons should be easy to understand.
- Error messages should be clear.

## 4.5 Availability

- The system should be available whenever banking services are required.
- The system should minimize downtime.

## 4.6 Maintainability

- The software should be easy to maintain and update.
- The system should use a modular design.

---

# 5. System Requirements

## 5.1 Hardware Requirements

- Processor: Intel Core i3 or above
- RAM: 4 GB or above
- Hard Disk: 10 GB free space
- Keyboard and Mouse
- Internet connection

## 5.2 Software Requirements

- Operating System: Windows/Linux
- Frontend: HTML, CSS, JavaScript
- Backend: Python/Java/PHP
- Database: MySQL
- Browser: Google Chrome / Microsoft Edge
- Development Tool: VS Code / Notepad

---

# 6. System Modules

The SA Bank system consists of the following modules:

### 6.1 Registration Module
Used to register new customers.

### 6.2 Login Module
Used to authenticate customers.

### 6.3 Account Module
Used to manage customer account information.

### 6.4 Deposit Module
Used to deposit money.

### 6.5 Withdrawal Module
Used to withdraw money.

### 6.5 Transfer Module
Used to transfer money between accounts.

### 6.6 Transaction Module
Used to store and display transaction history.

### 6.7 Admin Module
Used by the administrator to manage customers and transactions.

### 6.8 Logout Module
Used to securely end the customer session.

---

# 7. Database Requirements

The system may contain the following tables:

## Customer Table

| Field | Description |
|---|---|
| Customer_ID | Unique customer ID |
| Name | Customer name |
| DOB | Date of birth |
| Phone | Phone number |
| Email | Email address |
| Address | Customer address |
| Password | Login password |

## Account Table

| Field | Description |
|---|---|
| Account_No | Unique account number |
| Customer_ID | Customer reference |
| Account_Type | Type of account |
| Balance | Current balance |
| Status | Account status |

## Transaction Table

| Field | Description |
|---|---|
| Transaction_ID | Unique transaction ID |
| Account_No | Account number |
| Transaction_Type | Deposit/Withdrawal/Transfer |
| Amount | Transaction amount |
| Date | Transaction date |
| Status | Transaction status |

---

# 8. Use Cases

| Use Case | Actor | Description |
|---|---|---|
| Register | Customer | Create a new account |
| Login | Customer | Login to the system |
| Check Balance | Customer | View current balance |
| Deposit | Customer | Deposit money |
| Withdraw | Customer | Withdraw money |
| Transfer | Customer | Transfer money |
| View History | Customer | View previous transactions |
| Manage Account | Customer | Update account details |
| Manage Customers | Admin | Manage customer accounts |
| Logout | Customer | Exit the system securely |

---

# 9. Constraints

- Users must have valid login credentials.
- Transactions cannot be performed without sufficient balance.
- Account numbers must be unique.
- Required customer information must be provided during registration.
- The system requires a database to store customer and transaction information.

---

# 10. Future Enhancements

The following features can be added in future:

- ATM integration
- Mobile banking application
- Online bill payment
- Loan management
- Credit/debit card management
- OTP-based authentication
- Email/SMS transaction notifications
- QR-code payments
- Digital passbook

---

# 11. Conclusion

The **SA Bank** system provides a simple and efficient way for customers to manage their banking activities. It supports registration, login, balance enquiry, deposit, withdrawal, money transfer, and transaction history. The system aims to provide secure, reliable, and user-friendly banking services while reducing manual work.