# Vintage Store 

Please visit the website [here](https://vintagestore-9c006be944c1.herokuapp.com/).

## Introduction and purpose
Vintagestore e-commerce website is developed as part of the Milestone project 5 for Code Institute Diploma in Software Development with eCommerce. Vintagestore is an e-commerce application built in Django, incorporating HTLM, CSS and Python.

The application is built to provide a functional solution for a e-commerce business selling vintage clothing and accessories. The Admin User of the application is able to manage items in the website, users/customers, as well as their orders and queries. 

The target audience of this website are users interested to purchase brand new and second-hand fashion items with a vintage style. Users can register in the Vintagestore website, manage their user profiles, make orders and their payments.

## Design
This section includes how the Vintagestore e-commerce application has been developed, going from its concept to the ultimate solution used to develop the site.

### 1-Concept
The aim of this project was to develop a e-commerce application that is fully functional, allowing the business owner to run a fashion store offering and selling products online.

The business owner of Vintagestore is the User Admin, that manages upload, edit and deletion of items via UI; and via Django's admin portal. 

The website is thought looking to attract prospects and customers interested in purchasing vintage clothing and accessories.  

The application was developed to be simple to use for customers.  Users can browse for vintage items, leave reviews and score products, create a wish list, purchase items with debit/credit card, create a user profile that retains customer’s address and contact details allowing to facilitate and have a quicker experience during the customer’s next purchase.

### 2-Functional scope
In order for the application to operate as required, the following areas have been developed:

**Website administration** - the Admin User primarily manages the site through the Django's framework admin portal.  Admin User also has permission to manage site (adding, editing, delete items) within the UI.  

**Registration and Login**- users can register to the website through the navbar => Customer Centre menu.  Django Allauth solution supports the registration and login process.  A registration email notification is received by the user when registering on the website.

**User Profile** - once users are registered on the website, users can keep their information updated in their profile.  Within the profile, users are also able to view the history of orders placed. 

**Contact US**- IN DEVELOPMENT 

**Customer Reviews**- IN DEVELOPMENT 

**Wishlist**- IN DEVELOPMENT 

**Bag** - the bag functionality allows users to add and keep items in their bag, should they decide to proceed and complete the purchase of these items. Each addition of an item will update the bag, as well as provide user with a (pop-up) notification message. Within the bag, a user can perform actions of updating the quantity required of an item, or remove the item of the bag. The bag also allows the customer user to proceed to the website check-out section, in order to complete the purchase.

**Checkout**- the check-out section allows users to complete the purchase of item/s added in the bag. As part of the check-out process, the user needs to provide the following details: name, email address, and shipping address.  User also needs to include a debit/credit card as method of payment in order to complete the purchase.

**Card payments**- the application incorporates credit card payment solution provided by Stripe, which allows to provide real time feedback to customer users in situations where the credit card payment is rejected, or the card number is incorrect. (Also, there are mutliple events, which Stripe will provide detailed feedback on to a user if required).

**Newsletter**- IN DEVELOPMENT 

### 3-Solution
The solutions outlined below were used to develop the application:

**Languages**
The following languages were used:
* HTML
* CSS
* Python
* Javascript

**Data and Database**
The application required a database structure to support the e-commerce structure. Code Institute's PostgreSQL was used as database solution for this project.  The data was designed and organised as a relational database.  The needs in terms of the database relate to managing of website items, user profiles/accounts, purchase orders, user messages, user reviews of items, bag and wishlist.
Images and static files for application are stored in Amazon's AWS S3.


**Security**
The following features have been incorporated during the development of the application:

* Django's Allauth for user registration and authentication management.
* Un-authorised users attempting to access retricted URLs, will be prompted to Login screen, not being able to access the restricted feature (I.e:  Product Management, authorised for superusers).
* Payments for purchases are securely processed using Stripe as payment management platform.
* CSRF token feature used throughout the application to prevent unauthorised access and potential malicious attacks.

**Development**
The following technologies have been used during the application development:

* GitHub repository to store the project's code after being pushed from Gitpod.
* Gitpod IDE for version control by utilizing the Gitpod terminal to commit and Push to GitHub.
* Django framework to develop structure of the application, as well as to use some of the already developed functions as user authorisation or admin portal.
* Bootstrap5 for construction of the application, and responsiveness.
* Crispy forms library.
* DrawSQL for drawing database schema.
* Balsamiq for creation of wireframes.
* Google Gmail for sending user emails.
* Heroku for hosting the application.
* ElephantSQL to manage database of the application.
* AWS for storing static files and product images.
* Mailchimp to manage collection of newsletter signups from users.
* Facebook to create facebook business page.

### 4-Wireframes
TO BE ADDED 

### 5-User Stories
The development of this website is based on User Stories created for this project. The User stories were managed through a Kanban board in GitHub. There were a total 19 User Stories, labelled to reflect the following categories: Must-Have, Should-Have and Could-Have. During development of the project, User Stories were moved from To Do => In Progress => Done sections within the Kanban board.

### 6-E-commerce business model and marketing
Business model:
Vintagestore is a business to consumer (B2C) e-commerce application that offers vintage clothing and accessories that users can purchase.  
Users browsing the site, can access to available items pictures and details, without being registered in the website.  
Users that purchase an item, are required to register; and avail the site to store their shipping details, as well as keep track of their previous orders.
As of now, the method of payment allowed to proceed with a purchase is debit/credit card.  (In the roadmap to be considered as business growths, are other method of payments such as: mercado Pago/amazon, Google pay, Apple Pay).
It is planned to enhance the e-commerce business application, and allow users to post their own vintage fashion items and sell them through the website.  Vintagestore would deduct a fee from each of these selling transactions within the website, and this would encourage the circular fashion model that contributes to improve the environment as well. 

Marketing:
The following marketing strategies/tools have been used to promote the business:

**SEO** -IN DEVELOPMENT

**Facebook business page** - IN DEVELOPEMENT

**Newsletter** - IN DEVELOPEMENT

## User Experience
Vintagestore has been developed to attract customers interested in vintage fashion. The aim of the project was to develop a user friendly and intuitive app; simple for users to browse items, make purchases, review items and contact Vintagestore if needed.

## Features
This document section reflects features currently available in the website:

-Homepage
Homepage includes the message “Welcome to the world of vintage fashion’, and a button that allow users to access items published on the website.

-Navigation Bar, User Menu, and Site Search
Navigation bar allows users to select options from Customer Centre menu ( ). Users can type in the search option to find items; and view the current total pending in the user's shopping bag.

-Footer
IN DEVELOPMENT 

-Products Page
The products page currently displays rows of 4 products; and allow users to view more details about each specific item by clicking on the image. The name, price, and rating of the item are reflected below each item image.

-Individual Product Page
The individual item's page display the item enlarged image; allow the user to select the quantity of items to be added to the shopping bag (and decrease or increase quantity by clicking on minus or plus icons). Users can add the item/s to the shopping bag, or select the button to continue shopping through the website. Users that are logged-in are able to select size of selected item/s before adding item/s to the shopping bag.

-Shopping Bag
The shopping bag displays items previously added by user, allowing user to adjust the item quantity if needed. Users can alternatively remove items from the shopping bag.  Users can opt to continue shopping by selecting button, or continue to the checkout process.

-Checkout
In the checkout section, users are able to view details of the selected items to be purchased, and the total value of the order. Users need to populate the required fields (including delivery address, and debit/credit card details) in order to complete the purchase.

-User profile
Within the profile section, registered users are able to update their stored customer details (example: shipping address).  History of previous orders is also available.

-Contact Us
IN DEVELOPMENT 

-Wishlist
IN DEVELOPMENT 

-Customer Reviews
IN DEVELOPMENT 

-User Registration
New users are able to register in the website through Customer Centre section => Register. 

-User Login
Registered users are able to login to the Vintagestore website through Customer Centre section => Login.

-User Logout
Logged users are able to logout from their profile, through the Customer Centre section => Logout.

-Admin Product Management
Admin User is able to add/edit/delete items via UI, through Customer Centre section => Product Management.This feature is only available for superuser (Admin User).

-Admin Portal
Admin User has permission to access and manage the Vintagestore website through Django's admin portal.

Future feature developments and enhancements 
This section includes feature developments and enhancements to be considered, in order to improve user experience within the application and looking to improve business profitability:

-Include a chatbot functionality available to users that lands in the website.  This is aimed to help users in the browsing experience (‘virtual shop assistant’), and providing an automatic response (alternative to leave a message through the ‘Contact Us’ form) in case of any questions/concerns.
-Include a ‘marketplace’ section within the website, through which users can publish and sell their own vintage cloths and accessories.  This feature is aimed to increase business revenue by charging a fee for each sale transaction, as well as it is a way of potentially increase the amount of users accessing the website and making purchases.
-Expand the method of payments allowed to purchase items in the website (Example: add Google pay, Apple Pay).
-Display similar suggested items, if user selects an item that is not available.
-Display instant online notification if an item is not more available at the time when user select it for its purchase.
-Include a blog in the website (as a feature to add, besides the newsletter already available) with latest news and trends of vintage fashion.

Testing
COMPLETED END TO END TESTING TO BE COMPLETED

Functional:
TO BE ADDED 

Code validation testing:
TO BE ADDED 

-HTML code validation
TO BE ADDED 

-Python code validation
TO BE ADDED 

-CSS code validation
TO BE ADDED 

Bugs
TO BE ADDED 

-Fixed bugs:

-Unfixed bugs:


Deployment
The application was deployed in Heroku. A bucket was setup in AWS, to store static files and media images. Payments processing feature was implemented through Stripe as a payment platform. The database content ElephantSQL.

The section below describes the actions for the application deployment.
-Stripe
-DB SQL
-Amazon AWS S3
-Heroku

STATUS OF THE PROJECT
The project itself is still in development and some of the areas of the project are yet to be completed and these had been marked in the readme above with status IN DEVELOPMENT or TO BE ADDED

