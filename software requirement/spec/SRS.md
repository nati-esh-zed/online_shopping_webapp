# Online Shopping Web-app Software Requirement Specification

<div style="text-align: center">
<img src="./media/astu-logo.png" height="200px" alt="ASTU Logo"></img>
<!-- <img src="https://raw.githubusercontent.com/nati8333/online_shopping_webapp/main/software%20requirement/spec/media/astu-logo.png" height="200px" alt="ASTU Logo" style="float: center"></img> -->
</div>
<!-- ![astu-logo](https://raw.githubusercontent.com/nati8333/online_shopping_webapp/main/software%20requirement/spec/media/astu-logo.png) -->
<h1>Adama Science and Technology University</h1>

|                        |                                                     |
| ---------------------- | ----------------------------------------------------|
| School                 | **Electrical Engineering and Computing**            |
| School                 | **School of Electrical Engineering and Computing**  |
| Department             | **Computer Science and Engineering**                |
| Course                 | **Fundamentals of Software Engineering (CSEg3201)** |
| Semester Project Title | **Online Shopping Web-app**                         |
| Academic Year          | **2023/2024 G.C**                                   |
| Semester               | **1**                                               |
| Section                | **3**                                               |

| GROUP MEMBER   | ID           |
| -------------- | ------------ |
| Natnael Eshetu | A/UR5111/09  |
| Dawit Ashenafi | UGR/25404/14 |
| Abdi Dawud     | UGR/25390/14 |
| Sumeya Awel    | UGR/26377/14 |
| Eden Wekele    | UGR/25834/14 |

## Table of Contents

- [Online Shopping Web-app Software Requirement Specification](#online-shopping-web-app-software-requirement-specification)
- [Acknowledgement](#acknowledgment)
- [Definitions](#definitions)
- [Acronyms and Abbreviations](#acronyms-and-abbreviations)
- [Chapter 1](#chapter-1)
  - [1.1 Introduction](#11-introduction)
  - [1.2 Background of the Project](#12-background-of-the-project)
  - [1.4 Justification of the Project](#14-justification-of-the-project)
  - [1.5 Objective of the Project](#15-objective-of-the-project)
    - [1.5.1 General Objectives](#151-general-objectives)
    - [1.5.2 Specific Objectives](#152-specific-objectives)
  - [1.6 Scope and Limitations](#16-scope-and-limitations)
    - [1.6.1 Scope of the Project](#161-scope-of-the-project)
    - [1.6.2 Limitations of the Project](#162-limitations-of-the-project)
  - [1.7 Feasibility Study](#17-feasibility-study)
    - [1.7.1 Technical Feasibility](#171-technical-feasibility)
    - [1.7.2 Operational Feasibility](#172-operational-feasibility)
    - [1.7.3 Economic Feasibility](#173-economic-feasibility)
  - [1.8 Significance of the Project](#18-significance-of-the-project)
  - [1.9 Beneficiaries of the Project](#19-beneficiaries-of-the-project)
  - [1.10 Methodology](#110-methodology)
    - [1.10.1 Requirement Elicitation Methods](#1101-requirement-elicitation-methods)
    - [1.10.2 Software Development Method](#1102-software-development-method)
  - [1.11 Development Tools](#111-development-tools)
    - [1.11.1 Hardware Tools](#1111-hardware-tools)
    - [1.11.2 Software Tools](#1112-software-tools)
- [Chapter 2 | Description of Existing Systems](#chapter-2--description-of-existing-systems)
  - [2.1 Major Functionality of Existing Systems](#21-major-functionality-of-existing-systems)
  - [2.2 Users of the Existing Systems](#22-users-of-the-existing-systems)
  - [2.3 Drawbacks of the Existing Systems](#23-drawbacks-of-the-existing-systems)
- [Chapter 3 | Proposed System](#chapter-3--proposed-system)
  - [3.1 Overview](#31-overview)
  - [3.2 Business Rule](#32-business-rule)
  - [3.3 Functional Requirements](#33-functional-requirements)
    - [3.3.1 Users and User Accounts](#331-users-and-user-accounts)
    - [3.3.2 Payment](#332-payment)
    - [3.3.3 Item Exchange](#333-item-exchange)
  - [3.4 Non-functional Requirements](#34-non-functional-requirements)
    - [3.4.1 Operational Requirements](#341-operational-requirements)
    - [3.4.2 Legal Requirements](#342-legal-requirements)
    - [3.4.3 User Interface](#343-user-interface)
    - [3.4.4 Performance Considerations](#344-performance-considerations)
    - [3.4.5 Reliability](#345-reliability)
    - [3.4.6 Error Handling](#346-error-handling)
    - [3.4.7 Security](#347-security)
  - [3.5 System Model](#35-system-model)
    - [3.5.1 Scenarios](#351-scenarios)
    - [3.5.2 Use Case Diagram](#352-use-case-diagram)
    - [3.5.3 Sequence Diagram](#353-sequence-diagram)
    - [3.5.4 Collaboration Diagram](#354-collaboration-diagram)
- [Chapter 4 | System Design](#chapter-4--system-design)
  - [4.1 Overview](#41-overview)
  - [4.2 System Architecture](#42-system-architecture)
    - [4.2.1 Subsystem Decomposition](#421-subsystem-decomposition)
    - [4.2.2 Hardware and Software Mapping](#422-hardware-and-software-mapping)
    - [4.2.3 Component Diagram](#423-component-diagram)
    - [4.2.4 Persistent Data Management](#424-persistent-data-management)
    - [4.2.5 Database Design](#425-database-design)
    - [4.2.5.1 Entity Relationship Diagram](#4251-entity-relationship-diagram)
    - [4.2.6 Access Control](#426-access-control)
  - [4.3 User Interface Design](#43-user-interface-design)
- [Chapter 5 | Implementation](#chapter-5--implementation)
  - [5.1 Overview](#51-overview)
  - [5.2 Coding Standard](#52-coding-standard)
  - [5.3 Development Tools](#53-development-tools)
  - [5.4 Prototype](#54-prototype)
  - [5.5 Implementation Detail](#55-implementation-detail)
- [Chapter 6 | Testing](#chapter-6--testing)
  - [6.1 Introduction](#61-introduction)
  - [6.2 Scope](#62-scope)
  - [6.3 Resources](#63-resources)
  - [6.4 Schedule](#64-schedule)
  - [6.5 Test Case Scenario](#65-test-case-scenario)
  - [6.6 Pass Fail Criteria](#66-pass-fail-criteria)
  - [6.7 Approach](#67-approach)
  - [6.8 Test Case Specification](#68-test-case-specification)
  - [6.9 Estimated Risk and Contingency Plan](#69-estimated-risk-and-contingency-plan)
- [Chapter 7 | User Manual and Demo](#chapter-7--user-manual-and-demo)
  - [7.1 User Manual](#71-user-manual)
  - [7.2 Demo](#72-demo)
- [References](#references)

## Acknowledgment

First of all thank God for everything. And thanks to our FSE teacher Mr. Megersa Daraje for giving us this opportunity to do this project and for teaching and guiding us on how to do this project. Thanks to Alemu Tadesse for advising us and giving us feedback on the UML diagrams.

## Definitions

- [MySQL](https://www.mysql.com/)
  > MySQL is a popular open source database management system that offers various features, tools, and services  for data warehousing, analytics, machine learning, and more.
- [Node.js](https://nodejs.org)
  > Node.js® is an open-source and cross-platform JavaScript runtime environment that executes JavaScript code outside of a web browser 1. Node.js is widely used for developing web applications, APIs, microservices, and more.
- [Hapi.js](https://hapi.dev/)
  > hapi.js is an open-source and secure framework for developing web services and applications with Node.js. hapi.js offers a simple, modular, and extensible architecture that allows you to focus on your business logic and not on the details of the tool. hapi.js also provides a rich ecosystem of official plugins and third-party modules that cover various features and functionalities, such as authentication, validation, caching, logging, and more.
- [React.js](https://react.dev/)
  > React.js is an open-source and cross-platform JavaScript library for building user interfaces and single-page applications. React.js uses a component-based approach to create reusable and interactive UI elements. React.js also supports features such as hooks, state management, routing, and more.
- Router on the backend server
  > A router in this context means the part of the server that directs URL requests to specific resources.

## Acronyms and Abbreviations

| ACRONYM OR ABBREVIATION | DESCRIPTION                          |
| ----------------------- | ------------------------------------ |
| FSE                     | Fundamentals of Software Engineering |
| SRS                     | Software Requirements Specification  |
| API                     | Application Programming Interface    |
| PHP                     | Hypertext Preprocessor               |
| UI                      | User Interface                       |
| DBMS                    | Database Management System           |
| ERD                     | Entity Relationship Diagram          |
| MVC                     | Model View Controller                |

## Chapter 1

### 1.1 Introduction

We live in the modern age of computer technology. Even though the act of purchasing and online shopping does not have a long track record, it is the fastest growing and dominating business model and technology area. Companies like Amazon, Alibaba, eBay, and Walmart currently dominate the market. However, online shopping is not very common in our country, and we can understand the potential of this business in our country's case. It is significant to develop a proper system that could resolve the current online shopping drawbacks.

The main geographical target of this project is our beloved country Ethiopia. We aim to design and implement a reliable online shopping system for local use here in Ethiopia.

### 1.2 Background of the Project

Online shopping is a form of electronic commerce that allows consumers to buy goods or services from sellers over the Internet using a web browser or a mobile app. Online shopping has become a popular and convenient way of shopping for millions of people around the world, especially with the development of various online platforms, payment methods, and delivery services. However, online shopping did not emerge overnight; it has a history that dates to the late 1970s.

The growth of online shopping was further boosted by the invention of the World Wide Web in 1990 by Tim Berners-Lee, who also created the first web browser. The World Wide Web made it possible for users to access information and resources from different servers and locations. In 1994, Netscape developed a security protocol called SSL (Secure Sockets Layer) that encrypted the data exchanged between web browsers and web servers, making online transactions more secure and reliable. In the same year, the first online marketplaces, such as Amazon.com and eBay, were launched, offering a wide range of products and services to online shoppers. Since then, online shopping has evolved and expanded to include various features, such as comparison shopping, social commerce, mobile commerce, and more.

Online shopping is still in its early stages in Ethiopia, but it is growing rapidly. The COVID-19 pandemic has accelerated the adoption of digital technologies, and the Ethiopian government is taking steps to support the development of e-commerce. A regulation called 'Electronic Transaction' that provides a legal framework for Electronic Commerce (E-commerce) and other related aspects including e-receipts is in the final approval process. The long-awaited Payment instrument Issuers directives that were expected to open the mobile money and fintech space for non-banks and MFIs are issued now. Ethio Telecom or any other local Fin-tech start-ups and companies can operate legally. This will definitively add to the dynamics of the Fintech landscape and hopefully provide more and better avenues for people to buy online.

There are a few e-commerce websites and apps in Ethiopia that are worth exploring. Shega is a website that provides a list of e-commerce websites and apps in Ethiopia. Addis Mercato is an online marketplace that offers a wide range of products from supermarkets and stores in town.

### 1.3 Statement of the Problem

The main issues of online shopping in Ethiopia are accountability and legal processes, security, delivery, and a money back guarantee on failure or conflict. The proposed software solution aims to solve these issues.

- **Accountability and legal processes:**
Accountability should be taken for handling items and money with proper legal processes prepared to handle all cases. Customers and vendors would like to have the legal processes handled by the company with less of their involvement. Also, the company should ensure that vendors comply with local laws and regulations.
- **Security issues:**
Some vendors might try to scam customers and create multiple accounts. The company should verify vendors' and customers' existence to avoid scams.The system must be designed to protect unauthorized identity information access and must keep backups.
- **Delivery issues:**
Accidents or conflicts might arise during delivery of items. The company ought to have a system in place to handle this.As for thefts during delivery the deliverer ought to be accountable.
- **Money Back Guarantee on Failure or Conflict:**
Local payment methods such as CBE Birr, Amole, Tele birr, and M-Birr do not provide an API for a 2-phase payment system in which paid money is reserved until completion of item transaction either in success or failure. Customers would like to have the guarantee of their money being returned back safely, and without bureaucracy, to them on failure.
- **Internet Issues:**
Internet requirement is unavoidable but the system might be overloaded with command and fetch requests. The more resource files need to be transferred the more load the system will take thus the slower the service.

### 1.4 Justification of the Project

It is best to make this project as no local system provides a solution for all  the issues mentioned in the problem statement and the ones that do are not local and do not support local payment or delivery.

### 1.5 Objective of the Project

#### 1.5.1 General Objectives

Generally, our objective is to create a desirable, competent, secure, and reliable local online shopping software system for use in Ethiopia.

#### 1.5.2 Specific Objectives

Our specific objectives are:

- To create a functional online shopping system within the given time-frame.
- To incrementally and iteratively design and build the system.
- To simultaneously work on this project for maximum efficiency.
- To continuously, analyze and improve requirements and this specification document.
- To analyze, design, and implement features prioritized based on importance.

### 1.6 Scope and Limitations

#### 1.6.1 Scope of the Project

In this project, we only focus on developing a country-local system.

#### 1.6.2 Limitations of the Project

These are the limitations of this project:

- The software system will not work internationally.
- Internet access and a modern browser is required.
- Less than one month to finish this project.

### 1.7 Feasibility Study

#### 1.7.1 Technical Feasibility

It is possible to do this project using the modern softwares and tools available to us at this time. We have access to personal computers, great coding and editing softwares, good internet access, a lot of frameworks, libraries and resources for web development.

#### 1.7.2 Operational Feasibility

Node.js is best for this project as it is the latest web-technology and provides a variety of good well-maintained libraries and development tools.

This project can be deployed on a node.js server or on a virtual system server. And it should have a much better performance than the usual PHP server.

Thus it is possible to deploy and maintain this project using the technologies currently available to us.

#### 1.7.3 Economic Feasibility

This project requires an owning company to operate and maintain it. It requires legal action and accountability, software maintenance and upgrade. Thus it requires employees. It is possible to make this project operational and actively available to users if investors are willing to invest the required amount of funds to create and maintain the company.

### 1.8 Significance of the Project

This project is significant because:

- It makes it easier to find the items we want to buy and their details using modern technology.
- It will be trustworthy and involves the least legal processes and worries to customers.
- It will be most demanded in large cities such as Addis Abeba.

### 1.9 Beneficiaries of the Project

The beneficiaries of this project are:

- Stakeholders who invest in this project.
- Vendors who want to keep track of their inventory and sell online.
- Customers who want to purchase online and have items delivered.
- Employees, such as Managers and couriers.

### 1.10 Methodology

#### 1.10.1 Requirement Elicitation Methods

We used interview, online research, and group discussion methods to gather and form software requirements for this project. We have viewed and analyzed some of the local and international most used online shopping websites like Amazon and Tolo Mart. We have also done some research on the proclamations regarding trading and national payment systems in Ethiopia.

#### 1.10.2 Software Development Method

We use Agile model which has an incremental and iterative approach to software development. We aim to develop the system within a very short amount of time with as much features implemented as possible. We use modern version control tools like git and Github to aid us in collaboration and in incremental and iterative software development.

### 1.11 Development Tools

#### 1.11.1 Hardware Tools

- Personal Computers: Laptops.
- Peripherals: Wireless Mouse
- Smart Phones: For communication and file sharing.

#### 1.11.2 Software Tools

- WPS Office: for editing word documents.
- VSCode: for coding and general text editing.
- [CloudConvert](https://cloudconvert.com) for converting markdown files to docx and pdf.
- Draw.io: for designing modeling diagrams.
- MySQL Workbench: for managing database and designing ERD.
- Microsoft Edge, Google Chrome: for testing and debugging webapp, and browsing the web for resources.

## Chapter 2 | Description of Existing Systems

Some of the existing online shopping websites are [Mekina](https://www.mekina.net/), [MGebeya](https://www.megebeya.com/), [ToloMart](https://www.tolomart.com/), [DeliverAddis](https://deliveraddis.com/), [AddisMercato](https://addismercato.com/).

### 2.1 Major Functionality of Existing Systems

- **Browsing and search:**
It is easy to find items using search queries and filter categories such as brand, price, etc...

- **Ordering and payment:**
All existing systems provide order management but only some provide internet payment systems.

- **Account management:**
All provide account profile creation and management.

- **Delivery:**
Some provide delivery services of products/items with some supporting pay-on-deliver.

- **Additional features:**
Most provide product/item reviews and ratings from other customers. Some provide customer support such as hot-lines.

### 2.2 Users of the Existing Systems

The existing systems provide services for local customers in Ethiopia. Most of the customers that use them are located in Addis Abeba or similar large cities in the country.

### 2.3 Drawbacks of the Existing Systems

Some only provide shopping of specific categories of products/items such as cars or food. Some do not provide internet payment methods. Most do not provide money-back-guarantee.

## Chapter 3 | Proposed System

The proposed system for the project is described in Chapter 3 of this Communication. The first step is to define business rules, followed by describing functional requirements such as users and user accounts, payment and item exchange. The chapter then goes on to investigate the non functional requirements, which include operational, legal, user interface, performance, reliability, error handling and security.In order to provide a comprehensive overview of the proposed system, the system model is also presented, including scenarios, use case diagrams, entity relationships diagrams, sequence diagrams, activity diagrams, and state diagrams.

### 3.1 Overview

The proposed system for the project is described in this chapter of this Communication. The first step is to define business rules, followed by describing functional requirements such as users and user accounts, payment and item exchange. The chapter then goes on to investigate the non functional requirements, which include operational, legal, user interface, performance, reliability, error handling and security.In order to provide a comprehensive overview of the proposed system, the system model is also presented, including scenarios, use case diagrams, entity relationships diagrams, sequence diagrams, activity diagrams, and state diagrams.

### 3.2 Business Rule

These proclamations are considered for the design and working of this system.  
[Ethiopia Commodity Exchange Proclamation No. 550/2007](https://faolex.fao.org/docs/pdf/eth95240.pdf)  
[National Payment System(Amendment) Proclamation No. 1282/2023](https://nbe.gov.et/wp-content/uploads/2023/04/National-Payment-SystemAmendement-Proclamation-No.1282-2023.pdf)  

> **Proclamation No. 550/2007 Article 25**  
> **1/** The Exchange shall clear and settle all transactions on the Exchange either clearing internally with affiliated, recognized Clearing Institutions or through third-party Clearing Institutions, in accordance with the directives of the Authority.  
> **2/** Members shall maintain accounts with any of the affiliated recognized Exchange Clearing Institutions, in accordance with the Exchange by-laws.  
> **3/** Members shall grant written notice of Power of Attorney to the Exchange authorizing the Exchange to issue debit and credit instructions to affiliated recognized Exchange Clearing Institutions, for the purposes of clearing and settlement, in accordance with Exchange bylaws.  
> **4/** The Exchange shall reconcile daily each Member’s trading position on trading days.  
> **5/** The Exchange shall generate a written and electronic daily net obligation statement for each Member on trading days.  
> **6/** The Exchange shall, on the basis of the net obligation statement, instruct the affiliated recognized Clearing Institutions to settle the obligations of the Members.  
> **7/** The Exchange and Members shall be allowed to give standing written instructions to affiliated recognized Clearing Institutions to authorize such institutions to transfer funds to and from Member and Exchange Accounts established in these same institutions for the purposes of Exchange transactions, on the basis of an electronic instruction.  
> **8/** Notwithstanding provisions of any law, regulation, directive or customary practice that requires a signature be handwritten in order to have legal effect or enforceability, signature requirement under Sub-Article (7) of this Article is met if an electronic signature is used to authorize fund  transfers.  
> **9/** Any Clearing Institution shall not engage in trading activity within or outside the exchange.  

> **Proclamation No. 550/2007 Article 29**  
> The Exchange shall provide and maintain a system for protection of personal, financial, trade and other data relating to the affairs of the Exchange.  

> **Proclamation No. 1282/2023 Article 6**  
> **1/** Application for license to be a payment instrument issuer or payment system operator shall be submitted to the National Bank.  
> **3/** A business organization other than financial institution and government owned enterprise intending to be licensed as a payment instrument issuer or a payment system operator shall establish a subsidiary exclusively for the purpose.  
> **6/** An applicant for payment instrument issuer and payment system operator shall fulfill minimum paid up capital as may be prescribed by the National Bank directive.  

The company that owns and operates this system must hire lawyers to handle all legal cases.  
The company must operate in accordance to these laws.

### 3.3 Functional Requirements

#### 3.3.1 Users and User Accounts

- User account creation, session management and administration.
- There are customer, vendor, administrator, employees which include manager, lawyer and courier.

##### Vendors

- Vendors must be able to register items in stock given the required information
  such as brand, name, price and quantity.
- Vendors must be able to view and modify items registered in their stock.
- Vendors must be able to search and filter using some criteria such as brand, price range and area
  from their own stock and other's stock to checkout the competition.

##### Customers

- Customers must be able to search and filter using some criteria such as brand, price range and area
  from registered items and then must be able to select items and put them in a cart.
- Customers must be able to view and modify the items in their cart. Which are
  - View the items in a list
  - View the total price
  - Remove items from the list
  - Increase or decrease the quantity of items
- Customers must be able to pay through supported e-payment systems with ease.
- Customers must be able to view and keep track of, and cancel their orders.
  Status, notifications, location, delivery time should be considered.

##### Employees

###### Administrator

- There must be one administrator account.
- Administrator must be able to:
  - View and manage employees.
  - Registration and removal of employees.
  - Setting the salaries of the employees.
  - Backing up data.

###### Managers

- Managers must be able to hire and manage couriers. Management includes:
  - Hiring and firing couriers.
  - Assigning delivery tasks to couriers.
  - Handling failing delivery cases and conflicts.
  - Consulting and assigning lawyers to cases that require legal action.

###### Lawyers

- Layers handle all legal issues for the company.

###### Couriers

- Couriers handle safe and fast delivery of items.
- Couriers must be able to:
  - View and accept or reject delivery tasks.
  - Contact their manager, the vendor and the customer through safe and secure means.
  - Complete delivery tasks.

#### 3.3.2 Payment

- Payment should be done though a common API and with available e-payment systems.
- Customers, vendors and employees should have a checking account that supports e-payment
  and it must be registered in the system.
- When customers pay for a purchase the money must be temporarily put in a common
  'customers-holding' checking account until successful or unsuccessful delivery of items
  from vendor to customer through a courier.
  - Upon successful delivery the money must be transferred to the corresponding vendors'
    registered checking account with deducted fees.
  - Upon unsuccessful delivery the money must be transferred back to the customer's registered
    checking account.
- Deducted fees include tax, service fees, delivery costs and transaction costs.

#### 3.3.3 Item Exchange

- Item exchange may occur from vendor to courier, courier to customer, courier to manager,
  manager to courier and courier to vendor.
- The must be a form provided for item exchange. That form must include:
  - List of items to be exchanged with important information such as quantity and expected condition.
  - A checkbox for each item to signify acceptance or rejection of the item.
    The checkbox must either be marked or crossed.
  - A reason-for-rejection form items presented.
    Such reasons include items presented in an unexpected condition (not as advertised or damaged).
  - A submit button or a signature box if it is paper form.
- No one should accept items presented in an unexpected condition as they will take responsibility.
- The person who has items in their possession takes responsibility for the safety of those items.
  And the company is responsible for providing and handling a trust worthy and reliable courier
  and handles all legal issues regarding safe item delivery and accidents or scams.

### 3.4 Non-functional Requirements

#### 3.4.1 Operational Requirements

- A web-application is preferred as it is platform independent and internet is unavoidable.
- A web-server must be selected and setup to handle at least 10,000 customers for starter.
- Web server capabilities should be scaled up to meet increasing demand.
- A frontend library should be used to generate a single page web-application and generate
  the view components dynamically by fetching the required information from the backend web-server.

#### 3.4.2 Legal Requirements

- The company must have legally registered and verified business document in the
  country/area where it operates.
- An End User License Agreement(EULA) must be properly written and provided for end users.
  Consider consulting lawyer.
- Lawyers must be hired for consulting and to handle cases requiring legal action.

#### 3.4.3 User Interface

- The UI must be clear and easy to use.
- The UI must display errors properly without abruptly getting out of page and provide solutions if available.
- The UI must adapt to changing screen sizes. It must provide a responsive layout for different screen sizes.
- The UI should have sooth transition between states in order to provide a good user experience.

#### 3.4.4 Performance Considerations

The system has to be able to handle many requests as fast as possible. This means less data transfer balanced with less processing time. Rather than use a backend page generator like PHP to generate dynamic pages it might be best to generate the page on the frontend using libraries such as React.js and get the necessary data from the server using requests. The former takes more processing time on the backend server while the later takes less processing time on the backend server.

#### 3.4.5 Reliability

The system must provide all implemented features as stated in the requirement to be reliable. And handle failing cases and runtime errors properly with solutions and fallbacks.

#### 3.4.6 Error Handling

Three types of errors are expected to occur in this system.

- Errors regarding user input mistakes and validation
- Errors on the frontend client
- Errors on the backend server

Errors regarding user input mistakes and validation should to be handled on the frontend and backend. On the frontend users should be notified of their input mistakes and errors and must enter valid inputs before this input data can be sent to the server. And on the backend server the data assumed to be valid must be checked and validated for exploitive and harmful attacks such as SQL injections.

Errors on the frontend client include errors such as errors regarding data fetching, errors regarding data presentation. These are errors related to the frontend library and fetching data from the server. Proper handling of this type of errors
must be implemented to provide a good user experience. For example upon fetching error an error indicator must be provided in place of where the fetched data is supposed to be populated.

Errors on the backend server include unhandled exceptions and mistakes that cause the server to crash under some circumstances. Backend developers must handle all exceptions properly and avoid mistakes that would cause the server to crash. Tests should be prepared and done where possible.

#### 3.4.7 Security

The security concerns to be considered for this system are creating secure connections between client and server, secure storage of password and other sensitive data, preventing SQL injections, detecting and dealing with attacks such as DDoS attacks, differentiating between bots and real users and blocking bots from spamming.

Secure connections need to be made between the client and server in order to transfer all sensitive data securely. This is a solved problem in the web-development industry. And that solution is the `https` protocol, and it is the safest way to transfer sensitive data over the internet.

Secure storage of password can be done using good hashing. Since a password only needs to be verified on the backend server it does not need to be stored in as is. A password can be hashed and stored. Since it is very difficult to calculate the password from the hash it is best to store passwords hashed. And when there is a security fault or breach there can be enough time for users to change their passwords and secure their accounts.

As for other sensitive data where hashing is not an option the security concern is at the host and how the admins are accessing the host. Thus a strong password and multi-factor authentication should be used.

To prevent SQL and other forms of injections on the backend security measures must be taken when handling requests to detect and reject requests containing injected data.

DDoS attacks are deadly to the system's service. Measure must be taken to detect and prevent DDoS attacks such as timeouts.

Bots and spamming can be prevented using Captchas.

### 3.5 System Model

#### 3.5.1 Scenarios

##### 1 Scenario for registering in the system

- **Initial assumption:**
    The user has opened the web-app on a modern browser using the proper URL, either for the first time or after logging out previously.
- **Normal flow of events:**
    The user enters their full name, password, email, phone number, address and attach documents that prove national identity such as national ID or passport, then clicks on register. After that the registration information is stored on the back-end temporarily until validated and verified. A verify account registration email is sent to the provided email address. The user opens their email and clicks on the verify link which then completes the registration. If the identity verification attachment is verified to be valid then the user will be registered in the system.
- **What can go wrong:**
    The user enters passwords that do not match. The user should be notified on the page and must enter matching passwords. The user enters an invalid information. The user should be notified on the page and must enter a valid information.The user provides an invalid identity verification attachment. The user must be notified and must be given a form to provide a valid identity verification attachment through a link sent via email.
- **System state on completion:**
    The user is registered successfully in the system. The user information provided is stored on a database in the system. The password is hashed before storing.

##### 2 Scenario for logging in into the system

- **Initial assumption:**
    The user has opened the web-app on a modern browser using the proper URL, either for the first time or after logging out previously.
- **Normal flow of events:**
    The user enters email and password and clicks on login. The email and password are validated on the page and then requested to be verified on the back-end. On successful validation and verification the user will be logged in.
- **What can go wrong:**
    User enters invalid email or password. The user is notified on the page and must enter a valid email and password.User is not registered on the system using the provided email. User must be notified on the page and must either register first or enter the email address they registered.
- **System state on completion:**
    The back-end server creates a session and the session cookie is stored on the browser used for automatic login until expiry date.

##### 3 Scenario for resetting password

- **Initial assumption:**
    The user has opened the web-app on a modern browser using the proper URL, either for the first time or after logging out previously. And they are trying to login but they forgot their password.
- **Normal flow of events:**
    The user clicks on forgot password and is provided with a reset password form in which they must enter their email address. After which the email address is validated and verified and then a password reset link is sent via the email. The user opens their email and clicks on the password reset link which leads to a password reset form. Then they must enter a new password and click on reset.
- **What can go wrong:**
    The user enters an invalid email address. The user must be notified on the page and must enter a valid email.The user enters an email that has not been registered on the system. The user must be notified on the page and must register or contact support.The user does not enter a matching password. The user must be notified on the page and must enter matching passwords.
- **System state on completion:**
    The password is hashed and then updated on the database.

##### 4 Scenario for logging out of the system

- **Initial assumption:**
    The user has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system.
- **Normal flow of events:**
    The user clicks on logout and they are logged out of the system.
- **System state on completion:**
    The session is destroyed. And the session cookie is discarded.

##### 5 Scenario for an administrator registering an employee in the system

- **Initial assumption:**
    The administrator has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system.
- **Normal flow of events:**
    The administrator clicks on register employee which opens the employee registration form. The administrator enters the information required and clicks on register. The employee information is then verified.
- **What can go wrong:**
    The administrator enters an invalid information. The administrator must be notified on the page and must enter a valid information.
- **System state on completion:**
    The employee information is stored on the database.

##### 6 Scenario for an administrator firing an employee

- **Initial assumption:**
    The administrator has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system.
- **Normal flow of events:**
    The administrator clicks on remove employee which opens the employee firing form. The administrator filters and searches for the employee they need to fire from the list of employees and click on fire. The administrator is then prompted for reason of firing and must enter a reason and click on continue. The employee is then notified of their new status.
- **What can go wrong:**
    The administrator needs to undo the firing process. They can only undo the firing process before the employee information is archived after a certain amount of time.
- **System state on completion:**
    The employee information on the database is marked as fired and archived after a certain amount of time.

##### 7 Scenario for an administrator setting the salary of an employee

- **Initial assumption:**
    The administrator has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system.
- **Normal flow of events:**
    The administrator clicks on set employee salary which opens the employee list form. The administrator filters and searches for the employees they need to set salary for from the list of employees. And then they must select at least one employee before they can click on set salary. The administrator is then prompted for amount of salary and must enter a valid amount and click set salary. The employee is then notified of their new salary.
- **What can go wrong:**
    The administrator enters an invalid amount for salary. They must be notified on the page and must reenter a valid amount for salary.
- **System state on completion:**
    The employee salary information on the database is updated to the new amount.

##### 8 Scenario for a manager registering a courier in the system

- **Initial assumption:**
    The manager has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system.
- **Normal flow of events:**
    The manager clicks on register courier which opens the courier registration form. The manager enters the information required and clicks on register. The employee information is then verified.
- **What can go wrong:**
    The manager enters an invalid information. The manager must be notified on the page and must enter a valid information.
- **System state on completion:**
    The courier employee information is stored on the database.

##### 9 Scenario for a manager firing a courier

- **Initial assumption:**
    The manager has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system.
- **Normal flow of events:**
    The manager clicks on remove employee which opens the employee firing form. The manager filters and searches for the courier they need to fire from the list of employees and click on fire. The manager is then prompted for reason of firing and must enter a reason and click continue. The courier is then notified of their new status.
- **What can go wrong:**
    The manager needs to undo the firing process. They can only undo the firing process before the employee information is archived after a certain amount of time.
- **System state on completion:**
    The courier employee information on the database is marked as fired and archived after a certain amount of time.

##### 10 Scenario for a manager assigning a delivery task to a courier

- **Initial assumption:**
    The manager has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system.
- **Normal flow of events:**
    The manager clicks on view orders which opens the employee orders form. The manager then groups and selects orders by region and area and clicks assign courier. The manager is then provided with a list of the nearest available couriers ordered performance record. Then the manager chooses from this list and clicks on assign. A delivery task is created its status set to assigned, and the selected courier is notified.
- **What can go wrong:**
    There are no couriers available to deliver in that region or area. The manager must retry when couriers are available, or look to hire new couriers to work in that area if there is enough demand.
- **System state on completion:**
    A delivery task is recorded on the database and is properly associated with courier and order.

##### 11 Scenario for a manager handling a failing delivery case

- **Initial assumption:**
    The manager has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system.
- **Normal flow of events:**
    The manager is notified of failing delivery cases and follows the notification and views the related order and delivery task. The manager reads and assesses the reason of failure. Then the manager contacts the courier and requests for more information. The manager also calls the customer if required. The manager commands the courier to deliver the items either back to the vendor, or to the company for legal assessment and lawyer advised decision making. If the courier had an accident or cannot deliver then the manager assigns a new delivery task from the failing courier to the vendor or company.
  - **System state on completion:**
    The failing delivery task is recorded as failing with the detailed reason and proof attached to it. And a new delivery task recorded on the database and is properly associated with courier and order.

##### 12 Scenario for a courier viewing assigned delivery task

- **Initial assumption:**
    The  courier has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system.
- **Normal flow of events:**
    The courier is notified of assigned delivery tasks and follows the notification and views the delivery task with the related orders. Then the courier accepts the delivery task.
- **What can go wrong:**
    The courier rejects the delivery task by specifying a reason.
- **System state on completion:**
    The delivery task status is changed to active and associated with the accepting courier.

##### 13 Scenario for a courier requesting items from vendor

- **Initial assumption:**
    The  courier has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system. And they have accepted a delivery task.
- **Normal flow of events:**
    The courier drives to the vendor that provides the items in the order assigned. The courier contacts the vendor and notifies them of arrival and asks to take the items for delivery. Then the vendor gives the requested items to the courier by following the proper item exchange steps. The courier only accepts the items that are in the expected condition and reports the other items that are not in the expected condition. The courier then delivers the items to the customer's receiving location.
- **What can go wrong:**
    The courier rejects the items in unexpected condition and reports them.
- **System state on completion:**
    The delivery task status is changed to en-route with the received items' states set to being delivered.

##### 14 Scenario for a courier confirming delivery of items to customer

- **Initial assumption:**
    The  courier has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system. And they have accepted a delivery task and now en route to the customer's receiving location.
- **Normal flow of events:**
    The courier then arrives with the items at the customer's receiving location. If the location is a post office box then the courier fills the required forms and gives it to the post office. Or if the location is a place where the customer waits for the items then the courier contacts the customer and meets them to give them their items.  
- **What can go wrong:**
    The courier rejects the items in unexpected condition and reports them.
- **System state on completion:**
    The delivery task status is changed to completed with the received items' states set to deposited if the location is a post office.  
    The delivery task status is changed to delivered with the received items' states set to transferring if the location is the customers receiving location.

##### 15 Scenario for a courier confirming transfer of items to customer

- **Initial assumption:**
    The  courier has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system. And they have accepted a delivery task and now meeting the customer to transfer items.
- **Normal flow of events:**
    The courier asks them to view and fill out the item acceptance form on the web-app. The customer views the delivered items and accepts those that are in the expected condition and rejects those that are not in the expected condition by specifying proper reasons. Then the courier gives the accepted items to the customer and takes back the rejected items. The courier confirms the transfer of items to customer.
- **What can go wrong:**
    The customer rejects the items in unexpected condition and reports them.
- **System state on completion:**
    The delivery task status is changed to completed with the received items' states set to transferred.

##### 16 Scenario for a customer confirming delivery of items

- **Initial assumption:**
    The customer has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system. And they have been notified of the incoming delivery and now meeting the courier to receive items.
- **Normal flow of events:**
    The courier asks them to view and fill out the item acceptance form on the web-app. The customer views the delivered items and accepts those that are in the expected condition and rejects those that are not in the expected condition by specifying proper reasons. Then the courier gives the accepted items to the customer and takes back the rejected items. The courier confirms the transfer of items to customer.
- **What can go wrong:**
    The customer rejects the items in unexpected condition and reports them.
- **System state on completion:**
    The delivery task status is changed to completed with the received items' states set to transferred.

##### 17 Scenario for a customer browsing items in stock

- **Initial assumption:**
    The customer has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system.
- **Normal flow of events:**
    The customer enters keywords on the search-bar and chooses filter criteria and clicks on browse. Then a limited list of available items is presented to them for picking.
- **What can go wrong:**
    There are no items found.

##### 18 Scenario for a customer putting items in cart

- **Initial assumption:**
    The customer has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system. And the customer is now browsing for items.
- **Normal flow of events:**
    The customer picks from the items presented and clicks on the put-in-cart button. Then the picked items are added to the customer's cart.
- **What can go wrong:**
    The items put in cart are out of stock.
- **System state on completion:**
    The customers cart is aggregated with the picked items using cart-item table in the database. cart-item table contains item reference and quantity information and is associated with a cart.

##### 19 Scenario for a customer views items in cart

- **Initial assumption:**
    The customer has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system. And the customer has opened up their cart by clicked on my-cart button.
- **Normal flow of events:**
    The customer is presented with the list of items in their cart with information such as name, brief description, quantity, and price per item, and total price, delivery costs, and other fees.
- **What can go wrong:**
    The items put in cart are out of stock. The customer must remove the items before purchasing.
- **System state on completion:**
    The customers cart is aggregated with the picked items using cart-item table in the database. cart-item table contains item reference and quantity information and is associated with a cart.

##### 20 Scenario for a customer removes items from cart

- **Initial assumption:**
    The customer has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system. And the customer has opened up their cart by clicked on my-cart button.
- **Normal flow of events:**
    The customer is presented with the list of items in their cart. They select items in their cart and click on remove. Then they are prompted to confirm removal of items from cart. Then the items are removed from their cart.
- **What can go wrong:**
    The items cancels the removal of items.
- **System state on completion:**
    The customers cart is cleared of the removed cart-items in the database.

##### 21 Scenario for a customer changes quantity of items in their cart

- **Initial assumption:**
    The customer has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system. And the customer has opened up their cart by clicked on my-cart button.
- **Normal flow of events:**
    The customer is presented with the list of items in their cart. They click on the amount number input and enter a new amount or they can click on decrement or increment buttons if provided. Then the quantity of the items in their cart will be changed.
- **What can go wrong:**
    The items cancels the removal of items.
- **System state on completion:**
    The quantity of items in the customer's cart is updated in the database.

##### 22 Scenario for a customer purchases items in their cart

- **Initial assumption:**
    The customer has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system. And the customer has opened up their cart by clicked on my-cart button.
- **Normal flow of events:**
    The customer is presented with the list of items in their cart. They are done viewing and modifying their cart and now ready to make a purchase. They click on the purchase button. Then they are provided with payment options which they choose from and complete payment using supported payment APIs. Upon successful payment a new order is created, and the transaction recorded and associated with the order. The money paid is stored in company owned customers-holding bank account.
- **What can go wrong:**
    The payment fails.
- **System state on completion:**
    A new order is created and associated with cart-items and transaction record in the database.

##### 23 Scenario for a customer canceling an order

- **Initial assumption:**
    The customer has opened the web-app on a modern browser using the proper URL, and they are currently logged in into the system. And the customer has opened up their list of orders by clicking on my-orders button.
- **Normal flow of events:**
    The customer is presented with the list of orders they have made. They select the orders they want to cancel and then click on cancel-order. Then they are prompted for confirmation and reminded of the consequences of canceling the order(s). If they confirm then the orders will be set to canceled and any progress to deliver the items in the orders(s) is undone and costs and fees are deducted before the money is returned back to the customer. These means items will be returned back to the vendor if they were in the process of being delivered.
- **What can go wrong:**
    The customer does not confirm cancellation of the order(s).
- **System state on completion:**
    The orders' status is set to canceled and the items' states to in-stock in the database.

##### 24 Scenario for completion of delivery

- **Initial assumption:**
    The courier has successfully delivered items to customer and the customer has accepted the items delivered.
- **Normal flow of events:**
    The money paid by the customer is transferred to the vendor minus fees and costs, and this transaction record  is then associated with the order.
- **System state on completion:**
    The order is associated with the transaction record and set to completed status in the database.

#### 3.5.2 Use Case Diagram

![use-case-diagram--actors](media/use-case/actors.drawio.svg)  
![use-case-diagram--session](media/use-case/session-management.drawio.svg)  
![use-case-diagram--main-1](media/use-case/main-1.drawio.svg)  
![use-case-diagram--main-2](media/use-case/main-2.drawio.svg)  
![use-case-diagram--main-3](media/use-case/main-3.drawio.svg)  

<!-- ![use-case-diagram--actors](https://raw.githubusercontent.com/nati8333/online_shopping_webapp/main/software%20requirement/spec/media/use-case/actors.drawio.svg)  
![use-case-diagram--session](https://raw.githubusercontent.com/nati8333/online_shopping_webapp/main/software%20requirement/spec/media/use-case/session-management.drawio.svg)  
![use-case-diagram--main-1](https://raw.githubusercontent.com/nati8333/online_shopping_webapp/main/software%20requirement/spec/media/use-case/main-1.drawio.svg)  
![use-case-diagram--main-2](https://raw.githubusercontent.com/nati8333/online_shopping_webapp/main/software%20requirement/spec/media/use-case/main-2.drawio.svg)  
![use-case-diagram--main-3](https://raw.githubusercontent.com/nati8333/online_shopping_webapp/main/software%20requirement/spec/media/use-case/main-3.drawio.svg)   -->

#### 3.5.3 Sequence Diagram

![login-session--seq](media/sequence/login-session.drawio.svg)  
![customer-purchase--seq](media/sequence/customer-purchase.drawio.svg)  
![vendor-stock--seq](media/sequence/vendor-stock.drawio.svg)  
![manager-courier--seq](media/sequence/manager-courier.drawio.svg)  
![courier-delivery--seq](media/sequence/courier-delivery.drawio.svg)  

<!-- ![login-session--seq](https://raw.githubusercontent.com/nati8333/online_shopping_webapp/main/software%20requirement/spec/media/sequence/login-session.drawio.svg)  
![customer-purchase--seq](https://raw.githubusercontent.com/nati8333/online_shopping_webapp/main/software%20requirement/spec/media/sequence/customer-purchase.drawio.svg)  
![vendor-stock--seq](https://raw.githubusercontent.com/nati8333/online_shopping_webapp/main/software%20requirement/spec/media/sequence/vendor-stock.drawio.svg)
![manager-courier--seq](https://raw.githubusercontent.com/nati8333/online_shopping_webapp/main/software%20requirement/spec/media/sequence/manager-courier.drawio.svg)  
![courier-delivery--seq](https://raw.githubusercontent.com/nati8333/online_shopping_webapp/main/software%20requirement/spec/media/sequence/courier-delivery.drawio.svg)   -->

#### 3.5.4 Collaboration Diagram

![collaboration--diag](media/collaboration/collaboration.drawio.svg)  

<!-- ![collaboration--diag](https://raw.githubusercontent.com/nati8333/online_shopping_webapp/main/software%20requirement/spec/media/collaboration/collaboration.drawio.svg)  -->

## Chapter 4 | System Design

### 4.1 Overview

After analysis modeling the next step is creating system design based on that analysis models.

### 4.2 System Architecture

The architecture model that is best to use for this project is a hybrid MVC and server-client architecture model. The MVC architecture is on the client side and since there is client-server communication there is also a server-client architecture model.

One of the best software out there at this time are Node.js and React.js which are best fit for this architecture model. React.js offers a dynamic client-side MVC functionality and Node.js offers single-threaded high performance backend servers such as Hapi.js and a lot of 3rd party library support.

#### 4.2.1 Subsystem Decomposition

The overall system now has to be decomposed into subsystems. The subsystems of this system are user management system, employee management system, session management system, email token-verification system, delivery management system, vendor-stock management system, payment system, item-cart system, item search and filter system.

#### 4.2.2 Hardware and Software Mapping

The subsystems are going to be deployed on certain hardwares. Here are the software hardware mappings:

- user management system, employee management system, session management system, email token-verification system, delivery management system, vendor-stock management system, payment system, item-cart system, item search and filter system.

#### 4.2.3 Component Diagram

![component-diagram--ER](media/component/component-diagram.drawio.svg)  

<!-- ![component-diagram](https://raw.githubusercontent.com/nati8333/online_shopping_webapp/main/software%20requirement/spec/media/component/component-diagram..drawiosvg)   -->

#### 4.2.4 Deployment Diagram

![deployment-diagram--ER](media/deployment/deployment-diagram.drawio.svg)  

<!-- ![deployment-diagram](https://raw.githubusercontent.com/nati8333/online_shopping_webapp/main/software%20requirement/spec/media/deployment/deployment-diagram..drawiosvg)   -->

#### 4.2.5 Persistent Data Management

Persistent data in this system include database records, images and other attachment files. The database will be managed locally on the server using DBMS such as MySQL and accessed and modified through an API. Image and other attachment files are stored in the filesystem and privately accessed through a properly authorized request router.

#### 4.2.6 Database Design

The database can be design using a great tool such as MySQL Workbench which provides all the features needed for fast and reliable database design. It provides visual diagraming, backward and forward engineering features among other basic features.

##### 4.2.7 Entity Relationship Diagram

![entity-relationship--ER](media/entity-relationship/on-shop-EER-UML.svg)  

<!-- ![entity-relationship--ER](https://raw.githubusercontent.com/nati8333/online_shopping_webapp/main/software%20requirement/spec/media/entity-relationship/on-shop-EER-UML.svg)   -->

#### 4.2.8 Access Control

Access to database will be managed mainly by the provided MySQL server access control system and using predefined procedures and selective access grants.

Access to images and other attachment files will be stored in a private directory and managed by a router on the backend server which fulfills requests based on proper authorizations.

**Access Matrix**:

> Let DB stand for Database and PRM stand for Private Resource Manager.  
> PRM.Attachment represents image files or other attachments files.

| Actor          | DB.Routine Call   | DB.Table Select    | DB.Table Update   | DB.Table Delete    | PRM.Attachment Fetch | PRM.Attachment Upload |
| -------------- | ----------------- | ------------------ | ----------------- | ------------------ | -------------------- | --------------------- |
| Admin          | Any               | Any                | Any               | Any                | Any                  | Any                   |
| User           | Self,BankAccount  | Self,BankAccount   | Self,BankAccount  | Self,BankAccount   | Self                 | Self                  |
| Employee       | Self              | Self               | Self              | Self               | Self                 | Self                  |
| Manager        | Self,Employee     | Self,Employee      | Self,Employee     | Self,Employee      | Self,Employee        | Self,Employee         |
| Courier        | Self              | Self               | Self              | Self               | Self                 | Self                  |
| Customer       | Self,Cart         | Self,Cart          | Self,Cart         | Self,Cart          | Self                 | Self                  |
| Vendor         | Self,Stock        | Self,Stock         | Self,Stock        | Self,Stock         | Self                 | Self                  |

#### 4.3 User Interface Design

We will use Bootstrap 5 and react-icons to design a responsive and modern UI. Bootstrap 5 offers a wide variety of styles, responsive designs and scripts for interactivity by just using HTML classes. React-Icons provides a wide variety of icons for use in Node.js and React.js.

## Chapter 5 | Implementation

### 5.1 Overview

This system is going to be implemented using a Node.js environment using libraries React.js, Hapi.js, Bootstrap 5, React-Icons. And as much of the targeted features are going to be implemented incrementally and improved iteratively.

### 5.2 Coding Standard

The programming languages to be used are HTML, CSS, Javascript, Typescript.

#### HTML Coding Standards

- HTML-5 should be used.
- Tags and attributes should be broken into on a new line if the line-character-count exceeds 100.
- Start and end tags should either be on the same line, if small, or on different lines with the same indent.
- Tag attributes should be broken into new lines and indented by one more than the tags indent with the closing `>` or `/>` sign not on a new line by itself.

#### CSS Coding Standards

- CSS3 should be used.
- Selectors should be broken into on a new line if the line-character-count exceeds 100.
- Style definitions should be indented once compared to the parent indent.

### Javascript Coding Standards

- Code should be broken into a new line if the line-character-count exceeds 100.
- Braces should be on the same line at the end. like so `const foo = function() {`, `if(...) {`, `} else {`
- No spaces should be put between keyword or function name and the parenthesis after. like so `for(`, `if(`, `function foo(`
- Self-explanatory names should be chosen as compared to redundant and verbose comments.

### 5.5 Prototype

The basic prototype should implement session-management and the forms/pages prioritized from most important to least important.
The implementations should be filled with stubs and later implemented.

### 5.6 Implementation Detail

#### Authentication

- Session-cookie based authentication will be used to track session data. The session cookie will be created if the user has logged in with valid credentials.

...

## Chapter 6 | Testing

### 6.1 Introduction

Unit tests can be prepared and used to test individual components of the system where unit testing is required. And integration testing can either be prepared code or user interaction testing and the least required regression testing should be done with each integration.

### 6.2 Scope

Testing should focus on error/bug avoidance, exception handling and providing a good user experience.

### 6.3 Resources

Testing libraries.

### 6.4 Schedule

Testing should be done before pushing to the central repo to ensure a working code is integrated into the system.  
Other than that regular user-interaction testing should be done to get feedback and bug reports.

### 6.5 Estimated Risk and Contingency Plan

One major risk is that sufficient testing has not been implemented and thus the system will have vulnerabilities. This can be avoided by doing enough research on features that require high security and provide very important functionality. Professional advice should be sought and considered.

In case of failure of new version of the system the system should be changed to a previous stable version. And the failing version of the system should be put under evaluation for bad test implementations.

## Chapter 7 | User Manual and Demo

### 7.1 User Manual

### 7.2 Demo

## References

[Ethiopia Commodity Exchange Proclamation No. 550 of 2007](https://leap.unep.org/en/countries/et/national-legislation/ethiopia-commodity-exchange-proclamation-no-550-2007)  
[National Payment System(Amendment) Proclamation No.1282/2023](https://nbe.gov.et/files/national-payment-systemamendment-proclamation-no-1282-2023/)  

[Node.js SQL Injection Guide Examples and Prevention](https://www.stackhawk.com/blog/node-js-sql-injection-guide-examples-and-prevention/)  
[Best Practices To Prevent DDoS Attacks](https://securityscorecard.com/blog/best-practices-to-prevent-ddos-attacks/)  
[How To Avoid Time-based DDoS Attacks In Node.js](https://www.nearform.com/blog/avoid-time-based-ddos-attacks-node-js/)  
[A quick way for hashing passwords using Bcrypt with Nodejs](https://medium.com/@manishsundriyal/a-quick-way-for-hashing-passwords-using-bcrypt-with-nodejs-8464f9785b67)  

[Being iterative and incremental in software development](https://nulab.com/learn/software-development/iterative-incremental-software-development/)  
[What is the Best Place for Storing Uploaded Images](https://stackoverflow.com/questions/348363/what-is-the-best-place-for-storing-uploaded-images-sql-database-or-disk-file-sy)

[Data Dictionary](https://www.splunk.com/en_us/blog/learn/data-dictionary.html)

[StackOverflow](https://stackoverflow.com/)  
[MySQL](https://www.mysql.com/)  
[Node.js](https://nodejs.org)  
[Hapi.js](https://hapi.dev/)  
[React.js](https://react.dev/)  
