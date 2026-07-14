# OOP Bank Management System (C++)

A console-based Bank Management System developed in C++ using Object-Oriented Programming (OOP) principles.

The application enables bank employees to manage clients, perform financial transactions (including account transfers), track transfer history, administer system users through a secure login system with permission-based access control, and use a built-in currency exchange module for viewing currencies, searching currencies, updating exchange rates, and converting amounts between currencies.

User passwords are stored in encrypted form within the data files, and the project also includes a practical implementation of abstraction through an interface-based communication contract.

---

## How to Run

### Requirements

Before running the project, make sure you have:

- Visual Studio Code
- The Microsoft **C/C++** extension for Visual Studio Code
- CMake available on your system

### Run the Application

1. Clone or download the repository.
2. Open a terminal inside the project folder.
3. Open the project in Visual Studio Code:

```powershell
code .
```

4. Install the recommended Microsoft C/C++ extension if prompted.
5. Press `F5` to build and run the application.

### Sample Login

Use the following full-access sample account:

```text
Username: User2
Password: 1234
```

All sample users included with the project use the password **`1234`**, unless it has been changed through the application or directly in the data files.

> **Important:** Passwords in `Users.txt` are stored in encrypted form. When logging in, enter the original password (`1234` for the sample accounts), not the encrypted value displayed in the file.

---

## Features

### Client Management

- List all bank clients
- Add new clients
- Update client information
- Delete clients
- Find clients by account number
- Store client data in text files

### Transactions

- Deposit money
- Withdraw money
- Transfer money between client accounts
- Display total balances
- Automatically update account balances
- Record transfer operations in a transfer log
- View transfer history and transaction details

### User Management

- User authentication and login
- Login activity logging
- View login register history
- Add new users
- Update user information
- Delete users
- Find users
- List all users
- Store user passwords in encrypted form inside `Users.txt`

### Currency Exchange

- List all available currencies
- Find a currency by code or country
- Update currency exchange rates
- Convert amounts between currencies
- Convert any currency to USD
- Convert between any two currencies using USD as the intermediate base
- Persist currency data using `Currencies.txt`

### Permission System

- Role-based access control
- User-specific permissions
- Restrict access to system features
- Permission-controlled Login Register access
- Full-access administrator accounts

### Data Persistence

- Clients stored in `Clients.txt`
- Users stored in `Users.txt` with encrypted passwords
- Login history stored in `LoginRegister.txt`
- Transfer history stored in `TransferLog.txt`
- Currency data stored in `Currencies.txt`
- Automatic file loading and saving

---

## Technologies Used

- C++
- Object-Oriented Programming (OOP)
- Inheritance
- Encapsulation
- Abstraction
- Classes and Objects
- Abstract Classes / Interfaces
- Static Members and Methods
- File Handling (`fstream`)
- File-based Persistence
- Vectors (`vector`)
- Enumerations (`enum`)
- Microsoft Visual Studio
- Modular Design

---

## Project Structure

```text
cpp-bank-management-system/
│
├── Data/
│   ├── Clients.txt
│   ├── Users.txt
│   ├── LoginRegister.txt
│   ├── TransferLog.txt
│   └── Currencies.txt
│
├── Core/
│   ├── clsBankClient.h
│   ├── clsCurrency.h
│   ├── clsPerson.h
│   ├── clsUser.h
│   └── InterfaceCommunication.h
│
├── Lib/
│   ├── clsDate.h
│   ├── clsInputValidate.h
│   ├── clsString.h
│   └── clsUtil.h
│
├── Screens/
│   ├── Client/
│   ├── Currencies/
│   ├── User/
│   ├── clsMainScreen.h
│   └── clsScreen.h
│
├── Global.h
├── main.cpp
└── README.md
```

---

## Learning Objectives

This project demonstrates:

- Object-Oriented Programming design
- Class inheritance and code reuse
- Encapsulation and abstraction
- Interface-based programming
- File-based data management
- User authentication systems
- Permission-based authorization
- Modular software architecture
- Banking transaction processing
- Currency exchange and conversion logic
- Multi-screen console application development
- Transaction and login audit logging
- Simple text encryption/decryption for persisted credentials

---

## Key OOP Concepts Applied

- Classes and Objects
- Inheritance
- Encapsulation
- Abstraction
- Polymorphism through pure virtual functions
- Composition
- Static members and methods
- Object persistence
- Access modifiers
- Enumerations within classes
- Interface-based design
- Domain modeling through specialized business classes