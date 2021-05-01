<!-- Place this tag where you want the button to render. -->
<a class="github-button" href="https://github.com/ntkme" aria-label="Follow @ntkme on GitHub">Follow @ntkme</a>


# Bilkent University

# Senior Design Project
# A-Tab: Artificial Tabldot
# Specifications Report
Gürkan Gür, Arda Kaan Gültekin,Mahir Efe Macit,Subhan Ibrahimli

Supervisor: Halit Altay Güvenir

Jury Members: Dr. Çiğdem Gündüz Demir, Dr. Can Alkan

Specifications Report
October 12 2020
This report is submitted to the Department of Computer Engineering of Bilkent University in partial fulfillment of the requirements of the Senior Design Project course CS491/2.

## 1.Introduction

In today's world, time inefficiency is a common issue everyone faces. This problem can occur at any time in daily life. Therefore, this is more important than previous times. Anyone can face this problem while driving, working or even when the on is trying to eat outside. Although time efficiency is a common problem, the solutions of these difficulties are neither trivial nor common. To solve the time inefficiency, the root of the problem should be examined.

In cafeterias, restaurants and pubs, people buy meals through engaging with cashiers or sellers. The process of ordering and paying for meals can possibly be stressful and tiring when the cafeteria is overloaded. Reducing the time of ordering and paying processes can make a great save in terms of time efficiency. 

With the A-Tab project, our aim is to reduce the time process of asking the cost of the meal. A-Tab aims to give the cost of the meal that is ordered by the customer without any interaction with the cashiers by taking the photo of the meal. The project is significant in terms of the innovative tools that will be used through accomplishing its aims and can be improved in the future to accomplish other various tasks, like other image analysing applications. 

In this report, there will be firstly described the A-Tab project. After that, constraints of the project will be examined under the appropriate sections. Then, we will analyze professional and ethical issues that may arise in the process. After those, requirements of the project will be given under appropriate sections grouped under functional and non-functional requirements.

### 1.1 Description
The project aims to deal with the time inefficiency problem that is faced in mostly cafeterias and restaurants. The proposed solution helps the customers to see the costs of the meals they ordered by taking a photo of the meals. 

The application that the project will create will take the images as inputs. It will analyse the image of the meals. We designed a few subsections that will accomplish that purpose. Each subsection is classified by different algorithms. 

The first algorithm is designated for segmentation of the image: 
	- Non-meal and meal objects will be seperated. Non-meal objects are going to be disregarded. 
	- If they are different, meal objects will be seperated and changed into something that is easier to analyze. Then they will be sent to the second algorithm. 

The second algorithm will analyse the meals: 
	- Object classification will be done by the second algorithm. 

The third algorithm will make object matching: 
	- The meal that is classified will be checked through a large database of classes. A matched class will give the cost as return. After the third algorithm, the cost of the meals that are given to the application will be returned. 

We expect to face three main problems that we described above, segmentation, object classification and object matching. We are planning to use Machine Learning algorithms, some of them will be 4 taken from open sources, some of which we will create ourselves. ML uses statistical reasoning to find approximate solutions for tackling the above difficulties. [1] Through designing the analysis and high-level design report, we can discover and use new ways of solving the problems above. For example, for increased accuracy, Image classification can be done using CNN(Convolutional neural network)[2] In the same way, we can find and choose different ways to accomplish the main task of the project, like Data Labeling and RCNN. 

The project’s first concern is to give reliable results in an efficient way, we expect the application to give the desired results in less than 20 seconds. We are not concerned about making a usable program with a good interface, as our first concern is to make it extensible and reliable. We are primarily planning to make the application to work in Personal Computers, and extend it to work on android and ios operating systems.



