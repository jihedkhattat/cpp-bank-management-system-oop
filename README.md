# OOP Bank Management System (C++)

A console-based Bank Management System developed in C++ using Object-Oriented Programming (OOP) principles.

The application allows bank employees to manage clients, perform financial transactions, and administer system users through a secure login system with permission-based access control. All data is stored persistently using text files.

## Features

### Client Management

* List all bank clients
* Add new clients
* Update client information
* Delete clients
* Find clients by account number
* Store client data in text files

### Transactions

* Deposit money
* Withdraw money
* Display total balances
* Automatically update account balances

### User Management

* User authentication and login
* Login activity logging
* View login register history
* Add new users
* Update user information
* Delete users
* Find users
* List all users

### Permission System

* Role-based access control
* User-specific permissions
* Restrict access to system features
* Permission-controlled Login Register access
* Full-access administrator accounts

### Data Persistence

* Clients stored in `Clients.txt`
* Users stored in `Users.txt`
* Login history stored in `LoginRegister.txt`
* Automatic file loading and saving

## Technologies Used

* C++
* Object-Oriented Programming (OOP)
* Inheritance
* Encapsulation
* Classes and Objects
* Static Members and Methods
* File Handling (`fstream`)
* Vectors (`vector`)
* Enumerations (`enum`)
* Microsoft Visual Studio
* Modular Design using Header Files

## Project Structure

### Core Classes

* `clsPerson.h`
* `clsBankClient.h`
* `clsUser.h`

### Utility Classes

* `clsString.h`
* `clsDate.h`
* `clsUtil.h`
* `clsInputValidate.h`

### Screen Classes

* `clsLoginScreen.h`
* `clsMainScreen.h`
* `clsClientListScreen.h`
* `clsAddNewClientScreen.h`
* `clsDeleteClientScreen.h`
* `clsUpdateClientScreen.h`
* `clsFindClientScreen.h`
* `clsTransactionsScreen.h`
* `clsDepositScreen.h`
* `clsWithdrawScreen.h`
* `clsTotalBalancesScreen.h`
* `clsManageUsersScreen.h`
* `clsLoginRegisterScreen.h`
* `clsListUsersScreen.h`
* `clsAddNewUserScreen.h`
* `clsDeleteUserScreen.h`
* `clsUpdateUserScreen.h`
* `clsFindUserScreen.h`

### Other Files

* `Global.h`
* `Clients.txt`
* `Users.txt`
* `LoginRegister.txt`
* `main.cpp`

## Development Environment

This project was developed using **Microsoft Visual Studio** and utilizes Microsoft-specific C++ extensions such as `__declspec(property)`.

## How to Run

1. Open the project in Microsoft Visual Studio.

2. Ensure the following files exist in the project directory:

```text
Clients.txt
Users.txt
LoginRegister.txt
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

5. Log in using a valid username and password stored in `Users.txt`.

> Note: User accounts and permissions are managed through the `Users.txt` file.

> Note: This project uses Microsoft-specific C++ extensions and may require code modifications to compile with GCC/MinGW.

## Learning Objectives

This project demonstrates:

* Object-Oriented Programming design
* Class inheritance and code reuse
* Encapsulation and abstraction
* File-based data management
* User authentication systems
* Permission-based authorization
* Modular software architecture
* Banking transaction processing
* Multi-screen console application development

## Key OOP Concepts Applied

* Base and derived classes
* Inheritance
* Encapsulation
* Composition
* Static methods
* Class properties
* Object persistence
* Data abstraction
* Access modifiers
* Enumerations within classes
