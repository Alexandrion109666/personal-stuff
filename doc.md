# Analysis and Design Document

# Requirement analysis

## Assignment Specification
Use Java/C# API to design and implement an application for the employees of a book store. The
application should have two types of users (a regular user represented by the book store
employee and an administrator user) which have to provide a username and a password in order
to use the application.

## Function requirements
The regular user can perform the following operations:
- Search books by genre, title, author.
- Sell books.

The administrator can perform the following operations:
- CRUD on books (book information: title, author, genre, quantity, and price).
- CRUD on regular users’ information.
- Generate two types of reports files, one in pdf format and one in csv format, with the
books out of stock.


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

    * Use case: Search books by genre, title, author
    * Level: one of: Summary
    * Primary actor: Store Employee
    * Main success scenario: Store Employee successfully executes these opeartions
    * Extensions: Store Employee will be prompted if some wrong informations were provided

## Use case 3

    * Use case: Sell books
    * Level: one of: Summary
    * Primary actor: Store Employee
    * Main success scenario: Store Employee successfully executes these opeartions
    * Extensions: Store Employee will be prompted if some wrong informations were provided
    
## Use case 4

    * Use case: CRUD on books (book information: title, author, genre, quantity, and price).
    * Level: one of: Summary
    * Primary actor: Administrator
    * Main success scenario: Administrator successfully executes these opeartions
    * Extensions: Administrator will be prompted if some wrong informations were provided
    
    
## Use case 5

    * Use case: CRUD on regular users’ information.
    * Level: one of: Summary
    * Primary actor: Administrator
    * Main success scenario: Administrator successfully executes these opeartions
    * Extensions: Administrator will be prompted if some wrong informations were provided
    
## Use case 6

    * Use case: Generate two types of reports files, with the books out of stock.
    * Level: one of: Summary
    * Primary actor: Administrator
    * Main success scenario: Administrator executes successfully those operations
    * Extensions: Administrator will be prompted if some wrong informations were provided

    
# System Architectural Design

## Architectural Pattern Description
For this book-store application I used a 3 layered architecture, that consist of three main layers: **presentation/view**, **business - logic**, **peristence/dao** and **common**. By segregating an application into modules, developers acquire the option of modifying or adding a specific layer, instead of reworking the entire application. A three-module architecture is typically composed of a presentation module, a business module, and a data storage module.

![layer](images/layers.png)

## Diagrams

# Package
![package](images/modules.png)

# UML Sequence Diagrams
![seq](images/sequence.png)

*Authentication Sequence*

# Class Design

## Design Patterns Description
In software engineering, the singleton pattern is a software design pattern that restricts the instantiation of a class to one object. This is useful when exactly one object is needed to coordinate actions across the system. The concept is sometimes generalized to systems that operate more efficiently when only one object exists, or that restrict the instantiation to a certain number of objects. 

Usage: 
   ```java
  package main;

import org.springframework.context.support.ClassPathXmlApplicationContext;

public class ApplicationContext {

	private static final ClassPathXmlApplicationContext CTX = new ClassPathXmlApplicationContext(
			"classpath*:/bllContextConfiguration.xml");
	public static String employeeCNP;
	public static Long employeeId;

	private ApplicationContext() {
	}

	public static ClassPathXmlApplicationContext getApplicationContext() {
		return CTX;
	}
}

```
## UML Class Diagram
![strategy](images/stpattern.jpg)
# Data Model
![models](images/uml.png)
# Database schema
![db](images/bd.PNG.png)
![dbb](images/db1.png)
# System Testing
As testing technique we used integration test for services. We test the client and bank service. Our test runned with success. 

# Bibliography
- [Strategy Design Pattern](https://en.wikipedia.org/wiki/Singleton_pattern)
- [Drawing Software](http://draw.io)
- [Multitier architecture](https://en.wikipedia.org/wiki/Multitier_architecture)