### 1.2 Constraints
### 1.2.1 Economic
A-Tab would be a great opportunity for food places especially. It will prevent the economic loss of miscalculations on the payment phase and also it will try to minimize the queues at crowded times such as breakfast,lunch and dinner. Moreover the setup of the A-Tab is very simple, only need is a basic computer and camera with the internet connection.
### 	1.2.3 Implementation Constraints
-Our project will be in a desktop application(where the image data is analyzed) and a mobile application(where the user takes the photo and sends to the system). 
-We will be using gitHub and intelliJ to work concurrently.
### 	1.2.4 Ethical
Code of ethics will be applied and followed in the project development stages.
Any user data or information will not be shared or used if the user did not give us permission.
### 	1.2.5 Health and Safety
This is the constraint which A-Tab can benefit a lot especially in the pandemic era. It will reduce the addition and payment times crucially and also tries to minimize the interaction time between customer and cashier. Because of reducing the time queues won't exist or not too long like the classical payment detection methods.
### 	1.2.6 Manufacturability
This will not be a major concern since we are not planning to develop an electronic device. Our project is a software based program.
### 	1.2.7 Sustainability
The main concern about this project will be sustainability. Since, if it is not sustainable it will not be a proper solution. Since, the program only uses the photo which the user took(meal). It will be sustainable.
	
### 1.3 Ethical Issues
Since the image will be obtained from the user of A-Tab(User will take the photo), this may arise a problem in terms of getting the users data. However, users will be acknowledged that only the data of the photo will be used. To eliminate the problem of ethics we will follow and apply the IEEE Ethical Codes in our project. We will not gather any data if the users don’t give permission to do so. Other than that if any open source code is used it will be handled properly.
## 2.Requirements
### 2.1 Functional Requirements
### 2.1.1 Setup Requirements
Setup should be appropriate for efficient use of A-Tab. Camera should be located on the top angle and has clear vision of the tray and also has clear vision of plates. There should be a proper location for putting the tray for A-Tab scan, therefore the program should work efficiently. Camera distance also should be adjusted according to the size of the tray.
### 2.1.2 Server/DataBase Requirements
Program should be connected to Server continuously to calculate the similarity of the scanned plates and after that decide the kind of the food. If Similarity ratio is high however, the program cannot link the scanned object to the objects in the DataBase, it should take the object to the DataBase.
### 2.2 Non-Functional Requirements
### 2.2.1	Extensibility
This will be in our focus since our project can be developed and used in a significant number of places. Our view of handling it will help the project to be developed in the later stages(after the project is done). There will always be a better solution,interface. So we are trying to provide a project which is extensible.
### 2.2.2 Reliability
The photos will be sent through a mobile app to the desktop application. The results will be based on the photo taken.
### 2.2.3 Efficiency
Our aim is to give the results of the photo to user in less than 20 seconds.
### 2.2.4 Scalability
Service we are providing in any restaurant will not be affected by the number of customers or any other restaurant which are using the same application.
Our system will handle multiple images from different users simultaneously.

## 3.References
[1] “Machine Learning in Image Analysis - Theory and Practice.” Machine Learning in Image Analysis - Theory and Practice | Zuse Institute Berlin (ZIB), www.zib.de/MLIA. 
[2] Infrrd. “Image Processing With Deep Learning- A Quick Start Guide.” Medium, Becoming Human: Artificial Intelligence Magazine, 25 Aug. 2019, becominghuman.ai/image-processing-with-deep-learning-a-quick-start-guide-38e166340200. 


# Bilkent University
# Senior Design Project
# A-Tab: Artificial Tabldot
# Analysis Report

Gürkan Gür, Arda Kaan Gültekin, Mahir Efe Macit, Subhan Ibrahimli

Supervisor: Halil Altay Güvenir

Jury Members: Dr. Çiğdem Gündüz Demir, Dr. Can Alkan

# Analysis Report
November 21 2020

This report is submitted to the Department of Computer Engineering of Bilkent University in partial fulfillment of the requirements of the Senior Design Project course CS491/2

# Contents 

Contents	2

2.2. Functional Requirements	5

2.2.1 Food/Object Detection	5

2.2.2 Server/Database Requirements	5

2.2.3 Setup Requirements	5

