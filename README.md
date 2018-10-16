
Software Requirements Specification(SRS)
for
Pioneer Exchange
Version 1.0 approved
Prepared by Delta
4/20/2018

Table of Contents
Table of Contents	2
Revision History	3
1.	Introduction	4
1.1	Purpose	   4
1.2	Document Conventions	  4
1.3	Intended Audience and Reading Suggestions	4
1.4	Product Scope	4
1.5	References	5
2.	Overall Description	5
2.1	Product Perspective	5
2.2	Product Functions	5
2.3	User Classes and Characteristics	     6
2.4	Operating Environment	      6
2.5	Design and Implementation Constraints	    6
2.6	User Documentation	6
2.7	Assumptions and Dependencies	    6
3.	External Interface Requirements	6
3.1	User Interfaces	   6
3.2	Hardware Interfaces	23
3.3	Software Interfaces	24
3.4	Communications Interfaces	24
4.	System Features	25
4.1	System Feature 1	25
4.2	System Feature 2 	26
4.3        System Feature 3            28
4.4        System Feature 4            31
4.5        System Feature 5            32
4.6        System Feature 6            33
4.7        System Feature 7            34
4.8        System Feature 8            36
4.9        System Feature 9            37
5.	Other Nonfunctional Requirements	39
5.1	Performance Requirements	39
5.2	Safety Requirements	39
5.3	Security Requirements	39
5.4	Software Quality Attributes	40
5.5	Business Rules	40
6.	Other Requirements	40
Appendix A: Glossary	40



Revision History
Name
Date
Reason For Changes
Version
Kevin Tran 
4/20/18
Added Introduction and Purpose (Section 1,1.1)
1.0
Kevin Tran
4/24/18
Began Section 4.1 
1.0
Kevin Tran
4/26/18
Began Section 4.2, 4.3, 4.4, 4.5, 4.6, 4.7, 4.8
1.0
Michelle Solitano
4/22/18
Worked on 1.3, 1.4
1.0
Michelle Solitano
4/24/18
Started 2.2, 2.3
1.0
Michelle Solitano
4/26/18
Started 2.1
1.0
Michelle Solitano
4/29/18
Started 2.4, 2.6, 2.7
1.0
Douglas Dunn
5/01/18
Worked on 1.2, 1.3, 1.4, 4.5
1.0
Kevin Tran 
5/01/18
Edited Section 4.3, 4.4, 4.8, 4.9, 4.10, 4.11, 4.12
1.0
Abhishek Lalla
5/03/18
Added Section 3.1, 3.2, 3.3, 3.4
1.0
Abhishek Lalla
5/03/18
Modified header 
1.0
Kevin Tran
5/05/18
Edited 4.7, 4.14
1.0
Michelle Solitano
5/06/18
Edited Glossary
1.0
Douglas Dunn
5/06/18
Worked on 1.2, 1.5, 4.5, table of contents
1.0
Kevin Tran
5/06/18
Revised Section 4
1.0
Abhishek Lalla
5/06/18
Modified 3.1, 4.4, 4,9
1.0
Nima Movasseghi
5/06/18
Finished Section 5
1.0





1.	Introduction
Whether it may be a freshman or senior student attending California State University, East Bay there are many things that are a necessity for them in order to transition or continue their enrollment. It may be a source to find textbooks, living space, current events, etc. that are available on campus that they need. Rather than having multiple outlets to find exactly their core essentials or demands, Pioneer Exchange is a web application that is contributive and available that meshes everything into one website. 
1.1	Purpose 
The purpose of this Software Requirement Specification (SRS) is to describe the Pioneer Exchange Web Application in detail and to provide a list and description of its requirements and expected functionality. It is decomposed and broken down to each individual building blocks in order to fully understand the user interface to best assist its future users. This document will allow for a clear and concise understanding of the product and should be referenced in order to create a correctly functioning initial version of the Pioneer Exchange Web Application. This SRS will serve as a foundation for our team (Group Delta) to build the first version of our project. 
1.2	Document Conventions
Requirements and standards practiced in this SRS are following the IEEE Std 830-1998 - IEEE Recommended Practice for Software Requirements Specifications. Refer to section 3 and 4 for a detailed explanation of higher-level requirements. 
1.3	Intended Audience and Reading Suggestions
The intended audience for this SRS document are for the members of group Delta, the CEO of the company Hank Stalica, and for all developers willing to contribute to this open source project. Refer to Section 2 for a high level overview of how the application functions.
1.4	Product Scope
The sole purpose of this web application is to help CSU East Bay students have a more easy/comfortable college experience. Through this application, users can connect with one another, whether it’s for commerce needs, finding a roommate, find others in your classes or even learn about events within the community. Users would be required to have a valid CSUEastBay horizon email account to be able to register.

