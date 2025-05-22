
---

# 🛒 Ecommerce Checkout Automation using Selenium & TestNG

This project is a UI automation test suite written in Java using **Selenium WebDriver** and **TestNG** to test the end-to-end checkout flow of the [SauceDemo](https://www.saucedemo.com/) e-commerce website.

## 📋 Features Tested

The following test scenarios are automated:

1. **Login Test**
   Logs into the website with valid credentials.

2. **Navigate to Inventory Page**
   Ensures the user is directed to the inventory page after login.

3. **Select Product and Add to Cart**
   Selects a product and adds it to the cart.

4. **Open Cart**
   Navigates to the shopping cart.

5. **Proceed to Checkout**
   Initiates the checkout process.

6. **Fill Checkout Details**
   Inputs the first name, last name, and postal code.

7. **Confirm Order**
   Completes the order and verifies the success message.

---

## 🔧 Technologies Used

* **Java**
* **Selenium WebDriver**
* **TestNG**
* **Maven** 
* **ChromeDriver**

---

## 🚀 Getting Started

### ✅ Prerequisites

Make sure you have the following installed:

* Java JDK 8 or higher
* Maven 
* Chrome browser
* ChromeDriver 
* IDE (like IntelliJ IDEA or Eclipse)

### 📂 Project Setup

1. Clone the repository or download the `.java` file.
2. Ensure your system has the correct path set for `chromedriver` or place the driver in your project directory.
3. Import the project into your Java IDE.
4. Add Selenium and TestNG dependencies:

   * For using Maven, add the following to `pom.xml`:

     ```xml
     <dependencies>
         <dependency>
             <groupId>org.seleniumhq.selenium</groupId>
             <artifactId>selenium-java</artifactId>
             <version>4.18.1</version>
         </dependency>
         <dependency>
             <groupId>org.testng</groupId>
             <artifactId>testng</artifactId>
             <version>7.10.1</version>
             <scope>test</scope>
         </dependency>
     </dependencies>
     ```
   * Or download the `.jar` files manually.

### ▶️ Running the Test

* Run the test class `EcommerceCheckoutt.java` using TestNG.
* All steps will execute in sequence from login to order confirmation.

---

## ✅ Sample Output

```
Login Successful!
Navigated to Inventory Page!
Product Added to Cart!
Cart Opened!
Proceeded to Checkout!
Checkout Details Filled!
Order Placed Successfully!
Test Completed! All tests passed! Browser Closed.
```

---

## 🧪 Test Class Structure

```java
@BeforeClass  // Setup browser and WebDriver
@Test         // Each test step (login, add to cart, etc.)
@AfterClass   // Teardown and close browser
```

---

## 📌 Notes

* Website under test: [https://www.saucedemo.com/](https://www.saucedemo.com/)
* Credentials used:

  * **Username:** `standard_user`
  * **Password:** `secret_sauce`
* This is a demo site provided by Sauce Labs for testing and training purposes.