2.3. Non-Functional Requirements	6

2.3.1 Extensibility	6

2.3.2 Efficiency	6

2.3.3 Scalability	6

2.3.4 Usability and Accessibility	7

2.3.5 Error Handling	7

2.3.6 Capacity	7

2.3.7 Maintainability	7

2.3.8 Reliability	7

2.4 Pseudo Requirements	8

2.5. System Models	9

2.5.1. Scenarios	9

2.5.1.1. Scenario 1: Download and Install	9

2.5.1.2. Scenario 2: Register	9

2.5.1.3 Scenario 3: Login	9

2.5.1.4 Scenario 4: Pay	10

2.5.1.5 Scenario 5: Pricing	11

2.5.1.6 Scenario 6: Take Photo	11

2.5.1.7 Scenario 7: Log Out	11

2.5.2 Use Case Model	12

2.5.3 Object and Class Model	13

2.5.4 Dynamic Models	13

2.5.4.1 Sequence Diagrams	13

2.5.4.2 Activity Diagram	16

2.5.5 User Interface - Navigational Paths and Screen Mock-ups	17

3.1. Consideration of Various Factors in Engineering Design	23

3.1.1 Public Health	23

3.1.2 Public Safety	23

3.1.3 Public Welfare	23

3.1.4 Global Factors	24

3.1.5 Cultural Factors	24

3.1.6 Social Factors	24

3.1.7 Environmental Factors	24

3.1.8 Economic Factors	24

3.2. Risks and Alternatives	25

3.3. Project Plan	27

3.4. Ensuring Proper Teamwork	30

3.5. Ethics and Professional Responsibilities	30

3.6. Planning for New Knowledge and Learning Strategies	31










# 1.Introduction 
As we are moving into a new era, technology has begun to be considered as a convenient and useful tool for communication, interaction between individuals. Our team members make an effort to gain knowledge from their field and apply them in new projects. A-Tab can be considered one of those projects where the latest knowledge is combined to make an innovative tool for daily life usage. 

In cafeterias, restaurants, and pubs, people buy meals by engaging with cashiers or sellers. The process of ordering and paying for meals can possibly be annoying and tiring when the cafeteria is overloaded. Reducing the time of ordering and paying processes can make a great save in terms of time efficiency.

The goal of the A-Tab project is to reduce the time process of asking for the cost of the meal and payment. A-Tab aims to give the cost of the meal that is ordered by the customer without any interaction with the cashiers by taking a photo of the meal. Once the project is released for a usage, it can be applied in restaurants and cafes, and used by cashiers.

This report is intended to analyze the various points of the project including technical perspectives, requirements, system models, learning strategies etc. In the process of the project development, team members have been trying to find optimal solutions for the specified problem and evaluate those solutions according to the various factors in engineering design.


# 2. Proposed System
# 2.2. Functional Requirements
# 2.2.1 Food/Object Detection
A-Tab should process the taken photo from the camera and identify the food and non-food objects accordingly.
A-Tab should understand and determine the food correctly and give the price of it.
If A-Tab sees a non-food object it should determine that it is not food and it should not give a price to it.
If there is no food in the taken image, the app should understand it and give an error message to the user.
If the app detects the photo is taken in a wrong position(which means 180 degrees opposite or 90 degrees to left or right). It should convert the image to optimum position where it can reach the correct outputs.
If the food is not detected due to brightness,contrast  or sharpness of the taken image it should rearrange these attributes of the image.
If there are more than one food in the taken photo the app should give the overall price to the system.


