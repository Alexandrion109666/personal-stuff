# DiabClinics Supplementary Specification

# Introduction
This document includes system requirements that were not included in use case model. The requirements are:

- Regulatory requirements, including the standard of application
- The quality attributes of the system to be built, including requirements for use, reliability, performance and sustainability.
- Other requirements, such as operating system and environments, compatibility requirements and design constraints.

# Non-functional Requirements
The system should always be up-to-date, connected to the server and save the information in real-time without losing it. This will be possible using the CRUD by the administrator to modify the database.

## Availability

It will be valid on every computer connected to the Internet.

## Performance

One of the most important non-functional requirements of customers is a system with a good and fast performance rate. Therefore, the performance objective is divided into three sub-objectives: time, space and response. Each request to the server is processed as quickly as possible and the response or error is sent back to the user.

## Security

A user only has access to his or her personal data after successful authentication. A valid password is a string that has at least 8 characters, which contains both uppercase and lowercase letters and a numeric character. It will be safe, the data will be protected in a database, and each user has certain rights that can not be loaded.

## Testability

It can be tested locally at the beginning to see all the problems with this system. I will use JUnit tests and manual and / or automatic testing.

## Usability

It can be used by any individual who has minimal knowledge of using a computer.

# Design Constraints

The project will be implemented in Java, a high-level programming language, along with the Windowbuilder to be used for the graphical interface, and MySql for the baseline where I will retain the information.
The user will access the application, connect with login data, and depending on assigned rights, can do various operations.


# Resources

* http://www.upedu.org/process/gdlines/md_srs.htm
* Example of Supplementary Specification: http://csis.pace.edu/~marchese/SE616_New/Samples/Example%20%20Supplementary%20Specification.htm