1.5	References

1.5.1 	https://nodejs.org/en/docs/
         		Official documentation for the backend of the application

1.5.2 	https://expressjs.com/en/4x/api.html
         		Official API reference for Node Js framework

1.5.3 	https://docs.mongodb.com/
         		Official documentation for the database of the application

1.5.4 	https://reactjs.org/docs/hello-world.html
        		Official documentation for the frontend of the application

1.5.5 	https://standards.ieee.org/findstds/standard/830-1998.html
         		IEEE recommended practice for software requirements specifications
2.	Overall Description
2.1	Product Perspective
This product would allow CSU East Bay Students to register an account, post, search for for-sale goods by other students, look for housing or potential roommates, and keep track of current unofficial events around the campus.

2.2	Product Functions
1.	Users would be able to register for an account with their horizon email.
2.	Users would be able to post or search for goods, housing, or campus event.
3.	Messaging system would enables the users to stay anonymous and keep their information private.
2.3	User Classes and Characteristics
The various user classes that might use this product:
1.	Registered users who are selling/buying books, electronic items, event tickets, or any other items.
2.	Registered users who are looking for roommate(s) or housing arrangement.
3.	Registered users who are looking for unofficial events happening on/off campus.
4.	Registered users looking to connect with others in the same classes as they are in.
5.	Registered users who are just browsing, not really looking for anything.

2.4	Operating Environment
This web application is browser-based and will be able to run on most internet browsers with internet connection and Javascript enabled, such as Internet Explorer, Firefox, Google Chrome, and Safari. 
2.5	Design and Implementation Constraints
The primary constraint our group has with this project is that some of us had no experience regarding web development, so we had to try to catch up with the rest of the group by watching tutorials and doing research on our own. 
2.6	User Documentation
Since this is a web application for CSU East Bay students, everyone is assumed to know how to register an account, logging in and out, and browsing/posting on a  website. As such there’s would be no user manual available from the developer team.
2.7	Assumptions and Dependencies
Since this web application requires an internet browser and a working internet connection, any changes apply to those factors would also change how our web application works and operates.
3.	External Interface Requirements
3.1	User Interfaces
This section will discuss the various user interfaces of the web application. One common component amongst all application user interfaces will be a navigation bar at the top of the screen that displays the product logo, and four links that provide access to the product features: Buy/Sell, Housing, ClassConnect and Events.



NOTE: Although some of the mockups below do not include ‘Events’ in the navigation bar, any actual prototypes will contain ‘Events.’

3.1.1 	Landing Page

This is the first page users see once they access the site. The first user interface describes pre user login; second user interface describes post user login. Refer to section 4.1 for more information.





3.1.2 Buy/Sell Feature

The buy/sell feature comprises of the user’s ability to browse items, and the ability to post an item. Each capability has unique user interfaces. Refer to section 4.3 for more information.

	3.1.2.1 Buy/Sell -> Browsing Items

	
	




	



















3.1.2.2 Buy/Sell -> Posting Item
	
	





3.1.3 Housing Feature

The housing feature comprises of the user’s ability to browse ads, and the ability to post an ad. Each capability has unique user interfaces. Refer to section 4.5 for more information.

	















3.1.3.1 Housing -> Browse Ads

	



	3.1.3.2 Housing -> Post an Ad

	

3.1.4 ClassConnect Feature

The ClassConnect feature comprises of the user’s ability to register themselves into a class, and the ability to browse through the people in their registered classes. Each capability has unique user interfaces. Refer to section 4.7 for more information.

	