# 2.2.2 Server/Database Requirements
A-Tab should be connected to the server continuously to calculate the similarity of the scanned images and after that it should decide the kind of food number of foods in the plate. If the similarity ratio is high however, the program can not link the scanned object to the objects in the Database, it should take the object to the Database.
# 2.2.3 Setup Requirements
Setup should be appropriate for efficient use of A-Tab. Although the image can be played onto in terms of brightness and position of the photo(as if food is upside down or laying 90 degrees to the left or right). In order to minimize the problems that we might face, the camera should be located on the top angle and has clear vision of the tray and also has clear vision of plate(s). There should be a proper location for putting the tray for A-Tab scan, therefore the program should work efficiently. Camera distance also should be adjusted according to the size of the tray.
# 2.3. Non-Functional Requirements
# 2.3.1 Extensibility
This will be our main focus since our project can be developed and used in a significant number of places. Our view of handling it will help the project to be developed in the later stages(after the project is done). There will always be a better or faster solution and the interface of a program can always be improved. So the project should be extensible.
# 2.3.2 Efficiency
A-Tab application should give the result of the taken image and process it in less than 20 seconds in order to be time efficient.
Time spent in the restaurant line should be deduced in order to have a time efficient project.
The communication between the database and the program should be minimal in terms of time to be a time efficient program.
# 2.3.3 Scalability
The A-Tab program is not just for a specific restaurant, so the database and  system should work concurrently with many restaurants and the app should not be affected by the number of customers or the number of restaurants using it.
It should handle multiple images from different users simultaneously.
# 2.3.4 Usability and Accessibility
The system should be user friendly. Although processing an image is a hard process. The program should be user-friendly and easily used by users.
It should be clear when the program should interact with the user whether a photo could be processed or not.
The application should be free however, to run the application the program will need an additional camera to take the photos of the food.
It should be downloaded for both customer and restaurant. Restaurant will download its Desktop version and the customer will download its mobile version.
# 2.3.5 Error Handling
Errors and bugs should be noticed as soon as possible. Expected errors are identification problems and pricing problems. In case of identification errors unidentified objects should be added to the database. Pricing problems should be handled in the database also. Only way to overcome these errors is software changes, because we cannot show an  error message especially for unexpected conditions. However, for identification, the object frame will appear on the screen.
# 2.3.6 Capacity
In terms of capacity, the server should have appropriate storage for both images and prices. For an ordinary restaurant image storage should be approximately 50 and price is also the same.
# 2.3.7 Maintainability
In terms of arrangements and changings in datasets for one restaurant, only the specified restaurants dataset should be changed. Moreover also the changes in the backup side of the project should not affect the whole algorithm to maintain the modularity of the project. 
# 2.3.8 Reliability
The system should guarantee the privacy of the datasets of the restaurants and make the calculations correctly. In case of connection loss the system must give a warning message to the cashier to stop the process, because this situation can create conflicts and lead to calculation mistakes. Moreover there will be no access from interface to the server side to ensure the privacy of the datas.
# 2.4 Pseudo Requirements
For version control git will be used. A-Tab will be developed for desktop computers. Object Oriented programming paradigm is chosen for the development of the project External libraries and frameworks will be used for object detection and processing A-Tab requires internet connection to reach the database for both images and prices. Rest API will be used for server connections.Server implementation will be handled in C#. Microsoft Visual Studio will be used as an IDE for this implementation. Servers will be updated according to addings and changings in menus. More libraries and frameworks can be added to projects in case of some situations and improvements. Privacy and security for server connection will be provided for the safety of datasets. During implementation demos will be tested by parts, such as identification of single objects, single price, after that other situations Demos will be handled individually, after that restaurant testing can be done. According to feedback and errors, bugs and mistakes will be handled, these errors might affect the fundamentals of the algorithm. Licenses for third-party APIs,libraries and IDEs will be controlled before implementation. Free and open-source resources will be used as much as possible English Language will be used for the userface.
 


	
	

