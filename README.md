# Simple Product Management System in Java

This is a basic Java console application for managing a list of products. It features two user roles: "Founder" and "Losser" (presumably intended to be "User" or similar).

## Features

**Founder:**

* **Login:** Authenticates with a predefined username ("founder") and password ("12").
* **View Posts:** Displays the current list of products with their names/codes, descriptions, and contact numbers.
* **Upload Post:** Allows adding new product listings, including name/code, description, and contact number.
* **Delete Post:** Enables the removal of a product listing by entering its name/code.
* **Exit:** Logs out of the Founder menu.

**Losser (User):**

* **Login:** Authenticates with a predefined username ("loss") and password ("12").
* **View Product:** Displays the current list of products with their details.
* **Search Product:** Allows searching for a product by its name/code.
* **Exit:** Logs out of the Losser (User) menu.

## Getting Started

1.  **Prerequisites:** You need to have Java Development Kit (JDK) installed on your system.
2.  **Download the Code:** Clone or download the provided Java files (`Founder.java`, `Login_Info.java`, `Loss.java`, `Main.java`, `product_Info.java`).
3.  **Compile the Code:** Open a terminal or command prompt, navigate to the directory where you saved the files, and compile the Java files using the following command:

    ```bash
    javac Founder.java Login_Info.java Loss.java Main.java product_Info.java
    ```

4.  **Run the Application:** After successful compilation, run the `Main` class:

    ```bash
    java Main
    ```

    This will start the application, and you will see the main menu.

## How to Use

1.  The application will present you with a menu:
    ```
    1..Founder
    2.Losser
    3.Exit
    Enter Your Choice:
    ```
2.  **Founder Login (Choice 1):**
    * Enter the username: `founder`
    * Enter the password: `12`
    * Upon successful login, you will see the Founder menu:
        ```
        1.View post
        2.Upload post
        3.Delete post
        4.Exit
        Enter Your Choice
        ```
        * **1. View post:** Displays the list of products.
        * **2. Upload post:** Prompts you to enter the number of posts to add and then the details (name/code, description, contact number) for each.
        * **3. Delete post:** Asks for the name/code of the product to remove.
        * **4. Exit:** Returns to the main menu.
3.  **Losser Login (Choice 2):**
    * Enter the username: `loss`
    * Enter the password: `12`
    * Upon successful login, you will see the Losser menu:
        ```
        1.View product
        2.Search product
        3.Exit
        ```
        * **1. View product:** Displays the list of products.
        * **2. Search product:** Prompts you to enter the name/code of the product you are looking for.
        * **3. Exit:** Returns to the main menu.
4.  **Exit (Choice 3):** Closes the application.

## Code Structure

* **`Founder.java`:** Contains the `Founder` class, which handles the Founder's login and functionalities (view, add, delete posts). It inherits from `product_Info`.
* **`Login_Info.java`:** Stores the login credentials for both Founder and Losser.
* **`Loss.java`:** Contains the `Loss` class (intended for regular users), providing login, viewing, and searching functionalities. It also inherits from `product_Info`.
* **`Main.java`:** The entry point of the application. It contains the `main` method that displays the initial menu and handles user choices to access the Founder or Losser sections.
* **`product_Info.java`:** An abstract class that likely holds common functionalities and data structures for product information, such as the `product_list`, `product_dis`, and `contact_n` ArrayLists, and the `view()` method. It also initializes some default product data in the `add()` method.

## Potential Improvements

* **More Robust Input Validation:** Add checks for empty inputs, incorrect data types, etc.
* **Data Persistence:** Currently, the product data is lost when the application closes. Implement a mechanism to save and load data (e.g., using files or a database).
* **User Management:** Allow adding and managing multiple Founder and User accounts instead of hardcoding credentials.
* **Error Handling:** Implement more specific error handling for various scenarios.
* **User Interface:** Consider using a graphical user interface (GUI) instead of a console-based one for a better user experience.
* **Clearer Naming:** Rename the "Losser" role to something more appropriate like "User" or "Customer".
* **More Advanced Search:** Implement more sophisticated search options (e.g., searching by description).
* **Quantity and Pricing:** Add attributes for product quantity and price.



---

##  Author

**Md. Junayed Bin Karim**  
 CSE Student at Daffodil International University  
 [GitHub](https://github.com/Junayed-Bin-Karim)  
 [LinkedIn](https://www.linkedin.com/in/junayed-bin-karim-47b755270/)  
 karim22205101667@diu.edu.bd  


---
