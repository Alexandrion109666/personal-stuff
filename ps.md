# DiabClinics Specification

This application helps clinic's staff to perform in a very easy and efficeient way different operations against patient related data.
The application have two types of users that can operate through the application: doctor/nurse and administrator. All of them will have to provide their credentials in order to log in and use the application.
# Elaboration – Iteration 1.1

## Domain Model
For now the domain model may contain the next classes:

![diagram1](data_model.png)

## Architectural Design

### Conceptual Architecture
For this application I will use a 3 layered architecture, that consist of three main layers: presentation/view, business - logic, peristence/dao and common. By segregating an application into modules, developers acquire the option of modifying or adding a specific layer, instead of reworking the entire application. A three-module architecture is typically composed of a presentation module, a business module, and a data storage module.
Therewith, the application is also based on Model–view–controller (MVC), which is an architectural pattern commonly used for developing user interfaces that divides an application into three interconnected parts. This is done to separate internal representations of information from the ways information is presented to and accepted from the user. The MVC design pattern decouples these major components allowing for efficient code reuse and parallel development.

![diagram2](conceptual.jpg)

### Package Design

![diagram3](package.jpg)

### Component and Deployment Diagrams

![diagram4](component.png)

![diagram4](deploy.png)

# Elaboration – Iteration 1.2

## Design Model

### Dynamic Behavior
[Create the interaction diagrams (1 sequence, 1 communication diagrams) for 2 relevant scenarios]

### Class Design
[Create the UML class diagram; apply GoF patterns and motivate your choice]

### Data Model
[Create the data model for the system.]

### Unit Testing
[Present the used testing methods and the associated test case scenarios.]

# Elaboration – Iteration 2

## Architectural Design Refinement
[Refine the architectural design: conceptual architecture, package design (consider package design principles), component and deployment diagrams. Motivate the changes that have been made.]

## Design Model Refinement
[Refine the UML class diagram by applying class design principles and GRASP; motivate your choices. Deliver the updated class diagrams.]

# Construction and Transition

## System Testing
[Describe how you applied integration testing and present the associated test case scenarios.]

## Future improvements
[Present future improvements for the system]

# Bibliography
- [Architectural Styles](https://docs.microsoft.com/en-us/azure/architecture/guide/architecture-styles/)
- [Architectural Patterns and Styles](https://msdn.microsoft.com/en-us/library/ee658117.aspx)
- [Online diagram drawing software](https://yuml.me/) ([Samples](https://yuml.me/diagram/scruffy/class/samples))
- [Yet another online diagram drawing software](https://www.draw.io)
