# Aplicatie educationala Specification

Proiectul are la baza crearea si implementarea unei aplicatii desktop pentru liceu ce poate fi utilizata de profesori, elevi, parinti si de un administrator.

Profesorii pot efectua urmatoarele operatii:
- sa-si vizualizeze orarul
- sa vada situatia scolara a elevilor sai
- sa acorde note la materia pe care o preda
- sa incheie media la materia respectiva

Elevii pot efectua urmatoarele operatii:
- sa-si vizualizeze orarul
- sa-si vizualizeze notele, mediile si absentele

Parintii pot efectua urmatoarele operatii:
- sa vizualizeze orarul copiilor lor
- sa vizualizeze notele, mediile si absentele copiilor lor

Administratorul poate efectua urmatoarele operatii:
- sa faca CRUD pe profesori, elevi si parinti
- administrarea bazei de date
- mentenanta server

Parintii vor fi notificati prin email cand copiii lor primesc o nota sau absenteaza sau li se incheie media la o materie sau cea semestriala, iar elevul va fi notificat cand primeste o nota sau i se incheie media.

# Elaboration – Iteration 1.1

## Domain Model
![diagram1](data_model.png)

## Architectural Design

### Conceptual Architecture
Model-view-controller (MVC) este un model arhitectural utilizat în ingineria software. Utilizarea cu succes a modelului elimina business logic din considerentele interfe?ei utilizator, rezultând o aplica?ie în care este mai u?or sa modifica?i fie aspectul vizual al aplica?iei, fie regulile de business subiacente, fara a afecta cealalta. În MVC, modelul reprezinta informa?ia (datele) aplica?iei; vizualizarea corespunde elementelor din interfa?a cu utilizatorul, cum ar fi textul, elementele din caseta de selectare ?i a?a mai departe; ?i controlerul gestioneaza comunicarea datelor ?i business logicul utilizate pentru a manipula datele catre ?i de la model. Este comuna împar?irea unei aplica?ii în straturi separate : interfa?a de prezentare / utilizator (UI) (vizualizare), business logic (controler) ?i accesul la date (model).
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
