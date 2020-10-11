## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/grkngs/CS491-A-tab/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/grkngs/CS491-A-tab/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.


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

In today's world time inefficiency is a common problem everyone faces. This common problem can occur at any time in your daily life. Therefore this rising problem is more important than before. You can face this problem while you’re driving or working or even when you’re trying to eat outside. Although time efficiency is a common problem, the solutions of  these difficulties are neither trivial nor common. So, in order to solve the time inefficiency problem the root of the problem should be examined.
In cafeterias, restaurants, and pubs etc. people buy meals through engaging with cashiers or sellers. The process of ordering and paying for meals can be stressful when the cafeteria is overloaded. Reducing the time of ordering and paying processes can make a great save in terms of time efficiency.
With A-Tab, our aim is to reduce the time for asking the cost of the meal. A-Tab aims to give the cost of the meal that is ordered by the customer without any interaction with the cashiers by taking the photo of the meal. The project is important in general because of the innovative tools that it will be using through accomplishing its aims and can be improved in the future to accomplish other various tasks, like other image analysing applications.
In this report, first we will describe our A-Tab project. After that, constraints of the project will be examined under the appropriate sections. Then, we will discuss professional and ethical issues that may arise. After those, requirements of the project will be given under appropriate sections grouped under functional and non-functional requirements. 
### 1.1 Description
Our project aims to deal with the time inefficiency problem that is faced in mostly cafeterias and restaurants. Our proposed solution helps the customers to see the costs of the meals they ordered by taking a photo of the meals. 
The application that the project will create will take the images as inputs. It will analyse the image of the meals. We designed a few subsections  that will accomplish that purpose. Each subsection is classified by different algorithms.
The first algorithm is designated for segmentation of the image:
Non-meal and meal objects will be seperated. Non-meal objects are going to be disregarded.
If they are different, meal objects will be seperated and changed into something that is easier to analyze. Then they will be sent to the second algorithm.
The second algorithm will analyse the meals:
Object classification will be done by the second algorithm.
The third algorithm will make object matching:
The meal that is classified will be checked through a large database of classes. A matched class will give the cost as return. 
After the third algorithm, the cost of the meals that are given to the application will be returned.
We expect to face three main problems that we described above, segmentation, object classification and object matching. We are planning to use Machine Learning algorithms, some of them will be taken from open sources, some of which we will create ourselves. ML uses statistical reasoning to find approximate solutions for tackling the above difficulties. [https://www.zib.de/sites/default/files/Day1.pdf]
Through designing the analysis and high-level design report, we can discover and use new ways of solving the problems above. For example, for increased accuracy, Image classification can be done using CNN(Convolutional neural network)[https://becominghuman.ai/image-processing-with-deep-learning-a-quick-start-guide-38e166340200]
In the same way, we can find and choose different ways to accomplish the main task of the project, like Data Labeling and RCNN.
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
