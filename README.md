# **Budget Manager 📈**

>__1. Description of you website, including:__
>* Purpose 
>* Functionality / Features
>* Target audience 
>* Tech stack

### **Purpose**

The purpose of a budget app is to keep track of our expenses and to manage how our money is spent daily, as an international student living in Melbourne being on a budget and keeping track of how my money is coming in and out is crucial as nowadays we are all trying to get some financial education, I am a true believer that having the ambit of being on a budget is the first step for getting into financial education, a subject that no one has taught us so far. 

A budget is a financial plan that will help us to keep track of and manage our income and expenses. The main purpose of being on a budget is to ensure that we are spending our money wisely and that we are not overspending. Being on a budget makes us more aware of how our money is going out each month. This makes us prioritize different expenses and save more money for future goals. 

Being on a budget also allows us to save enough money for different goals in the future, even if it saves for a new laptop, phone, or even bigger things like paying off debt, making a down payment, or building an emergency fund, etc. It allows us to save more money than if were not on a budget.

**The perks of being on a budget are:**

* Increased financial awareness 
* Reduced financial stress 
* Improved savings 
* Achieving financial goals 
* Greater financial freedom 

Nowadays, a lot of students keep track of their expenses by doing a simple spreadsheet in Excel, which is the easiest way to keep track of your expenses however, a lot of people start lacking interest after a couple of days since it is annoying sometimes to go and grab your laptop for a better view for registering your expenses of the day, that’s why with my app a will be providing and smooth and easy way to register your expenses from each day so you can keep track of your expenses from wherever you are. 

### **Features**

* **User Registration**

Easy user registration for the user to set their username and password, also as an extra for keeping track of what kind of people is using the app, I have decided to add an extra question asking what are they more in the sense into knowing if they are students which is the target audience for the budgeting app, or a professional for example. 

* **Savings Goals**

Saving Goals is one of the main features of the app as it is the one that will be keeping track of how much money we are saving for different purposes. Each person has a different goal for saving money, so we can not set default name for the different savings accounts since people might not be saving at the moment for a car (an example), that's why I have decided to give the freedom to users for selecting the name of their savings account as each user has different needs.

* **Expenses**

Another main feature of the app, as it is the page that keeps track of all the expenses and also lets us know how much we have spent on each category, for this project we have created default categories as in this case, it is more predictable to tell what kind of expenses a user has as they are more related to expenses of our daily routine like groceries, eating out, shopping, etc. 

* **Automated Bills**

Automated Bills are an extra feature for this app as it is not crucial, however, is plus on the app, as it allows us to keep in mind those expenses that happen on a weekly, monthly or yearly basis, an easy example of this is paying for rent every 1st of the month, or for some students it can also be paying for their tuition every month, bills like power, gas, subscriptions, etc. All these kinds of expenses that have been already settled can be registered on this side of the app, as the user will be able to name, categorise it, add the amount, the next payment day and how often the bill will be, so the app can keep track if it will be an expense of every month, etc. 


* **Money In/Out**

Money In/Out is an extra feature as well, this feature can be seen also as a summary of all four features, in this page we can only view how much money is in, and how much money has been out so far, keeping on mind that it will stop tracking at the end of the month for restarting the expenses again. 

### **Target audience**

The target audience for a budget app is all the people that are trying to save money, saving money is not an easy or difficult task, is all about having habits and being organized with money, having as an outcome the ability to save as much money as we decide to no matter how much your income is, there is always ways and rules to follow for saving money. Even though I'm creating this app for students than for professionals as the interface is more friendly and not as serious as other budgeting apps, professionals are also invited to join this new app and enjoy the features that the app has to offer. 

### **Tech Stack**

![Budget Manager Tech Stack](/docs/TechStack.png)

For this project, we will be using a MERN stack, which is an open-source one that combines different JavaScript-based frameworks, such as MongoDB, Express, React, and Node.js, allowing us to create and build web and mobile applications. 

>**The MERN components are used for the next purposes:**

* **MongoDB** - Mongo is a NoSQL Database where data is stored as documents with key-value pairs. It also enables to create databases, schemas and documents instead of tables. While using Mongo we can delete, query and update records. 
    
    All the data registered about goals, expenses, amounts and categories from our features will be stored here in different records, as we will be asking all the time for different data, deleting, updating and creating new records each day. 

* **ExpressJS** - This is a NodeJS framework that helps us simplify our code. It offers a range of middleware making the deployment of our app more efficient as it saves us from creating different Node modules. Also wraps all the HTTP requests and responses complementing perfectly the ReactJS framework by developing interactive user interfaces while communicating with the server 

* **ReactJS** - This is a JavaScript library that allows the development of user interfaces or in this case, the development of single-page applications as it uses the virtual DOM for rendering the different sections. 

* **NodeJS** - It is an open-source JS runtime environment that allows users to run code on the server.  

>**2. Dataflow Diagram**

![Dataflow Diagram](/docs/DataFlow%20Diagram.png)

