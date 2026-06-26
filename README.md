# OOP Bank Management System (C++)

A console-based Bank Management System developed in C++ using Object-Oriented Programming (OOP) principles.

The application enables bank employees to manage clients, perform financial transactions (including account transfers), track transfer history, administer system users through a secure login system with permission-based access control, and use a built-in currency exchange module for viewing currencies, searching currencies, updating exchange rates, and converting amounts between currencies.

User passwords are stored in encrypted form within the data files, and the project also includes a practical implementation of abstraction through an interface-based communication contract.

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

## Development Environment

This project was developed using **Microsoft Visual Studio** and utilizes Microsoft-specific C++ extensions such as `__declspec(property)`.

---

## How to Run

1. Open the project in Microsoft Visual Studio.

2. Ensure the following files exist inside the `Data/` directory:

```text
Clients.txt
Users.txt
LoginRegister.txt
TransferLog.txt
Currencies.txt
```

3. Build the project:

```text
Build -> Build Solution
```

or press:

```text
Ctrl + Shift + B
```

4. Run the application:

```text
Debug -> Start Without Debugging
```

or press:

```text
Ctrl + F5
```

5. Log in using a valid username and its original password (not the encrypted value shown in `Users.txt`).

> **Important:** Passwords stored in `Users.txt` are encrypted. Do **not** enter the encrypted value shown in the file when logging in.

> **Sample Accounts:** All sample users included with this project use the password **`1234`** unless you change it through the application or edit the data files manually.

> **Note:** User accounts and permissions are managed through `Users.txt`.

> **Note:** This project uses Microsoft-specific C++ extensions and may require code modifications to compile with GCC/MinGW.

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