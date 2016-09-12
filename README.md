# Web-Applications-Engineering
Assignment2

Group Assignment - 25 Marks (Group of Max 5)

Aims and Background
This project aims to give students hands-on experience in:
Designing and implementing a fully-functional Web application.
Using well-known application patterns such as MVC.
Using JDBC and related technologies to maintain persistence of user data.
The theme of assignment will be oriented around online bookstore sites, similar to Amazon bookstore. Your assignment is to design and implement a web application that allows commercial trading of publications (e.g. books).

The assignment will build-upon the work conducted in Assignment 1 - with respect to business logic and user-interface. However, you will need to make sure to "convert" your data-layer so that it is fully relational. You cannot re-use the XML DB that you have implemented for Assignment 1.

Requirements
The core requirements of this assignment are organised across the following five modules:
User Registration.
Book Seller: Offering Items for Sale.
Customer: Search and buy publications.
Admin Functionality.
Graph Store and Visualization.
The following modules are expected to be re-use from Assignment 1 (and must also be included in the deliverable as part of this assignment):
The underlying platform.
Search Facility.
Shopping Card.

1. User Registration
A user visits a registration page and enters the following details: a username, a password, an email address.
This page displays a form with the current values of: username, nickname, first name, last name, email, year of birth, full address and credit card number. (Use a dummy credit card number since you will not be interacting with real payment systems)
On submitting this information, the system sends an email containing a confirmation URL to the supplied address.
The user reads the email, goes to the confirmation URL; the system confirms the registration.
Every detail other than the username can be changed at any time by the user.

2. Book Seller: Offering Items for Sale
User A logs into his/her account.
User A can add a new Item (Book, Journal, Conference, etc). Item attributes are defined in Assignment1, e.g. title, authors, publication-type, publication-date, and venues. You will aslo need to consider the 'price' and 'picture' attributes.
The user clicks a button to register the item. This will enable the item to be represented in the search results.
The user should be also able to "Pause" the registered item. This will temporarily place the item on hold and remove them from search.
Note: You have to ensure to implement the system such that it will enable multiple book sellers use the system simultaneously.

3. Search and Buy
This functionality works as follows:
User B logs into his/her account.
User B searches for a particular item; (refer to Assignment1 specs).
The results of the search are displayed as a list.
Clicking on an item in the list takes the user to the page for the item, showing Title, Picture, authors, etc.
The user can add/remove entries from his/her Shopping Cart; (refer to Assignment1 specs). 
If the use buy an item, an email will be automatically sent to the book seller, informing the seller that the item has been sold.

4. Admin Functionality
The admin is a special account in the system which can only be accessed via a separate page (that is, not the usual user login page). The admin has the following functions:
Remove an item from sale.
Ban a user from the site.
Monitor customer activities:
The admin should be able to select a customer (not the book seller).
Customer activity report will be shown. This report includes: the items that has been bought (only: pub-title, timestamp, price, seller), and the items that has been added to the Shopping Card but removed after a while (only: pub-title, added-timestamp, removed-timestamp). To achieve this you will need to trace the customer activities and store them in a table(s).
The pub-title should be a link: when clicked addidtional information (e.g. author, etc.) about the publication will be shown.

5. Graph Store and Visualization
Create two triple tables to store the entities (minimum: Author, Publication and Venue) and the relationships (minimum: "paper--(authoredBy)-->author", "paper--(publishedIn)-->venue", and "") among them.
Support the following queries on the graph nodes (e.g. author) attributes (e.g. name): (1) search for an authors; (2) search for a publications; and (3) search for venues
Visualize the search result as a graph. For the visualiztion, you can use existing APIs such as "https://d3js.org/" and "http://visjs.org/".

Assignment Execution

System Requirements
You should use a minimum of Java, JSP/Servlets, and JDBC. Apache Tomcat should be used as the Web application server. You can choose whatever database you would like to use. Also, you are allowed to use any package/library or framework.

You can demonstrate your assignments using CSE lab computers as well as your laptops.

You will see a series of J2EE Design Patterns in the labs (and also in lectures). Your application must be based on the MVC pattern and you must be able to identify the different layers in your code.

Submission and Demo
The due date for this assignment is (end of Mid Semester Break): Sunday, 2 October 2016, 23:59:59.

After testing, generate a war file from your project. In Eclipse, this is Right-Click on project name --> Export --> WAR file. Make sure that the "Export Sources" checkbox is checked.
email the WAR file to the following email address:

To: unsw.cse.comp9321@gmail.com
CC: All your group members
From: [Your unsw email address]
Subject: COMP9321-Ass2-S2_16
Body: 
  [group id]
  For-each Group member: [Student Number]-[Student Name]
Important Notes:
This email address (unsw.cse.comp9321@gmail.com) is only for submitting your assignemts. For other inquiries please contact your lecturer.
You do not need to email the Database files. The WAR file will be sufficient.
You can demonstrate your assignments using CSE lab computers as well as your laptops.
The following additional libs are accepted: JSTL. And for front-end purposes, JQuery and Bootstrap. Additionally, any other Javascript libs that are simply referenced (i.e. without having to add to the build path) in your HTML/JSP page is accepted.
 
Demos
Demo will be held during the lab times in week 10. You should use the same .war file that you submitted for your demo.
Each demo will be around 10-15 mins long.

Evaluation and Marking
This assignment is worth 25 marks and will be marked on a group basis. A more detailed marking specification has now been provided (Download Assignment 2 Marking Scheme). Other factors of importance is: Quality of Demo, which includes incorporating features such as high quality data for demo, input form validation, guarded views, and preventing form resubmission on pressing back button. Extra innovation is also encouraged - feel free to experiment or incorporate features found in other online bookstore websites. 
Late Submissions and Penalties

Late submissions will lose 2 marks on the first day, and 1 mark per day after that.
Important

Please use the message board for questions, resolving doubts.