# 2.5. System Models
# 2.5.1. Scenarios
# 2.5.1.1. Scenario 1: Download and Install
Use Case: Install 
Actors: Customer,Restaurant ( Users)
Entry Condition(s): From the developers site,both the customer and restaurant are able to download and install the application. 
Exit Condition(s): When install process is completed 
Flow of Events:
1. Users will download and install the application from the developers site. 
2. Users accept the permissions and confirm the install.
3. Most of the process is handled by OS itself.
# 2.5.1.2. Scenario 2: Register
Use Case: Register
Actors : Restaurant 
Entry Condition(s) : When the register button in the main menu is clicked
Exit Condition(s) : When the registration process is complete. Or the back button is clicked.
Flow Of Events :
User opens the mobile app
Register button in the main menu is clicked.
Username is determined.
Password is determined and written into the box required.
Apply button is clicked.
Failed Flow Of Events : 
Register button in the main menu is clicked.
Back button in the register menu is clicked.
# 2.5.1.3 Scenario 3: Login
 Use Case: Login
 Actors : Restaurant 
 Entry Condition(s): 
1.From the main menu the sign in button is clicked. 
2.No users already logged in into the device.
Exit Condition(s): Login is done successfully.
Flow of Events:
User opens the mobile app
User clicks on the login button in the main menu.
User is prompted with a username and password.
User will provide those fields
User will click onto the login button.
Failed Flow of Events
Wrong username or password is provided by the user.
Required fields are blank.
User clicks the back button.
# 2.5.1.4 Scenario 4: Pay
Use Case: Pay
Actors: Customer
Entry Condition(s): The photo of the food is taken and the customer pressed the pay button in the main menu. Customer has to be logged in.
Exit Condition(s): Payment is done successfully.
Flow Of Events: 
The image of the food is taken by the customer or restaurant.
The pricing is done according to the photo.
Customer clicked the payment button.
The money is transferred from customer to restaurant.
The application redirects itself to the main menu.
Failed Flow of Events
Customer does not have enough balance in his account.
Customer clicks back button.
The taken image does not have food in it.
A problem occurred in the bank during money transfer.
# 2.5.1.5 Scenario 5: Pricing
Use Case: Pricing
Actors: Restaurant
Entry Condition(s): Restaurant has to be logged in. Restaurant clicked on the pricing button.
Exit Condition(s):	Restaurant has closed the application.	
Flow Of Events:	
1. Restaurant takes the photo off the meal or gives an existing photo to the application.
2. Photo is analysed in the application. Application displays an empty box for the user to fill in.
3. Restaurant fills the box with the price.
4. Application adds the meal to the dataset
# 2.5.1.6 Scenario 6: Take Photo
Use Case: Take Photo
Actors: Restaurant, Customer
Entry Condition(s): One of the user types clicks the take a photo button in the main menu.
Exit Condition(s): User has to be logged in to an account. The button has to be clicked.
Flow Of Events:
One of the user types clicks the button.
Caption button is clicked to take the photo.
User can retake the photo if he/she wants.
Application redirects itself to main menu
Failed Flow of Events:
      1.User clicks on the back button.
# 2.5.1.7 Scenario 7: Log Out
Use Case: Log Out
Actors: Restaurant
Entry Condition(s): User clicks on log out button.
Flow Of Events: 
User clicks on the logout button.
Application quits from terminating for the current user and displays the main menu.


# 2.5.2 Use Case Model



# 2.5.3 Object and Class Model


For good sized picture: https://i.hizliresim.com/uMJexi.png



# 2.5.4 Dynamic Models
	# 	2.5.4.1 Sequence Diagrams
		Sequence Diagram #1: Program analysis the food which the customer took:
		
							Figure xx. Customer-A-Tab Sequence Diagram
		For good sized picture: https://i.hizliresim.com/DVvtf5.png
Customer clicks start on the screen. A-Tab opens the camera, and the customer takes a picture of the food. A-tab checks the database for the picture, if it does not exist, the data controller returns false and the main controller starts the visual analyser. Visual Analyser separates the image components and analyses the image. Then the main controller sends the analysed images to the data controller and the data controller checks the prices of the images. The main controller gets the prices from the data controller and displays it through the layout manager.

         Sequence Diagram #2: Program analysis the food which the restaurant enters:

							Figure xx. Restaurant-A-Tab Sequence Diagram
		For good sized picture: https://i.hizliresim.com/Lw7VVl.png