3.1.4.1 ClassConnect -> Register

	





	3.1.4.2 ClassConnect -> View Classes
	
	




3.1.5 Messaging 
Refer to section 4.4 for more information.


3.1.6 Account Activity

Users have the ability to look at a log of their posts, which they may uploaded through any of the four features. Refer to section 4.8 for more information.




3.1.7 Events 

The Events feature comprises of the user’s ability to browse through events other users may have posted or the ability to post an event themselves. Each capability has unique user interfaces. Refer to section 4.9 for more information.







3.2	Hardware Interfaces
Pioneer Exchange is supported by all types of user devices. This includes computers/laptops, tablets and mobile smart phones.

Requirements for computers/laptops:
1.	Any web browser installed
2.	Internet connection with at least 4Mbps download speed, 1Mbps upload speed and 4ms ping
3.	Monitor
4.	Keyboard
5.	Mouse or trackpad
Requirements for tablets:
1.	Any web browser application installed
2.	Internet connection with at least 4Mbps download speed, 1Mbps upload speed and 4ms ping

Requirements for mobile smart phones:
1.	Any web browser application installed
2.	Internet connection with at least 4Mbps download speed, 1Mbps upload speed and 4ms ping
3.3	Software Interfaces
1.	Users must have an email with .csueastbay.edu domain (these are google email accounts with a customized domain) to be able to create an account
2.	Google Sign in API - allows users to create an account or login into existing account using their .csueastbay.edu emails
3.	Heroku - allows for deployment of web application to the internet and storage of web assets
4.	MongoDB - NoSQL database that allows for storage and synchronization of data between user and web application
3.4	Communications Interfaces
3.4.1 MongoDB

MongoDB is a NoSQL database that will be used to store user data. The Pioneer Exchange web application will interact with the MongoDB database, by querying specific information at the request of the user (depending on what they search for whilst accessing the various features.) User data being stored:
1.	Username and password
2.	Logs of item posts, housing ads, class registrations or event posts that users may upload

3.4.2 Heroku

Heroku will allow Pioneer Exchange to run and operate on the cloud, by configuring routes and distributing HTTP traffic

3.4.3 Google Sign in API

When a user attempts to login, Pioneer Exchange will request that the user grant access to data in their Google Account. When the user consents, Pioneer Exchange will request and receive credentials to access the Gmail API.
4.	System Features
4.1	Display Landing Page
4.1.1	Description 
Upon entering in the URL of the website, a static page should be visible to the user with a section available to register onto the website already at their disposal. 
4.1.2	Stimulus/Response Sequences
4.1.2.1 Stimulus: A user enters web address of the social/ecommerce platform in a web browser. 
4.1.2.2 Response: A home page is displayed with the link to register in the system within about 3.4-5 seconds.

4.1.3	Functional Requirements
[R4.1.3-1] A user of Pioneer Exchange should be able to see the link on the front page of the website. 
[R4.1.3-2] Users would require to have a functional keyboard and mouse in order to use the application. Once a user enters in the web address, a view should be taken to the front page with the following fields at the top of the navigation bar: 
Pioneer Exchange · Buy/Sell · Housing · Class Connect · Events 
[R4.1.3-3] A working image on the left hand side should be visible in the background. In the forefront of the picture should have a brief description about the site such as “Exclusive to the CSUEB community!”
[R4.1.3-4] On the right hand side, it should display an option to register for the site with a button that says ‘Sign in with Google’.
4.1.4 Priority: High
4.2	User Registration
4.2.1	Description 
Users of Pioneer Exchange should be able to register into the system.
4.2.2	Stimulus/Response Sequences
4.2.2.1Stimulus: A user clicks the ‘Sign in with Google’ link on the right hand side of Home page 
4.2.2.2 Response: A form is presented to the user with mandatory fields that is needed to be filled out and the button to ‘Submit’
4.2.2.3 Stimulus: A user fills the form and click ‘Submit’ button. 
4.2.2.4 Response: A message with the status (Success or Failure) is displayed. Upon successful request a user should be able to receive email notification with the welcome message and the steps as to how to authenticate their horizon email in order to use the site. 
4.2.2.5 Stimulus: A user connects with Google’s API in order to access the web application. 
4.2.2.6 Response:The user is now able to login and navigate the website
4.2.3	Functional Requirements
[R4.2.3-1] A user of Pioneer Exchange should be able to see the link to ‘Sign in with Google’ on the front page of the website. 
[R4.2.3-2] When a user clicks the link , a view should be taken to the form page with the following fields to fill out on the user’s end: 
· First name · Last name · Gender · Major · Email 
[R4.2.3-3] A user fills the form and selects link to ‘Submit’ s/he should be able to register in the system.
[R4.2.3-4] The user should enter their CSU East Bay horizon email into the Google API in order to authenticate account- authenticating should take no more than 5 seconds upon inputting horizon email (i.e username@horizon.csueastbay.edu) 
[R4.2.3-5] After successful registration a user should receive a welcome email from the system. 
4.2.4 Priority: High


