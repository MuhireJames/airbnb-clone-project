# Airbnb Clone Project  
This  is a project that provide a robust and scalable foundation for managing user interactions, property listings, bookings, and payments.Some of goals are:user management,property management,booking management payments integrations,user reviews and data optimimisation.  
Stack to be used :Django,Django rest framework,GraphQl,PostgreSQL,Docker,Redis and CI/CD pipelines and Celery as payment gateway  

## Team Roles  
**Business Analyst**:Who will be responsible for understanding customer’s business processes and translate customer business needs into requirements  
**Product owner**:who is responsible for holding responsibility for a product vision and evolution and make sure final product meets customer requrement  
**Project Manager**:Makes sure a product or its part is delivered on time and within budget
**UI/UX designer**:Transforms a product vision into user-friendly designs  
**Software Architect**:Designs a high-level software architecture  
**Software Developer**:Responsible for actual job and codes an application,for both frontend features and backend code including database design and Api development  
**Quality assurance (QA) engineer**:Makes sure an application performs according to requirements   
**Test automation engineer**:Designs a test automation ecosystem  
**DevOps Engineer**:Builds continuous integration and continuous delivery (CI/CD) pipelines for faster delivery  

## Technology Stack  
**Django**: A high-level Python web framework used for building the RESTful API.  
**Django REST Framework**: Provides tools for creating and managing RESTful APIs.  
**PostgreSQL**: A powerful relational database used for data storage.  
**GraphQL**: Allows for flexible and efficient querying of data.  
**Celery**: For handling asynchronous tasks such as sending notifications or processing payments.  
**Redis**: Used for caching and session management.  
**Docker**: Containerization tool for consistent development and deployment environments.  
**CI/CD Pipelines**: Automated pipelines for testing and deploying code changes  

## Database Design  
### 1. Users  
#### Purpose  
Stores user credentials and profile information  
##### Fields  
-id  
-username  
-password  
-role    
-created_at 

### 2. Properties    
#### Purpose  
Represents properties that users can list and book  
##### Important fileds  
-id  
-owner_id  
-title  
-description  
-address  
-availability  
-price_per_night  
-created_at  

### 3 .Bookings  
#### Purpose  
Tracks property reservations made by users  
##### Fields  
.id  
.user_id  
.property_id  
.start_date  
.end_date  
.total_price  
.status  
.created_at  

### 4. Payments  
#### Purpose  
Handles transaction records for bookings.  
##### fields  
.id  
.booking_id  
.amount  
.payment_method  
.payment_status  
.transaction_id  
.paid_at    
### 5 .Reviews    
#### Purpose    
Allows users to leave reviews and ratings on properties  
##### Fields  
.id  
.user_id  
.property_id  
.start_date  
.rating   
.comment  
.created_at

## Feature Breakdown  
**User Management feature**:It all about all user management related features like user authentication and authorisation,creating CRUD operation  
**Review feature**:Where users can make review ,edit or delete reviews  
**Payment processing**:Users may make payment of their related bookings they liked  

## API Security  
**User authentication**:where users will be allowed to register and login into our application  
**User authorisation**:Where users will be having access to some routes while other will be restricted like some routes to be accessed by by admin only  
**Rate limiting**: where users will be allowed to do limited api request to our app  

## CI/CD Pipeline 
### Description    
Continuous Integration (CI) and Continuous Deployment (CD) pipelines are essential for modern application development    
## ✅ Key Benefits  
.Faster Development Cycles    
Automates the workflow from code commit to deployment, reducing manual effort and accelerating release timelines. 

.Improved Code Quality  
Automated tests run on every code change, helping catch bugs and regressions early in the development process. 

.Consistent Deployments  
Ensures code is deployed the same way every time, reducing the chance of human error and environment discrepancies. 

.Instant Feedback  
Developers are quickly alerted to issues through failed builds or tests, enabling faster fixes and better collaboration.  

.Better Collaboration  
Teams can merge changes more confidently and frequently, reducing merge conflicts and integration challenges.

.Scalability and Reliability  
As your app grows, CI/CD helps maintain a stable and scalable infrastructure by automating repeatable tasks.  

## 🛠️ Common CI/CD Tools  
*GitHub Actions  
*GitLab CI/CD  
*Jenkins  
*CircleCI  
*Travis CI  