Restaurant clicks start on the screen. A-Tab opens the camera, and the restaurant takes a picture of the foods. The A-tab checks the database for the picture, if it does not exist, the data controller returns false and the main controller starts the visual analyser. Visual Analyser separates the image components and analyses the image. Then the main controller sends the analysed images to the data controller and gets price information from the restaurant through the layout manager. Then the data controller sets the price for the given image.

         Sequence Diagram #3: Customer pays for the foods he ordered:

							Figure xx. Payment Sequence Diagram


After processing of the images, customer clicks pay now. A-tab asks for payment information and the customer writes the payment information. A-tab transfers money from the user to the restaurant and displays the bill for the order to the customer.
		# 2.5.4.2 Activity Diagram


					Figure xx. Activity diagram




# 2.5.5 User Interface - Navigational Paths and Screen Mock-ups
	Register Screen

	Login Screen
This is our basic login screen which you can both have a new account if you click on register screen or you can login to the application





Main Screen

After the login process is done successfully there are 3 main pages you can go to settings screen,payment screen and identification screen. And the log out button navigates to the login screen.









Identification Screen

This screen is where our algorithms work where the photo is taken. Taken photo is send to the database.


	


Setting screen will allow users to allow both internet connection and camera usage from the menu.
# 3. Other Analysis Elements

# 3.1. Consideration of Various Factors in Engineering Design
In the development process of A-Tab we observed that application would have various effects on different topics.
# 3.1.1 Public Health
A-Tab would have a great impact on public health. Firstly, it will control the queue population crucially, in other words it will prevent the overpopulated queues thanks to the shortened payment calculation time. Thanks to this ability people will secure their social distance with others. In this pandemic era it could affect the Covid-19 spread possibilities. Moreover it will also prevent the spread of other diseases such as, cold, flu and influenza. Cashiers can also be involved in this procedure. They will also secure their social distance because they wont move or lean forward to the customers table. There is also the possibility that thanks to A-Tab people probably would use contactless payment systems and it would decrease the exchange of coins or cash money. This situation will contribute to preserving hygiene.
# 3.1.2 Public Safety
A-Tab won't have software that will affect the safety. All the information and datasets would be secured in the server essentially. Datasets or customer information will not be shared to the third party applications or something else. However statistics of meals can be shared to the restaurant to enhance their sales or finding alternative solutions.
# 3.1.3 Public Welfare
A-Tab would affect welfare in a good way. It will prevent the calculation mistakes. Therefore both customers and restaurants will benefit from them. Customers won't pay more or less and restaurants won't earn more or less.
# 3.1.4 Global Factors
A-Tab is basically a language free application,however we will use English which is a worldwide known language as an optional language. Application could be used in every country because databases can be arranged according to the known meals.
# 3.1.5 Cultural Factors
For a determined restaurant dataset is specified and they are mostly culture based sets. However, in some cultures foods cannot be separated easily and cannot be classified basically. To prevent the possible mistakes precautions can be taken such as more detailed identification systems.
# 3.1.6 Social Factors
There is not a direct link between A-Tab and social factors. However, all the personal information and criterias can be identified as social factors. A-Tab can be used by any person from any country and any age. But on the other hand, especially people who use restaurants which work as a tabldot profits from A-Tab. For example in Bilkent University there are plenty of cafes and restaurants that work in this system and also people who work in plazas can profit from A-Tab. 
# 3.1.7 Environmental Factors
Since, the application will consist of a camera and back-end code, the environment will not be harmed during the process.
# 3.1.8 Economic Factors
A-Tab will probably increase the sales of restaurants because it will facilitate the paying process and the queue waiting times. Moreover A-Tab does not require any extra equipment and it will be free application. Only need is the basic camera setup and camera feature is now available in all the computers and mobile phones.  