4.3	Buy/Sell
	4.3.1	Description 
When navigating to the Buy/Sell page, users are given the options to search the items that they wish to buy and post an item that they wish to sell. They can also select an item type- can be textbooks, electronics, event tickets, or other. 
4.3.2	Stimulus/Response Sequences
4.3.2.1 Stimulus: A user hovers on the link ‘Buy/Sell’ on the Home Page navigation bar.
4.3.2.2 Response: The navigation bar drops down, giving two options: ‘Browse an item’ or ‘Post an item’.
4.3.2.3 Stimulus: (Browse an Item) A user clicks on the ‘Browse an item’ option 
4.3.2.4 Response: (Browse an Item) The home page routes to the Buy/Sell page where users will be able to view a ‘Search all items...’ and ‘select item type’ bar. 
4.3.2.5 Stimulus: A user enters in a desired item on the ‘Search all items…’ bar and hits ‘Enter’ on their keyboard or click the ‘Search’ button on the page.
4.3.2.6 Response: A list of similar items will display onto the screen with an image on left while price and title description on the right hand side.
4.3.2.5 Stimulus:(Select Item Type) A user clicks on a drop-down bar with different item types and select the one they want. Users are given the option to pick the item types that they want(i.e. textbooks, electronics, event tickets, or other).
4.3.2.6 Response: A list of similar items will display on the screen with an image on left while price and title description on the right hand side.
4.3.2.7 Stimulus: (Post an Item) A user hovers over the Buy/Sell Navbar and clicks on the ‘Post an Item’ dropdown view option.
4.3.2.8 Response: The Home page will route to a page that will have a bar display ‘What type of item are you selling?’ 
4.3.2.9 Stimulus: The user selects the item type they want to sell/post (options: textbook, event tickets, electronics, or other). 
4.3.2.10 Response: A page with some requirements will be asked of the user to fill out 
4.3.2.11 Stimulus: User fills in form and hits ‘Submit’
4.3.2.12 Response: The item is posted onto the Buy/Sell page.
4.3.3	Functional Requirements
[R4.3.3-1] A user of Pioneer Exchange should be able to navigate to another page specifically to buy or sell their items within 3 seconds 
[R4.3.3-2] Users would be able to input up to 300 characters into the search bar in order to search for the availability of listed items from other students. 
[R4.3.3-3] Users will also be given the option to select an item type-whether that may be textbooks, electronics, event tickets, or other. When they click a specific item type, they can be more specific. For example, if the user selects textbook, they can select a category (chemistry, computer science, english, etc.). The same thing will apply for Electronics. Users can select electronics and laptops if that’s what they specifically need. This is applicable for all item types. 
[R4.3.3-4] Upon posting an item a user would like to sell, they will be prompted to fill in some additional information. Each item type will vary. For example, for textbooks, users will be required to fill things in like subject, book title and author, desired price, upload a picture, and any additional comments they wish to add. For electronics, users can put what type it is (camera, laptop, etc.), what brand it is, desired price, upload a photo, and add any additional details (optional). 
cha
[R4.3.3-5] On the search results for buying an item, a working image on the left hand side should be visible, whereas the right hand side should show a title description and price. Additional to that, there should be a ‘Contact Seller’ button below (see sec. 4.4) 
4.3.4 Priority: High
4.4	Messaging
4.4.1	Description 
After searching for an item and user have found the items they wish to purchase from the buy/sell page, there is a ‘Contact Seller’ button. As well as this, when users click on a post on the housing page, there is a ‘Contact Poster’ button. In addition this, when users click on the ‘ClassConnect’ page, there is a ‘Connect’ button. Clicking any of these 3 buttons ‘Contact Seller,’ ‘Contact Poster’ or ‘Connect,’ users will be lead to the messaging page. This is a page with a text box where users can type in the message they want emailed to the other party’s (seller, housing ad poster, or registered classmate) email. The user doing this not create a direct email; Pioneer Exchange will take this message and handle the emailing part of the action. The receiving party will receive this message in the form of an email with the sender being Pioneer Exchange, and the subject line being ‘You have a new message!’ 
4.4.2	Stimulus/Response Sequences
	4.4.2.1 Stimulus: A user clicks on an item that they wish to buy in the Browse Items section of the Buy/Sell feature.
	4.4.2.2 Response:  A page will load with an image of just the item the user selected as well as       the item’s title, price, a short description that the seller have posted, and a ‘Contact Seller’ button.
