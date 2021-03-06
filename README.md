# CMPE202_FinalProject

  As part of the project we have designed and developed set of Restful APIs for starbucks to manage orders, cards and make payments. Deployable Jar file has been generated and deployed in AWS as a docker image in Amazon container. The application also has EC2 Auto-scaling and load balancer enabled to handle multiple requests simultaneously. 

# Technology Stack

- Spring Boot - For the development of the application with various REST APIs

- Postman - REST API client to test the newly created APIs

- AWS Services 

  - EC2

  - RDS

  - Route53

  - Elastic Load Balancer

  - Autoscaling

  - Amazon Docker
  
- Project Management Tools 

  - Zube - For Sprint tracking and management 
    
  - GitHub - Source code and Project Management 
    
  - Google Sheet - Task tracking and sprint burndown 
    
  - Zoom - Team collaboration (Organizing daily scrum and other meetings)

# Architecture Diagram

![Blank Diagram](https://user-images.githubusercontent.com/42783963/57505041-be592c80-72ab-11e9-9a87-502a0439f389.png)

# Docker Container Depoloyment on AWS ECS
![nowgit](https://user-images.githubusercontent.com/42689991/57551030-d4530580-731c-11e9-9c9e-216fdbf73b06.PNG)

# Use Case Diagram

### Authentication
![Authentication](https://user-images.githubusercontent.com/34608166/57509172-670d8900-72b8-11e9-9ec0-dccbd06c74aa.png)

### Add Card
![addCard](https://user-images.githubusercontent.com/34608166/57507769-8e625700-72b4-11e9-81ba-932c80607538.png)

### Load Balance
![loadBalance](https://user-images.githubusercontent.com/34608166/57507817-b2259d00-72b4-11e9-8922-1ef7e657fc96.png)

### Make Payment
![MakePayment](https://user-images.githubusercontent.com/34608166/57510073-afc64180-72ba-11e9-8d8d-078905521804.png)

### Transaction History
![transactionHistory](https://user-images.githubusercontent.com/34608166/57507742-7be81d80-72b4-11e9-9b03-2ad7250a6935.png)



# Choice of Design Pattern 


### MVC

MVC design pattern helps in separation of the three different objects data model, presentation information and control information concerned with the application. MVC pattern allows multiple developers working on the model, view, and controller at the same time. MVC design pattern also provides a way to switch the views for the application thus providing multiple views for the same application. Modification of any of the component in the MVC pattern does not affect the other component as the three components are not dependent.

  

- Model - Model represents an object or Java POJO carrying data as it consists of all the data associated with the application and defining any manipulation involved in that data. 
  

- View - View represents the visualization of data and is not concerned about the manipulation of data. 
  

- Controller - Controller exists between both View and Model by controlling the data flow into the model object and changing of views whenever there is a change in  the data
# Class Diagram

![Starbucks - Class Diagram](https://user-images.githubusercontent.com/42783963/57561735-7507ec00-7342-11e9-9496-659addfd9c72.png)

---
# Individual Contribution
---

# XP Core Values
### Mukesh Ranjan Sahay - Communication

I have continuously collaborating team to keep the project on track. Below are the tasks under my radar for the core value communication.

- Initiated daily zoom meeting to discuss current tasks and immediate next tasks. 
- Brainstormed the requirement with the team and came up with collaborative ideas. 
- Created and shared private repo for our team with other team members. 


### Thirumalai Nambi Doss - Respect

Appreciating and encouraging every smaller improvements and progress of the project gives the feel of everyone being respected.

- I ensure that everyone’s time and effort is respected even if things wrong.  
- In order to uphold the core value respect, my role is to make sure everyone is equally respected with their new attempts. 
-   I always keep the spirit high even during critical situations.


### Sudha Amarnath - Courage
Holding up the truth about the project is my primary motive to keep up the core value of courage.

- I strongly believe in a team effort and if anything goes wrong we accept the challenge and face them as a team. 
- I make sure there are no false or exaggerated facts about project progress. 

### Muthukumar Sukumaran - Simplicity

My primary role is to keep things as simple as possible to avoid complications in code. 

- I strongly believe that “more code creates more bugs”. 
- To keep things simple I encourage my team to granularize the requirement into smaller user stories 

## StoryBoard


https://zube.io/ms-sjsu/cmpe202_finalproject/w/workspace-1/sprintboard?where%5Bsprint_id%5D=32172

<img width="1678" alt="Sprintboard" src="https://user-images.githubusercontent.com/42783963/57493075-5b01d700-7278-11e9-8bf9-01d69715ccd8.png">


# Journal Sprint - 1

  

### Login API (Mukesh Ranjan Sahay)

What tasks did I work on

- Defined each member’s component 
- Setup the framework for the project 
- Create a Login API for authentication of the application 
  

What I am planning to work on next

- Create a Payment API for the added cards 
  

### Database Setup (Thirumalai Nambi Doss Palani)

What tasks did I work on

- Set up AWS RDS database 
  

What I am planning to work on next

- Create an Add Card API for the authorized users 
  

### Architecture Setup (Sudha Amarnath)

What tasks did I work on

- Identify the components and architecture of the system 
  

What I am planning to work on next

- Host and deploy the Starbucks app to the AWS Auto Scaled EC2 Cluster 
  

### Modeling the Functionality (Muthu Kumar Sukumaran)

What tasks did I work on

- Prepare the use case diagram 
  

What I am planning to work on next

- Create the Manage Orders API to view the list of transactions 
  
## Task Sheet

https://docs.google.com/spreadsheets/d/1OPykANhVQRjI8_Ru5q1IhSUUn3ANxdksqwxk6FdoUwo/edit?ts=5cd0b5e0#gid=0

<img width="1150" alt="Sprint 1" src="https://user-images.githubusercontent.com/42783963/57513061-33cff780-72c2-11e9-83e8-4ba2fb6fe2a2.png">

## Burndown Chart

https://docs.google.com/spreadsheets/d/1OPykANhVQRjI8_Ru5q1IhSUUn3ANxdksqwxk6FdoUwo/edit?ts=5cd0b5e0#gid=500653002

<img width="1150" alt="Burndown 1" src="https://user-images.githubusercontent.com/42783963/57513170-7eea0a80-72c2-11e9-9ad6-c51a8a571f01.png">


# Journal Sprint - 2

  

### Payment API (Mukesh Ranjan Sahay)

What tasks did I work on

- Created a Payment API for the added cards 

What I am planning to work on next

- Create a Docker image of the Starbucks app and host it to AWS 
  

### Add Card API (Thirumalai Nambi Doss Palani)

What tasks did I work on

- Created an Add Card API for the authorized users 
  

What I am planning to work on next

- Prepare the documentation for the application 
  

### Deployment (Sudha Amarnath)

What tasks did I work on

- Hosted and deployed the Starbucks app to the AWS Auto Scaled EC2 Cluster 
  

What I am planning to work on next

- Perform the end to end testing  
  

### Manage Orders API (Muthu Kumar Sukumaran)

What tasks did I work on

- Created the Manage Orders API to view the list of transactions 
  

What I am planning to work on next

- Prepare the class diagram for the application 

## Task Sheet

https://docs.google.com/spreadsheets/d/1OPykANhVQRjI8_Ru5q1IhSUUn3ANxdksqwxk6FdoUwo/edit?ts=5cd0b5e0#gid=148020726

<img width="1150" alt="Sprint 2" src="https://user-images.githubusercontent.com/42783963/57513064-3599bb00-72c2-11e9-8a64-29e078a3c9ac.png">

## Burndown Chart

https://docs.google.com/spreadsheets/d/1OPykANhVQRjI8_Ru5q1IhSUUn3ANxdksqwxk6FdoUwo/edit?ts=5cd0b5e0#gid=452565306

<img width="1150" alt="Burndown 2" src="https://user-images.githubusercontent.com/42783963/57513174-814c6480-72c2-11e9-9afe-411fc2c91c99.png">
  

# Journal Sprint - 3

  

### Dockerizing (Mukesh Ranjan Sahay)

What tasks did I work on

- Created a Docker image of the Starbucks app and host it to AWS 
  

### Documentation (Thirumalai Nambi Doss Palani)

What tasks did I work on

- Prepared the documentation for the application 
  

### Testing (Sudha Amarnath)

What tasks did I work on

- Performed the end to end testing  
  

### Structuring the System (Muthu Kumar Sukumaran)

What tasks did I work on

- Prepare the class diagram for the application

## Task Sheet

https://docs.google.com/spreadsheets/d/1OPykANhVQRjI8_Ru5q1IhSUUn3ANxdksqwxk6FdoUwo/edit?ts=5cd0b5e0#gid=840283743

<img width="1150" alt="Sprint 3" src="https://user-images.githubusercontent.com/42783963/57513067-37fc1500-72c2-11e9-84b2-adb39a724bce.png">

## Burndown Chart

https://docs.google.com/spreadsheets/d/1OPykANhVQRjI8_Ru5q1IhSUUn3ANxdksqwxk6FdoUwo/edit?ts=5cd0b5e0#gid=817197761

<img width="1150" alt="Burndown3" src="https://user-images.githubusercontent.com/42783963/57513183-83162800-72c2-11e9-8cc0-27637259e511.png">
  

# List of APIs 

  

## Authentication API

1. Signup - Register a new user with the specified details of the user 

- URL - /signup 
- HTTP Method: POST 
- Parameters 
    - Email 
    - Password 
    - FirstName 
    - LastName 
    - City 
    - State 

### Sample URL 
```swift
https://msoncloud.com/signup?email=test13@test13.com&first_name=test13&last_name=test13&city=test13city&state=test13state&password=test13](https://msoncloud.com/signup?email=test13@test13.com&first_name=test13&last_name=test13&city=test13city&state=test13state&password=test13) 
```


### Sample Response
```swift

{
    "cust_id": 16,
    "first_name": "test13",
    "last_name": "test13",
    "email": "test13@test13.com",
    "city": "test13city",
    "state": "test13state",
    "password": "test13"
}
``` 

<img width="1178" alt="User Signup" src="https://user-images.githubusercontent.com/42783963/57511087-3d0a9580-72bd-11e9-98ed-0c60ab41b67b.png">
 

2. Login - Login to the account of the user by validating the user details 

- URL - /login 
- HTTP Method: POST 
- Parameters 
    - Email 
    - Password 

### Sample URL 
```swift
https://msoncloud.com/login?email=test13@test13.com&password=test13
```
### Sample Response 
```swift
{
    "cust_id": 16,
    "first_name": "test13",
    "last_name": "test13",
    "email": "test13@test13.com",
    "city": "test13city",
    "state": "test13state",
    "password": "test13"
}
```

<img width="1178" alt="User Login" src="https://user-images.githubusercontent.com/42783963/57511121-57447380-72bd-11e9-8425-c38acdbb1a72.png">

## Add Card API 

Add a new Card with Card details like Card ID and Card Code to the specified Customer. The Initial Balance of the card is assigned through this API.

  

- URL - /addcard 
- HTTP Method: POST 
- Parameters 
    - Customer ID 
    - Card ID 
    - Card Code 
    - Balance 

### Sample URL
```swift
https://msoncloud.com/addcard?cust_id=10&card_id=123458217&card_code=123&balance=50
```

### Sample Response 
```swift
{
    "cust_id": 10,
    "card_id": 123458217,
    "card_code": 123,
    "balance": 50,
    "_id": 19
}
```

<img width="1178" alt="Add New Card" src="https://user-images.githubusercontent.com/42783963/57511127-61ff0880-72bd-11e9-8260-da8d7959d8dc.png">


## Payments API 

The Payments API is used to make a payment with the specified amount which will be deducted from the initial balance of the card when it was added to the user.

- URL - /makepayment 
- HTTP Method: POST 
- Parameters 
    - Customer ID 
    - Card ID 
    - Card Code 
    - Balance 

### Sample URL
```swift
https://msoncloud.com/makepayment?cust_id=10&card_id=123456783&card_code=123&balance=20
```
### Sample Response
```swift
{
    "cust_id": 10,
    "card_id": 123456783,
    "card_code": 123,
    "balance": 170,
    "_id": 0
}
```

<img width="1178" alt="Make Payment" src="https://user-images.githubusercontent.com/42783963/57511156-7511d880-72bd-11e9-9ae9-0fb79b229ea3.png">


### Sample response from Docker container deployed in AWS ECS
```swift
http://www.sudhaaws.com/makepayment?cust_id=10&card_id=123456783&card_code=123&balance=20
```
![8](https://user-images.githubusercontent.com/42689991/57515435-81029800-72c7-11e9-8176-b150125fe433.PNG)


## Manage Orders API 

The Manage orders API is used to list the history of transactions carried out by the user. It also lists the transactions of all cards added under the user’s account. The Response consists of the Transaction ID, Transaction time and the amount paid at the time of payment.

- URL - /history 
- HTTP Method: GET 
- Parameters 
    - Customer ID 
    - Card ID 
    - Card Code 
    - Balance 

### Sample URL 
```swift
https://msoncloud.com/history?cust_id=10
```
### Sample Response 
```swift
[
    {
        "TRANSACTION_ID": 7,
        "CUST_ID": 10,
        "CARD_ID": 123456783,
        "TRANSACTION_TIME": "2019-05-10T05:04:46.000+0000",
        "PAYMENT_AMOUNT": 20
    },
    {
        "TRANSACTION_ID": 8,
        "CUST_ID": 10,
        "CARD_ID": 123456783,
        "TRANSACTION_TIME": "2019-05-10T06:30:42.000+0000",
        "PAYMENT_AMOUNT": 20
    },
    {
        "TRANSACTION_ID": 9,
        "CUST_ID": 10,
        "CARD_ID": 123456783,
        "TRANSACTION_TIME": "2019-05-10T06:31:02.000+0000",
        "PAYMENT_AMOUNT": 20
    },
    {
        "TRANSACTION_ID": 10,
        "CUST_ID": 10,
        "CARD_ID": 189327583,
        "TRANSACTION_TIME": "2019-05-10T06:38:37.000+0000",
        "PAYMENT_AMOUNT": 25
    },
    {
        "TRANSACTION_ID": 11,
        "CUST_ID": 10,
        "CARD_ID": 123456783,
        "TRANSACTION_TIME": "2019-05-10T07:45:02.000+0000",
        "PAYMENT_AMOUNT": 20
    }
]
```

<img width="1178" alt="Manage Orders" src="https://user-images.githubusercontent.com/42783963/57511178-865ae500-72bd-11e9-881c-6662ade9a3ee.png">


## Add Balance API 

The Add Balance API is used to add an additional amount (reloading) to the already added card.

- URL - /addbalance 
- HTTP Method: POST 
- Parameters 
    - Customer ID 
    - Card ID 
    - Card Code 
    - Balance 

### Sample URL
```swift
https://msoncloud.com/addbalance?cust_id=10&card_id=123456783&card_code=123&balance=50
```
### Sample Response
```swift
{
    "cust_id": 10,
    "card_id": 123456783,
    "card_code": 123,
    "balance": 220,
    "_id": 0
}
```

<img width="1178" alt="Add Balance" src="https://user-images.githubusercontent.com/42783963/57511200-91ae1080-72bd-11e9-8236-baaa0593f71c.png">


### Sample URL
```swift
http://www.sudhaaws.com/addbalance?cust_id=10&card_id=123456783&card_code=123&balance=50
```
### Sample response from Docker container deployed in AWS ECS
![9](https://user-images.githubusercontent.com/42689991/57515836-6381fe00-72c8-11e9-945b-95c6a0b3f35f.PNG)



## Rest Assured Test Case Run Results 
![10](https://user-images.githubusercontent.com/42689991/57559112-34ee3c80-7335-11e9-93b5-1df90ef8d2b8.PNG)



## Docker Cluster in AWS ECS
![3](https://user-images.githubusercontent.com/42689991/57514720-ed7c9780-72c5-11e9-9ae1-f93409749b72.PNG)

## Successful SNS notification for Docker Container deployment
![4](https://user-images.githubusercontent.com/42689991/57514713-ece40100-72c5-11e9-952f-b8efc43ef924.PNG)

## Docker Repository in AWS ECS
![5](https://user-images.githubusercontent.com/42689991/57514715-ece40100-72c5-11e9-99b7-7486c8313397.PNG)

## Task Definitions
![6](https://user-images.githubusercontent.com/42689991/57514717-ece40100-72c5-11e9-8304-1a1a2ae4b48e.PNG)

## Docker container build from project jar file and push to AWS repository
![7](https://user-images.githubusercontent.com/42689991/57514718-ece40100-72c5-11e9-9eb6-dfde583696b9.PNG)

## Team's Velocity

<img width="1679" alt="Velocity" src="https://user-images.githubusercontent.com/42783963/57561828-0c6d3f00-7343-11e9-80eb-3a6eb1b59c47.png">