**From the Dataflow Diagram, we can map out that:**

* A budget user exists and can log in for its authentication 
* If a budget user does not exist, it can sign in and have authentication as well 
* Once authenticated the user can perform different actions 
* Users can create, edit and delete saving goals 
* Users can create, edit and delete expenses 
* Users can create predicted bills 
* Users can have an overview of their expenses and savings 
* All Expenses data is sent to a specific database
* Savings data is stored in a unique database, as well as Bills data and Users data from Budget Manager

As can be seen in the dataflow diagram it has different starting points for data, beginning with the data used for logging in as it is used for doing authentication of the user, after that this data will keep flowing along any action as it is the data that have allowed us to stay inside of the app. 

Data is collected by performing actions like creating expenses, goals, etc. Will start their flow by retrieving the data that the user has typed, and sending it to their specific database, as well as it can be seen when being on the home interfaces of each feature, or in the overview of the Money In/Out feature. 

>**3.Application Architecture Diagram 

![AAD](/docs/Application%20Architecture%20Diagram.png)

This Architecture Diagram describes how the app will be working, a single-page application is an easy diagram as it will be performing easy CRUD actions, however even though the app will be doing easy CRUD actions it is needed different kinds of layers along our app. 

Firstly, we can see the presentation layer, as the word itself here we find UI’s since from this point it can be seen how the client or the user, enters into the app and it will only have access to the views of the different windows that are rendered throughout the HTTPS requests that the user does. Even though the user will be doing HTTPS requests through the buttons and fields found in the app, these HTTPS requests will be the real Application Layer as they will be communicating with the database. 

Once HTTPS Requests are sent and processed the database receives the data requested and will send back the data that we have requested or the confirmation of the changes done to the databases of the Budget Manager in an XML or JSON format so our page can render the new data and project it into our app.

 >**4. User Stories**

### **User Story 1**

**“As an international student, I want to keep track of my expenses, so I can save a small amount at the end of every month and keep track of my expenses.”**

* Expenses Tracker
* The user wants to save money even if it's a small amount
* The user is an international student
* The user wants to keep track of his expenses

The app itself will have an expense tracker as one of the main features, so the user will be able to keep track of his expenses and even what kind of expenses was it by registering the kind of category this was.
___

### **User Story 2**
**“Im a graduated student and I have been on a budget for the last year however it has been really boring to keep doing it from a spreadsheet on my laptop, I wish there was a dynamic and easy app for budgeting, so I will not be bother by using my laptop all the time”**

* The user is a graduated student
* User wants a dynamic and friendly budgeting app
* Want to keep on a budget
* He wants an app that can be managed from his phone and not only from his laptop

Budget Manager intends to be available on any device and also the design of Budget Manager has been done with the purpose of being easy and friendly to use by also following the psychology of colours so users can feel confident and optimistic about it.
___

### **User Story 3** 
**“As a user of Budget Manager, I intend to have different saving goals as I have different purposes on each since I manage different expenses that need to be covered at the end of the month like rent, tuition, personal savings, etc”**

* Users want to have a different savings account
* If possible name them based on what they are going to be used for

As an extra feature of creating a saving account, users will be able to name their savings account by the name they decide to.
___

### **User Story 4**
**“I’m an user that is just getting into the habit of saving, so occasionally i overspend a bit of money and i tend to withdraw money from my savings and i want to keep like that till i get used to be on a budget”**

* User wants to be able to withdraw money from his saving accounts
* It is getting into the habit of being on a budget
    * Should some alerts be trigerred as a warning when withdrawing money from their savings?

Even though uses should not withdram money from their savings account till they achieve their goal, they will be able to withdraw money from their different savings accounts.
___

### **User Story 5**
**“As a casual employee, I'm really rigorous about the due dates of my bill, most of the time I forget the due date of my subscriptions or bills, it will be a plus to be able to keep a record of my bills as sometimes I don't enough money on my front account”**

* The user wants to be able to view the due date of his bills and subscriptions in advance
* Being able to difference bills from subscriptions or other kinds of predicted payments
* Have a proper date of payment

As a 'nice to have' feature of Budget Manager is to have predicted bills, where the user will be able to add his/her subscriptions, bills, etc by the next payment due and also by telling how recurrent will this be (monthly, weekly, etc).
___

### **User Story 6**
**“As a user of BM, I want to be able to see an overview of my expenses and savings so far, because I want to be able to have a summary all together in one page without having to go from the expenses page to the savings on and off”**

* The user wants to have a summary on one page
* In summary, he wants to be able to see expenses and savings so far

As another of our ‘nice to have’ features, I have in mind having an overview page where it will show expenses and savings so far of each user, represented by a pie chart so the user can have a better dimension of how the money has been managed so far.
___

>**5. Wireframes for multiple standard screen sizes, created using industry standard software**