4.4.2.3 Stimulus: A user clicks on the link ‘Contact Seller’ from the item page
4.4.2.4 Response: The link will open up a textbox that the user can input their message.
4.4.2.5 Stimulus: The user then hits ‘Send’ once constructing their message.
4.4.2.6 Response: The message of the user is sent to the seller via email. 
4.4.2.7 Stimulus: A user clicks on ‘Contact Poster’ button on the page of a housing post
4.4.2.8 Response: The link will open up a textbox that the user can input their message.
4.4.2.9 Stimulus: The user then hits ‘Send’ once constructing their message.
4.4.2.10 Response: The message of the user is sent to the seller via email.
4.4.2.11 Stimulus: A user clicks on ‘Connect’ button nexts to the name of the person they want to contact, on the ClassConnect page
4.4.2.12 Response: The link will open up a textbox that the user can input their message.
4.4.2.13 Stimulus: The user then hits ‘Send’ once constructing their message.
4.4.2.14 Response: The message of the user is sent to the seller via email.
4.4.3	Functional Requirements
[R4.4.3-1] A user of Pioneer Exchange should be able to view a textbox when clicking the ‘Contact Seller’ button on the buy/sell page after they’ve searched for their items. 
[R4.4.3-2] Users would be able to send the seller a direct message through the sellers provided email. Email will be the primary form of communication as all users are connected to their CSUEB email. 
4.4.4 Priority: High
4.5	Housing
4.5.1	Description
Users of the social/ecommerce platform is able to look through a variety of housing posts with roommates that are available as well as post an Ad of their own.  

4.5.2	Stimulus/Response Sequences

