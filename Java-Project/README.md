# Cafeteria Management, DU
## Overview
The Cafeteria Management, DU, is a Java-based application designed to streamline cafeteria operations at the Science Complex, University of Dhaka.

It provides a secure and efficient platform for teachers, students, admins, and employees to manage cafeteria services.
The system features user authentication, food ordering, purchase tracking, and administrative controls, ensuring a seamless 
experience for both customers and staff. With role-based access, real-time updates, and secure login mechanisms, this system 
enhances efficiency, transparency, and user convenience.

## Tools
- IDE: IntelliJ
- Language: JAVA
- Framework: JavaFX
- Database: MySQL
- Testing: Manual testing for the overall 
system functionality


## Workflow
![image alt](https://github.com/Clear20-22/Java-Project/blob/5ae01b462834a38334f3274799ee52cdaafe6912/Blank%20diagram.png)

## Directory Layout

```
cafe/
│
├── src/                        # Source code
│   ├── main/                   
│      ├── java/
|      |      |── module-info.java            
│      │      |── cafe.management.cafe/
|      |           ├── AdminController.java
│      │           ├── CafeManagement.java       # Main entry point of the application
│      │           ├── cardProduct.java          
|      |           ├── CustomerController.java  
|      |           ├── CustomerOrderHistory.java 
│      │           ├── CustomerSummary.java  
|      |           ├── DatabaseUsers.java        # Database connection logic cardProduct.java 
|      |           ├── EmployeeData.java
│      │           ├── ManagementControl.java
│      │           ├── ProductData.java
│      │           └── SurfaceLayoutContoller.java
|      |           ├── data.java
│      └── resources/          
│          ├── cafe.management/        
│                         ├── cafe/    # JavaFX FXML & CSS files
|                              ├────── cardProduct.fxml
|                              ├────── CustomerLayout.fxml
|                              ├────── LoginPage.fxml
|                              ├────── LoginStyle.css
|                              ├────── mainForm1Design.css
|                              ├────── SurfaceLayout.fxml
|                              ├────── test.fxml
│                         ├── img/              
├── target/
├── lib/                         
├── out/
│     ├──── artifacts
|                  ├───cafe_jar
|                           ├──── cafe.jar
├── .git/
├── .idea/
├── .mvn/
├── javafx-sdk-23.0.1.                      
├── README.md                       
├── pom.xml
├── .gigintore    

```

## Key Features

### For Teachers & Students:
- **Secure Login & Sign-up** – Access the system using a registration ID and password.  
- **View Menu** – Browse available food items with prices.  
- **Order Food** – Add items to the cart and complete purchases.  
- **Purchase History** – View past orders and payments.  
- **Leave Reviews & Ratings** – Provide feedback on food quality.  
- **Profile Management** – Update personal details.  
- **Password Recovery** – Reset password using a predefined codeword.  

### For Admin & Employees:
- **User Management** – Admin can approve new employees and track users.  
- **Inventory Management** – Update product availability and pricing.  
- **Sales Tracking** – Monitor daily and total income.  
- **Order Management** – Process and track customer orders.  
- **Employee Access Control** – Admin approves employee logins to prevent unauthorized access.  

## Additional Features:
- **Sign-out Confirmation** – Ensures secure logout.  
- **"About Us" Page** – Provides details about the cafeteria and its services.  



## Download and Setup Instructions

### **1. Download the ZIP File:**
Download the project ZIP file from the [repository](#).

### **2. Extract the Files:**
Extract the contents of the ZIP file to your preferred directory.

### **3. Environment Setup:**

Ensure that you have **JavaFX** set up in your IDE. You may need to manually configure JavaFX if it is not bundled with your IDE. Refer to the [JavaFX installation guide](https://openjfx.io/) if necessary.

- **For IntelliJ IDEA or Eclipse:**  
    Add the **JavaFX SDK** to your project libraries.
    Set the VM options to include JavaFX modules like:
    ```bash
    --module-path "path-to-javafx-sdk/lib" --add-modules javafx.controls,javafx.fxml
    ```

### **4. Database Setup:**

1. **Modify Database Credentials:**

   - Open the `DatabaseUsers.java` file located in your project folder.
   - Find the following lines and update them with your **MySQL username** and **password**:
   
     ```java
     String jdbcUsername = "root";  // MySQL username
     String jdbcPassword = "root";  // MySQL password
     String jdbcURL = "jdbc:mysql://localhost:3306/cafeteria_db";  // Database URL
     ```

   - Replace `"root"` with your actual MySQL username and password. Example:
   
     ```java
     String jdbcUsername = "your_username";  // MySQL username
     String jdbcPassword = "your_password";  // MySQL password
     String jdbcURL = "jdbc:mysql://localhost:3306/cafeteria_db";  // Database URL
     ```

2. **Save the file** after modifying the credentials.

### **5. Run the Application:**  

To run the application, follow these steps:  

1. Open a terminal or command prompt in the directory where `cafe.jar` is located.  
2. Use the following command to run the application:  

   ```sh
   java --module-path "your_lib_file_directory" --add-modules javafx.controls,javafx.fxml -jar cafe.jar


1. **Run the server** (for chat functionality or backend processes).
2. **Run the Admin and Client sections** of the application as needed.

---

## Troubleshooting

- **Database Connection Error?**  
  Make sure MySQL is running and that the database URL, username, and password are correctly set in the `DatabaseUsers.java` file.

- **JavaFX Issues?**  
  Ensure you have added the JavaFX SDK and set the VM options correctly in your IDE.

---

## License

Feel free to fork, clone, and modify the project. If you encounter any issues, please open an issue on this repository.

---

🚀 **Enjoy using the Cafeteria Management, DU.**


## Authors
- Suraya Jannat Mim (Roll: 17)<br>
- Anisha Tabassum (Roll: 19)<br>
- Jubayer Ahmed Sojib (Roll: 23)<br>
- Tamal Kanti Sarker (Roll: 39)