💡 Check Wireframes in [Figma Budget Manager](https://www.figma.com/file/9aP74PmjvV3k0VeWMFa3Uf/Budget-Manager?type=design&node-id=0%3A1&mode=design&t=4g8dJY4GJIITDvL7-1).

### **Sign In - Interface**

The sign in interface has an easy and friendly interface where the user can sign in or log in, each color in the buttons is related to what the user decides to do. At the end of both actions the user gets a "Let's Begin" screen for continuining into the next screen. 

The user will log in his user and password, and for target audience purpose for first users we will have a simple question for the users so we can know into more detail if students, professional or others are the ones who are signing into the app. 

![Home Wireframe](/docs/wireframes/Home.png)

> 📝 **We encourage to visit the [Figma project](https://www.figma.com/file/9aP74PmjvV3k0VeWMFa3Uf/Budget-Manager?type=design&node-id=0%3A1&mode=design&t=4g8dJY4GJIITDvL7-1) as inside of the project all the flows and prototypes can be seen there, so you can have a deeper introduction into how the flow of the app will be and how users will be able to interact with the differemt components. Aside that all screensizes can be found in there as well.**

### **Goals - Interface**

As we can see on the wireframe, we have a nav bar on the bottom where all our features can be seen. Next to our nav bar we have the 'Add new goal' button which will lead us to the interface for adding a new goal, where the user will be able to pick a name, target amount, initial amount and decide if it wants to save it or go back. 

Once the goal is created the user wil have the chance to eliminate, edit or add amount into the goal, is a really easy interface with no complexity at all, as it can be kind of predictable what is needed from the user to register. 

![Goals - Interface](/docs/wireframes/Goals.png)

### **Expenses - Interface**

On the expenses interface we can see a pie chart which will be the one that keeps track of the categories expenses like goign out, groceries, etc. In this case since is more predictable to know what kind of expenses a user can have, the categories have been introduced by default so the user just needs to select the one that fits better his expense category. 

Once the expenses are added we can see how the pie chart changes based on the expenses that the user registers. 

![Expenses - Interface](/docs/wireframes/Expenses.png)

### **Predict Bills - Interface**

On this interface we can see the change of color about adding a bill, since it is a different kind of expenses i have decided to provide a different color so the user when introducing data can tell if it's on the right interface or not. 

User will just have to add basi data like company, categories that have been added by default as well, amount, frequency and date, so the app can tell the user when will the next bill be, so the user can be aware of his expenses and try to manage his money based on this kind of expenses. 

The user can also delete or edit a bill by clicking on the bill that it decides to change, in this we can see the flow of the interface if the user decided to edit or delete the Rent Bill of SHA Rental. 

![Predict Bill - Interface](/docs/wireframes/Predict%20Bills.png)

### **Money In/Out - Interface**

We have a simple wirefram in this interface as this section of Budget Manager will be used more as overview of expenses, savings, etc. The user will not really be able to generate any change to the data presented as it is just an slice of everything that he has introduced, the only component that the user will be able to use, will be the nav bar located at the bottom of the screen

![Money In/Out - Interface](/docs/wireframes/Money%20In-Out.png)


>**6. Screenshots of your Trello board throughout the duration of the project**

📊 Check [Trello Board](https://trello.com/invite/b/JmcGUZEL/ATTI71e6594f42123a0d62571ad238421aae9030AAD3/budget-manager)

**1. Create Trello Board with cards** 
___
![Step 1](/docs/trello/1.png)

**2. Add required infromation to the fields that we will need to work later on. Settle down feature os Budget Manager** 
____
![Step 2](/docs/trello/2.png)

**3. Insight of how the features cards look like with all planeation a bullet points of what we are looking for on each feature**
___
![Step 3](/docs/trello/3.png)

**4. Create an sketch of the tech stack, and start adding information about how to manage the dataflow diagram**
___
![Step 4](/docs/trello/4.png)

**5. Add all wireframes, before due date, except from the final wireframe as there were little details that needed to be finished**
___
![Step 5](/docs/trello/5.png)

**6. Finish the Dataflow diagram, and start working on the architecture diagram while trying to settledown the Tech Stack**
___
![Step 6](/docs/trello/6.png)

**7. Add mor etask into the architecture diagram as i was still working on little details about, also finished the Tech Stack**
____
![Step 7](/docs/trello/7.png)

**8.All Diagrams were finished and uploaded into the README file**
___
![Step 8](/docs/trello/8.png)

**9. Start working on each user story so we can work further into touching up features for the next stage**
___
![Step 9](/docs/trello/9.png)

**10. Add more tasks into User Stories and Wireframes**
___
![Step 10](/docs/trello/10.png)

**11. The final wireframes are ready!**
___
![Step 11](/docs/trello/11.png)

**12. Purpose and Target Audience done**
___
![Step 12](/docs/trello/12.png)

**13. Add User Stories to README**
___
![Step 13](/docs/trello/13.png)

**14. Trello Board finished, looking forward for the next stage**
___
![Step 14](/docs/trello/14.png)