4.5.2.1 Stimulus: A user clicks(or hovers) on the link ‘Housing’ from the Home Page navigation bar.
4.5.2.2 Response: The navigation bar drops down, giving two options: ‘Browse ads’ or ‘Post an ad’.
4.5.2.3 Stimulus: (Browse ads) A user clicks on the ‘Browse ads’ option
4.5.2.4 Response: (Browse ads) The home page routes to the Housing page where users will be able to view housing ads that have previously been posted.
4.5.2.5 Stimulus: A user clicks prev, next, or a numbered button from the bottom of the page.
4.5.2.6 Response: The page routes to a different page with different housing ads the user can view. 
4.5.2.7 Stimulus: A user clicks on one of the housing ads from the current page.
4.5.2.8 Response: A larger picture of the house will appear as well as the details of the housing ad. Contact seller option will be available on this page (Reference section 4.4 for Contact Seller Response/Stimulus).
4.5.2.9 Stimulus: (Post an ad) A user clicks or hovers over the Housing Navbar and clicks on the ‘Post an ad’ option.
4.5.2.10 Response: The home page will route to a page that will have inputs to store the title, description, and picture of the apartment/house.
4.5.2.11 Stimulus: User fills out inputs, as well as uploads a photo and hits submit.
4.5.2.12 Response: New ad gets posted and page redirects to the page where all the housing ads are. Posted ad is appeared as the first ad on the page. 
4.5.3	Functional Requirements
[R4.5.3-1] A user of the social/ecommerce platform should be able to view different options of housing with their possible roommates 
[R4.5.3-2] Users would be able to send the seller a direct message 
4.5.4 Priority: High
4.6	Log Out
4.6.1	Description 
Any logged in user shall have a “Logout” button on any scene they can access, and when the button is pressed user’s logged out.
4.6.2	Stimulus/Response Sequences
4.6.2.1. Stimulus: “Logout” button is pressed.
4.6.2.2. Response: User is automatically logged out from system, and the scene is redirected to the “Home Page.”
4.6.3. Functional Requirements
[R4.6.3-1]  Every page the user will have the option to have a “Logout” button for them to click on.
4.6.4 Priority: High
4.7	Class Connect
4.7.1	Description 
Users are able to provide their major and be connected with students with similar major and    classes. Students that need help, but do not know anyone in the class will be able to connect with others through this feature. 

4.7.2	Stimulus/Response Sequences
4.7.2.1 Stimulus: A user clicks on the link ‘Class Connect’ from the navigation bar 
4.7.2.2 Response: The link will route to a page where it displays a message for ClassConnect’s purpose- along with a Register button at the bottom
4.7.2.3 Stimulus: User clicks the Register button
4.7.2.4 Response: User will be redirected to a page where they’ll see a scroll down bar with a variety of subjects and a box to enter in the course’s number as well as a bar that says ‘Add yourself to the list’.
4.7.2.5 Stimulus: User will select their subject and enter in course number- press ‘Add yourself to the list’
4.7.2.6 Response: After user enters details and clicks the action, they should see a message that states ‘Success’ 
4.7.2.7 Stimulus: User clicks view classes under the ClassConnect drop down bar
4.7.2.8 Response: User can view their classes that they’ve added ( maximum of 5 courses).
4.7.2.9 Stimulus: User clicks on the course they’ve registered.
4.7.2.10 Response: User can see other classmates who have registered and a ‘Connect’ button on the right hand side.
4.7.2.11 Stimulus: Users clicks on ‘Connect’ button.
4.7.2.12 Response: A text box appears with a send button at the bottom. 
4.7.2.13 Stimulus: User enters their message and hits send.
4.7.2.14 Response: The message is sent to the the other classmate’s via email.
4.7.3	Functional Requirements
[R4.7.3-1] Users should be able to view a page with a brief description of the ClassConnect’s purpose alongside a working register button that enables the user to sign up for their specific courses  
[R4.7.3-2] Users are only allowed to sign up to a maximum of 5 courses, otherwise it’ll prevent the user to continue signing up for another course. 
[R4.7.3-3] Users should experience a working bar with a wide variety of different subject type (i.e. mathematics, computer science, etc.) to select from. The user should be able to enter in a 4 digit course code that corresponds to the subject type. Upon adding the class, the users should be able to view what they have added.
[R4.7.3-4] Users can view their classes and have visibility of other classmates who have registered as well. From here users are allowed to message one another to connect, converse, and assist one another.
4.7.4 Priority: Medium 
4.8 Account Activity
4.8.1  Description
After the user signs in, their name appears on the top right corner of the website. When they click on their name, a page appears that shows a summary of all the posts they may have put up onto Pioneer Exchange via any of the four features: Buy/Sell, Housing, ClassConnect or Events. From here, users have the option to view any of their posts or delete any of them.
4.8.2	Stimulus/Response Sequences
4.8.2.1. Stimulus: User clicks on their name on the top right corner of the website.
4.8.2.2. Response: User is redirected to an ‘Activity’ page where they’re able to view all existing posts they’ve made for all features: Buy/Sell, Housing, ClassConnect connections, and events. Users will also have visibility of a ‘View’ or ‘Delete’ button on the right-hand side of each existing post/connection. 
4.8.2.3. Stimulus: User clicks ‘View’ on their post
4.8.2.4 Response: User is able to view the post that they’ve created.
4.8.2.5 Stimulus: User clicks ‘Delete’ on their post.
4.8.2.6. Response: The post that the User have created is then deleted from the website.
4.8.3. Functional Requirements
[R4.8.3-1]  User will have visibility of all items that they’ve posted from the ‘Buy/Sell’ feature. Within this scope, they should see a box outline surrounding all of their items posted. Each posted item will be formatted neatly into a row starting with the Item type on the left hand side. Moving next to the right, users should be able to view name of the item (i.e. textbook name, event name, item name), desired price, and a ‘View’/’Delete’ button. 
[R4.8.3-2] User will have visibility of all items that they’ve posted from the ‘Housing’ feature. Within this scope, they should see a box outline surrounding all of their items posted. Each posted item will be formatted neatly into a row with the Posting Title. User should be able to have the option to ‘View’ or ‘Delete’ their Posting Title. 
[R4.8.3-3] User will have visibility of all items that they’ve posted from the ‘ClassConnect’ feature. Within this scope, they should see a box outline surrounding all of their items posted. Each posted item will be formatted neatly into a row starting with the ‘Registered Class’ and number of classmates registered too. User should be able to have the option to ‘View’ or ‘Delete’ their class connections/registrations. 
[R4.8.3-4] User will have visibility of all items that they’ve posted from the ‘Event feature’. Within this scope, they should see a box outline surrounding all of their items posted. Each posted item will be formatted neatly into a row with the event name and date. User should be able to have the option to ‘View’ or ‘Delete’ their events. 
4.8.4 Priority: High
4.9 Events 
Description
The Events feature allows the user’s ability to browse through events other users may have posted or the ability to post an event themselves. When viewing events, users have the ability to sort by most recently added, earliest to latest (by date) or latest to earliest (by date). 

