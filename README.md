# Project 1 - Employee Reimbursment System (ERS)

## Executive Summary
The Expense Reimbursement System (ERS) will manage the process of reimbursing employees for expenses incurred while on company time. All employees in the company can login and submit requests for reimbursement and view their past tickets and pending requests. Finance managers can log in and view all reimbursement requests and past history for all employees in the company. Finance managers are authorized to approve and deny requests for expense reimbursement. The reimbursement types should have the following options: LODGING, FOOD, TRAVEL


# Tech Stack
 - Java 8
 - Apache Maven
 - PostgreSQL
 - AWS RDS
 - Java Servlets
 - JDBC
 - HTML
 - CSS
 - JavaScript
 - AJAX / Fetch API

# Functional Requirements
 - Domain objects persisted in relational database
 - Database should be in 3NF
 - CRUD functionality for all domain objects
 - All CRUD functionality accessible via RESTful API
 - Functional web UI to consume RESTful API
 - Workflows to complete all user stories
 - Validate all user input
 - Unit test coverage for service-layer classes

The persistence-layer system shall use JDBC to connect to a Postgres database. The API-layer shall utilize Java servlets to expose a public interface. The front-end view shall use HTML/CSS/JavaScript to make an application that can call server-side components in a generally RESTful manner. The middle tier shall follow proper layered architecture, and have reasonable JUnit test coverage of the service layer. Webpages shall be styled to be functional and readable. 

# User Stories
### Requirements:
#### Guest:
 - As a guest, I can register for a new account
 - As a guest, I can log into my account

#### User:
 - As a user, I can submit a request for reimbursement
 - As a user, I can cancel a pending request for reimbursement
 - As a user, I can view my pending and completed past requests for reimbursement
 - As a user, I can edit my pending requests for reimbursement

#### Admin/Finance Manager:
 - As an admin, I can approve expense reimbursements
 - As an admin, I can deny expense reimbursements
 - As an admin, I can filter requests by status

#### Stretch Goals:
 - As an admin, I can change a user's role between admin and user

# UI Help
Due to the schedule of our curriculum, we won't begin discussing JavaScript until the week of the presentation. Your trainer will be providing drop-in JavaScript code you can use to connect your HTML/CSS front-end to your Java backend. You may need to adjust what is provided to fit into your application. Expect this no later than Monday 4/18/2022.

## weDiagrams, Images, Models
The following images are diagrams that go with the skeleton that was produced to guide you. These should be taken as guidance, not as requirement. Your project does not need to conform to what is seen in these images, your project should conform to the functional requirements and user stories laid out above.


**State-chart Diagram (Reimbursement Statuses)** 

![](./imgs/state-chart.jpg)


**Logical Model**

![](./imgs/logical.jpg)

**Physical Model**

![](./imgs/physical.jpg)

**Use Case Diagram**

![](./imgs/use-case.jpg)

**Activity Diagram**

![](./imgs/activity.jpg)


# Milestones
> This file lays out a general timeline that you can follow to gauge your progress on P1. 

> We can break our project down into smaller MVPs in order to make it more manageable. 
> As a first part to project 1, we will build a console-based application (interaction in IntelliJ's console collecting user input) without a front end. 

## By the beginning / middle of Week 3
- Some progress on business logic and console interaction using the Scanner Class
- Implement methods from the P1 Skeleton
  - with some tests passing

## By the end of Week 3 / Beginning of Week 4
- Console user interaction done
- Database persistence done (your console-based application is successfully saving data to a database).

## By the end of Week 4 
- Application is connected to AWS RDS Database and data is persisted
- Back end is complete with Servlets
- Some progress made on html for front end
  - no JavaScript yet, but can have place holders (buttons/tables)

## By the middle of Week 5
- Front end complete
- Application is using JavaScript to make placeholder buttons populate the web page with dynamic data from the back end.

## Due Thursday/Friday of Week 5
- Application is functioning
- Presentation has been practiced


## Misc Notes

* This README should act as the source of truth for this project. If there is any question or ambiguity I will refer to the text in this document as the final arbiter. The skeleton provided should act as a guide to the structure of the application and should assist in getting started. This skeleton contains some of the necessary classes and method signatures and notes on how these classes and methods should work.


* Remember the logical progression of our java applications. We tend to go from the main method, to the API-layer, to the service-layer, to the persistence-layer. There are exceptions to this rule of thumb, but in general it's a good rule to follow, and the skeleton is structured accordingly. 


* Your trainer can only teach you so much -- This project will require you to do a bit of self study (For instance, learning about how enums work. They aren't that scary I promise). Your BEST resource when self studying besides google is each other. This is a great opportunity to figure out how to articulate your problems to others and help others with their own problems.


* When creating your applications, the diagrams above are simply suggestions for best practice... There are easier and harder ways to implement the same thing. For instance: 
    * The reimbursements table in your database only **needs** the 5 required fields found in the AbstractReimbursement Class. Similar story with the users table. Further, the reimbursement status is a separate table in the logical and physical models, but you may opt to simply make status a field in the reimbursement table to skip the addition of the extra table (though it's good practice).
    * The Use Case and Activity diagrams are **not** all of the required functionalities you need, but are good to look at to make sure your application is flowing properly. 


* Let me reiterate - HELP EACH OTHER! Don't spend 3 hours on the same problem when you could talk it out with your peers after ~1 hour of bashing your head against stackoverflow.com. But of course, do your own work and make sure to actually learn or you'll have a bad time during P2. 


## Submission
### Due Date: Thursday 4/28/2022 at 9:00 AM CST
Your project needs to be pushed into the main branch of your P1 repository no later than the due data and time above. Commits after this deadline will not be considered. On the due date there will be a presentation. You will be expected to briefly cover your project, and should be prepared to discuss it with QC.