Effect Level
Effect
Public Health
8
It will reduce the contact between people since it will reduce the time spent in queue
Public Safety
7
Private information of the users will not be distributed to any third party company
Public Welfare
2
Appropriate pricing
Global Factors
2
Applicable in any country
Cultural Factors
4
Culture Based sets are used
Environmental Factors
0
None
Economic Factors
5
Increasing the number of sales by reducing the queue length and time
Social Factors
4
Can be used by anyone in terms of age,country

# 3.2. Risks and Alternatives
A-Tab has several implementation risks that can affect the development and using process. We have to consider these risks and should overcome these possible problems with B plans.

1- Setup Problems
Setup should be appropriate for efficient use of A-Tab. Camera should be located on the top angle and has clear vision of the tray and also has clear vision of plates. There should be a proper location for putting the tray for A-Tab scan, therefore the program should work efficiently. Camera distance also should be adjusted according to the size of the tray. To overcome some setup problems we can try to enhance the analyzing algorithm. Moreover different angle perspectives can be used in the application to identify easily.
2- Image Processing Problems
For most of the foods in any culture spices and sauces are added to foods to make them more tasty. However these additions could change the look of the foods crucially. Therefore it could affect the identification process of the A-Tab. In order to prevent this problem we have two solutions. Firstly this spice and sauce process can be done after identification and payment process, if it is done in this way A-Tab will not require any change in the development phase. Secondly foods can be saved to the database with these addings, but it will require a bigger database and could not handle the identification problems.

3- Unidentified Food
Unidentified food is the biggest problem for the A-Tab. To overcome this problem the database should be improved in any change in the menu. Restaurants should notify us to add new food to the database or some identification algorithm can be developed for the restaurant to make their addition without our help.

4- Server problems
Server connection should be stable for the A-Tab identification process. If internet connection would be lost, the identification process cannot be done. To overcome this problem direct ethernet connection can be preferable. Moreover, more recent server technologies can be used also.

5- Workshare problems
We need to share the work equally between the teammates to keep the motivation high and affect the developing process in good ways. Any conflicts can damage the project process, therefore we are making our decisions together. Since the topic choice is a new section for all of us we need to make sure everybody collaborates in that.



Likelihood
Effect on Project
Plan B Summary
Problem during setup
Medium
Images don't work properly
Enhancing analyzing algorithm
Image Processing Problems
Medium
Image could not be processed due to high complexity
Bigger database will be used but sacrifice will be made in terms of time
Unidentified Food
Medium
Program will not work
Additional changes in database specifically for restaurant
Server Problems
Low
Not having proper server connection
Server technology will be changed.
Work Share
Very Low
Slows down the process
Making decisions together

# 3.3. Project Plan
Proper project planning is the key procedure. We try to arrange meetings recently and we have a WhatsApp group to keep in touch. Since we are in the pandemic era we arrange our group meetings in Zoom and Discord platforms. Up to present we prepared our project specification report, builded our website and delivered our analysis report. We determined our project plan to finish the project in a determined schedule.
1- Work on Machine Learning and Image Processing Libraries.
2- Prepare a proper demo until the last day of the semester. Firstly we will try to identify basic objects such as bananas or apples.
3- Deliver High-Level Design Report.
4- Need to improve the algorithm for multiple objects.
5- Improve our database and build the connection between server and application.
6- Enhance the demo.
7- Deliver Low-Level Report.
8- Improve the structure and user interface.
9- Optimize the demo and try to make it identify the whole tray.
10- Deliver the Final Report.
	
Based on these goals we divided the overall project into work packages. We tried to divide the project into equal parts and tried to balance the workshare between us. Each workshare has a leader and all the other group members involved in all work packages.