4.9.2	Stimulus/Response Sequences
4.9.2.1. Stimulus: User hovers over on ‘Event’ at the top of the navigation bar.
4.9.2.2. Response: Users can choose to ‘view events’ or ‘post an event’
4.9.2.3 Stimulus: User clicks on the ‘view events’ option.
4.9.2.4 Response: User is redirected to a page of event listings. 
4.9.2.5 Stimulus: User clicks on the ‘View Event’ button on the right hand side.
4.9.2.6 Response: User is able to view the event’s name, date, and a brief description. 
4.9.2.7 Stimulus: User is able to click ‘sort by’ and choose to sort by ‘Most recently added’
4.9.2.8 Response: The events load in the order they were posted, with the most recently added at the top
4.9.2.9 Stimulus: User is able to click ‘sort by’ and choose to sort by ‘Earliest to Latest’
4.9.2.10 Response: The events load in terms of the dates of the event. The event with the closest date to the date at the time of stimulus will be at the top.
4.9.2.11 Stimulus: User is able to click ‘sort by’ and choose to sort by ‘Latest to Earliest’
4.9.2.12 Response: The events load in terms of the dates of the event. The event with the furthest date to the date at the time of stimulus will be at the top.
4.9.2.13 Stimulus: User hovers over the ‘Event’ up top at the navigation bar 
4.9.2.14 Response: User can view the ‘post an event’ option.
4.9.2.15 Stimulus: User clicks the ‘post an event’ option.
4.9.2.16 Response: User is redirected to a page where they are able to fill out event information 
4.9.2.17 Stimulus: User fills out form and hits ‘Post Event’ 
4.9.2.18 Response: Event is posted to the event list.
4.9.3. Functional Requirements
[R4.9.3-1] When the user is routed to the Event page they should be able to see a listing of all the events that have been posted. Each individual event should be inside a box with the event name starting from the left, then the date and ‘View Event’ button moving towards the right. 
[R4.9.3-2] Upon clicking on the “View Event’ button, users should be able to see a picture of the event(optional), the name, the date, and a brief description of the event. 
[R4.9.3-3] When users are posting events, they are required to have a title, description and date. A picture would be an optional choice. Once user hits the ‘Post Event’ button, it is now visible on the ‘View Event’ option.
4.9.4 Priority: Low
5.	Other Nonfunctional Requirements
5.1	Performance Requirements
5.1.1	The Web Application will load and present data to a user within 3-5 seconds after logging in     85% of the time.
5.1.2	The Web Application will render up to date information 95% of the time.
5.1.3	Notification will be sent within 10-15 seconds 85%  of the time.
5.1.4	The server will respond to a request within 15 seconds 90% of the time.
5.1.5	A transaction between two users will take up to 20 seconds 85% of the time.
5.1.6	An email notification sent to a user regarding a transaction will take up to 10 seconds 95% of the time
5.2	Safety Requirements
5.2.1	The user will have the option to remove their account to Pioneer Exchange at any time. Once the request has been made, the user’s information will be deleted across all the databases within 48 hours of request. The process will ensure all of the user’s sensitive data to be properly deleted, and no data to be leaked.
5.2.2	As part of our commitment to privacy, we will not sell or otherwise provide any user’s personal information to unauthorized parties. The user’s email and phone number will be used strictly for verification purposes when initializing their account, and to be used to send notifications if and only if the user has explicitly decided to opt-in to in the notifications settings.

