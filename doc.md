# Analysis and Design Document

# Requirement analysis

## Assignment Specification
Use JAVA/C# API to design and implement an application for the front desk employees of a
bank. The application should have two types of users (a regular user represented by the front
desk employee and an administrator user) which have to provide a username and a password in
order to use the application.

## Function requirements
The regular user can perform the following operations:
- Add/update/view client information (name, identity card number, personal numerical
code, address, etc.).
- Create/updatc/delete/view client account (account information: identification number,
type, amount of money, date of creation).
- Transfer money between accounts.
- Process utilities bills.

The administrator user can perform the following operations:
- CRUD on employees information.
- Generate reports for a particular period containing the activities performed by an
employee.


## Non-functional Requirements
   - Security: Authentication mechanism
   - Testable: Modules are easily tested
   - Usability
   - Maintenance
   - Easy way to add new functionalities
# Use-Case Model

## Use case 1

    * Use case: Authentication
    * Level: one of: Administrator/Employee-goal
    * Primary actor: Administrator/Employee
    * Main success scenario: Administrator/Employee is authenticated successfully
    * Extensions: Administrator/Employee will be promped if bad credentials were provided

## Use case 2

    * Use case: Add/update/view client information
    * Level: one of: Summary
    * Primary actor: Bank Employee
    * Main success scenario: Bank Employee successfully executes these opeartions
    * Extensions: Bank Employee will be prompted if some wrong informations were provided

## Use case 3

    * Use case: Add/update/view client account
    * Level: one of: Summary
    * Primary actor: Bank Employee
    * Main success scenario: Bank Employee successfully executes these opeartions
    * Extensions: Bank Employee will be prompted if some wrong informations were provided
    
## Use case 4

    * Use case: Transfer money between accounts
    * Level: one of: Summary
    * Primary actor: Bank Employeet
    * Main success scenario: Bank Employee successfully executes these opeartions
    * Extensions: Bank Employee will be prompted if some wrong informations were provided
    
    
## Use case 5

    * Use case: Pay utilities
    * Level: one of: Summary
    * Primary actor: Bank Employeet
    * Main success scenario: Bank Employee successfully executes these opeartions
    * Extensions: Bank Employee will be prompted if some wrong informations were provided
    
## Use case 6

    * Use case: CRUD on employees
    * Level: one of: Summary
    * Primary actor: Administrator
    * Main success scenario: The administrator executes successfully those operations
    * Extensions: Administrator will be prompted if some wrong informations were provided

## Use case 7

    * Use case: Generate reports between dates
    * Level: one of: Summary
    * Primary actor: Administrator
    * Main success scenario: A digital report is generated
    * Extensions: will be prompted if some wrong informations were provided
    
# System Architectural Design

## Architectural Pattern Description
For this bank application we used a 3 layered architecture, that consist of three main layers: **presentation/view**, **business - logic**, **peristence/dao** and **common**. By segregating an application into modules, developers acquire the option of modifying or adding a specific layer, instead of reworking the entire application. A three-module architecture is typically composed of a presentation module, a business module, and a data storage module.

![layer](layer.png)

## Diagrams

# Package
![package](package.png)

# UML Sequence Diagrams
![seq](sequence.png)

*Authentication Sequence*

# Class Design

## Design Patterns Description
Strategy Pattern is a behavioral software design pattern that enables selecting an algorithm at runtime. We used this pattern to define our error message for every UI fields.
We defined an one-method interface that is implemented by different validation algorithms used for specific fields. So when we validate the form we build error messages based on our validations at runtime. 

Usage: 
   ```java
  private boolean isValid() {
    StringBuilder errorMessages = new StringBuilder();
    List<String> validationMessages = Arrays
        .asList(
            new UsernameFieldValidationMessage().validate(usernameField.getText()),
            new EmailValidationMessage().validate(emailField.getText()),
            new PasswordFieldValidationMessage().validate(passwordField.getText()));
    for (String msg : validationMessages) {
      errorMessages.append(msg);
    }
    if (errorMessages.length() == 0) {
     return true;
    } else {
      Alert alert = new Alert(AlertType.ERROR);
      alert.initOwner(dialogStage);
      alert.setTitle("Invalid Fields");
      alert.setHeaderText("Please correct all the fields.");
      alert.setContentText(errorMessages.toString());
      alert.showAndWait();
      return false;
    }
  }
}
```
## UML Class Diagram
![strategy](strategy.png)
# Data Model
![models](models.PNG)
# Database schema
![db](db.png)
# System Testing
As testing technique we used integration test for services. We test the client and bank service. Our test runned with success. 

# Bibliography
- [Strategy Design Pattern](https://en.wikipedia.org/wiki/Strategy_pattern)
- [Drawing Software](http://draw.io)
- [Multitier architecture](https://en.wikipedia.org/wiki/Multitier_architecture)