These work packages are for the first semester only. We will have different objectives and milestones in the next semester.
WP1: Analysis of the Project
Start Date: 25.09.2020
End Date: 21.11.2020
Leader: Mahir Efe Macit
Members Involved : Subhan Ibrahimli, Arda Kaan Gültekin, Gürkan Gür
Objective(s): Main focus of this work progress table is to fulfill the requirements of the project and various other factors that can affect and change the project design.As A-Tab group we will try to manage all the specifications and the factors as a team. Importance of this work progress is since it is our first deliverable and these will be a main stone of our project. These will lead the way to a good project at the end.
Milestone(s):
Meeting as a group : As we discussed we will hold meetings to fulfill the requirements and to be on the same page as a group.
Specification Report : Determining specifications and requirements of the project
Analysis Report : Determining object models, developing the structure of the project and UI interface.
WP2: Designing the Project
Start Date: 23.11.2020
End Date: 27.12.2020
Leader: Gürkan Gür
Members Involved: Subhan Ibrahimli, Arda Kaan Gültekin , Mahir Efe Macit
Objective(s): Main focus of this phase is to start high level designing of the project. After the analysis and high level design of the project. This will lead to the high level design deliverable. We will focus on UI and we will consider what we have done in analysis so far.
Members Involved: Subhan Ibrahimli, Arda Kaan Gültekin , Mahir Efe Macit
Milestone(s):
Check Analysis Part: We will consider what we have done in analysis part and we will add new parts if it is necessary.
High Level Design : We will define our design goal during this design. We will divide the part accordingly.
Low Level Design: This process will be used to design our data structures and design the data structures according to our needs.

WP3: Testing
Start Date: 09.04.2021
End Date: 17.05.2021
Leader: Arda Kaan Gültekin
Objective(s): This will be our last part in the project after the development stage is done. We will test whether our program can detect the food and nonfood object when the image is given. If any error occurs during the testing phase we will try to eliminate the errors by changing the necessary parts of our application.
Milestone(s):
This is the last step of the project.Our application will be delivered after this step.
Members Involved: Subhan Ibrahimli, Gürkan Gür , Mahir Efe Macit

WP4: Development
Start Date: 23.11.2020
End Date: 09.04.2021
Leader: Subhan Ibrahimli
Members Involved: Arda Kaan Gültekin,Gürkan Gür, Mahir Efe Macit
Objective(s): We will create our structures and processes in this step. This part will include having image libraries and using them to detect food and objects and separate them.
Milestone(s):
Camera Positioning: We will try to identify the best possible location for the camera to place in the restaurant. We will try to find the mathematics behind it.
Object/Food Detection: We will try to implement the program which is to detect the objects first and then to recognize the food and price it accordingly.
Training Dataset: If we can not find a proper dataset for food. We will be training our own dataset to test it.


# 3.4. Ensuring Proper Teamwork
We tried to divide the A-Tab developing process into equal work packages. Each work package has a leader and all the group members involved in each process in order to encourage efficiency and team chemistry. In work packages, the group leader determines the work process,however everybody has the right to make changes in the schedule. We are taking decisions together during our meetings. In case of emergency situations or some events one or some of us might not help the project. In those scenarios other members can handle their work share and for those visa versa. Moreover if one of the group members is done, the member will help others work. A-Tab project has a private GitHub repository to keep the codes safe and proper. Commitments will be kept in the repository and commitments are available for only team members. 
	
# 3.5. Ethics and Professional Responsibilities
A-Tab requires a basic register and login system. Personal information is not required to access the system. However, datasets will be private for the restaurant owners with their prices. In order to not harm the competition between restaurants and keep their statistics private, we will not share these data with third-parties. Scanning datas will not be recorded, therefore customers can be sure about their privacy. Furthermore we will try to use softwares and libraries which are approved and have copyright rules.

# 3.6. Planning for New Knowledge and Learning Strategies
For new knowledge and learning strategies, A-Tab requires detailed knowledge for various disciplines from computer science. Our learning strategy mainly focuses on reading articles and watching tutorial videos about object detection especially. Moreover some group members taking courses about artificial intelligence and image processing, we believe that these courses will be helpful during the development of the A-Tab project. For development we need to use some Python libraries such as Tensorflow and Pytorch,etc. We will make research about those libraries and try to enhance our Python knowledge.