5.3	Security Requirements
5.3.1	Each user will have to have a California State University, East Bay student email address to have access to the web application. 

5.3.2	Any form of user-to-user communication within the web application, there will be a note stating that the website does not encourage any outgoing messages to contain any personal information or passwords to be shared.
5.4	Software Quality Attributes
Team Delta will provide development support up until June 30th, 2018. Granted, if there is a need for additional past the date, Team Delta will re-evaluate whether to move forward with support. Please refer to sections 2.4 and 2.5 for supported versions of software. 
5.5	Business Rules
5.5.1	All transactions between two users are final. 
5.5.2	The seller has the right to refuse any offer they deem is unfit for the product they are selling.
5.5.3	The seller can change their product’s description if-and-only-if they are not finalizing a current transaction.
6.	Other Requirements
Appendix A: Glossary
API : Application Programming Interface. Tools used to develop software.
App : Short for an application.
Checkbox : A clickable box used to indicate yes or no.
Chrome : A web browser developed by Google.
ClassConnect : A feature in PioneerExchange that lets students connect with each other.
Component : A part or element of a larger whole, in this case our website.
Database : A structured set of data held in a computer.
Developer : Someone who develops code.
Domain : The main address of a web page.
Firefox : A free and open-source web browser developed by Mozilla Foundation.
Heroku : A cloud platform that lets companies build, deliver, monitor and scale apps.
Horizon : An email network specifically for CSU East Bay students.
Internet : A global computer network.
Internet Explorer : A web browser designed by Microsoft.
Landing Page : The section of a website accessed by clicking a hyperlink on another web page, typically the website's home page.
MongoDB : A document-oriented database.
Navigation Bar : A section of a graphical user interface intended to aid visitors in accessing information.
NoSQL : Non-SQL or Not Only SQL, is a database design approach.
Notification : A message sent to a user, notifying them of a specific event/action that occurred.
Opt-In : Express permission by a customer, or a recipient of a mail, email, or other direct message to allow a marketer to send a merchandise, information, or more messages.
Registered User : A CSU East Bay student who has signed up for an account.
Password : A user generated string used for logging into the website.
Safari : A web browser developed by Apple.
Social Network : A dedicated website or other application that enables users to communicate with each other by posting information, comments, messages, images, etc.
Q&A : Questions and answers.
Server : A computer or computer program that manages access to a centralized resource or service in a network.
SQL : A Structured Query Language used to communicate with databases.
Web Application : A client–server computer program which the client (including the user interface and client-side logic) runs in a web browser.
Web Browser : An application used to view web pages.
Web Page : A hypertext document connected to the internet.
Wireframing : A way to design a website service at the structural level.
Upload : To transfer data from one computer/machine to another.
URL : The address of a web page.
User : Anyone who uses the web application.
User Interface : (UI) The means by which the user and a computer system interact, in particular the use of input devices and software.


