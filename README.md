# Store Management System Using Java Swing and Arrays

## System Overview
This project is a multi-frame Store Management System developed as a Java Swing application. It applies structured programming and basic Object-Oriented Programming (OOP) concepts in a GUI environment. The application simulates a checkout system, monitors stock levels, and logs purchase history. A core constraint of this project is that all data storage and manipulation strictly utilize fixed-size arrays; Java Collection Frameworks like `ArrayList` or `Vector` are completely excluded.

## Frame Responsibilities
The system is divided into three separate `JFrame` classes, each handling a distinct part of the application:

* **Store Transaction Frame (Frame 1):**
    * Handles customer purchases and checkout computations.
    * Displays available products (Name, Price) and allows users to select a product and enter a quantity.
    * Computes the subtotal and total cost, then processes the transaction.
    * Prevents negative quantities and transactions that exceed available stock.
    * Reduces inventory quantity and saves transaction details to the logs upon completion.

* **Transaction Logs Frame (Frame 2):**
    * Displays the history of all completed transactions in the order they were processed.
    * Shows the specific product name, quantity purchased, and total price for every entry.
    * Maintains data persistence while the program remains running.

* **Inventory Frame (Frame 3):**
    * Allows viewing and monitoring of the store's current stock.
    * Displays the product name, price, and remaining stock.
    * Automatically updates inventory values immediately after each transaction occurs.

## How Arrays Are Used
To meet project constraints, arrays handle all data storage and are logically passed between the GUI components. 

* **Product & Transaction Processing:** Product names are stored in a `String[]`, prices in a `double[]`, and quantities in an `int[]`. 
* **Transaction Logging:** The logs frame utilizes a `String[]` for transaction product names, an `int[]` for purchased quantities, and a `double[]` for transaction totals. An index counter is used to track the number of processed transactions.
* **Inventory Management:** Inventory quantities are stored in an `int[]`. This array is shared logically with the Store Transaction Frame to evaluate available stock before approving a purchase.

## Project Screenshots
*(Place your images in a designated screenshot folder inside the repository.)*
* [Screenshot of Transaction Frame goes here]
* [Screenshot of Logs Frame goes here]
* [Screenshot of Inventory Frame goes here]

## Live Demo
* [Insert your Google Vids live demo link here]
