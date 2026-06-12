# ATM Interface - Project 3

**Developer:** Dhanshu
**Organization:** DecodeLabs (Industrial Training Kit - Batch 2026)

## Overview
The ATM Interface is a Java-based enterprise-grade application designed to handle financial transactions securely using Object-Oriented Programming (OOP) principles. This project focuses on building a resilient digital twin of a physical ATM, emphasizing data encapsulation, input validation, and the separation of the user interface from the core business logic.

## Key Features
* **Decoupled Architecture:** Maintains a strict separation of concerns between the User Interface (`ATM` class) and the Data Vault / Business Logic (`BankAccount` class).
* **Strict Encapsulation:** Protects sensitive internal state (such as account balances) using private variables and secure mutator methods.
* **Robust Input Validation:** Acts as a security gate, utilizing `hasNextDouble()` and `hasNextInt()` to elegantly handle malformed user input without crashing the application.
* **Secure Transaction Rules:** Implements rigorous business logic to prevent overdrafts, reject negative deposits, and ensure mathematical precision.
* **Continuous Session Management:** Provides an interactive console menu allowing users to seamlessly check balances, deposit funds, and withdraw cash until they choose to exit.

## Technical Architecture
* **BankAccount (The Vault):** Handles all financial math and enforces overdraft rules. It operates completely independently of the console.
* **ATM (The Lobby):** Manages the human element, orchestrating the `Scanner`, displaying menus, and acting as the bridge between the user and the account logic.

## How to Run
1. Ensure the Java Development Kit (JDK) is installed on your system.
2. Open your terminal or command prompt.
3. Navigate to the directory containing the source code files.
4. Compile the program using the following command:
   `javac Main.java`
5. Execute the compiled application:
   `java Main`
6. Follow the on-screen prompts to interact with the ATM interface.