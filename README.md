Part 1:		
1.	What does ORM stand for? What does ODM stand for? 
-	ORM stands for Object Relational Model. 
-	ODM stands for Object Data Model.
2.	Based on the title of this part of the tutorial, what ORM/ODM will we be using?  What are some popular alternatives?
-	Based on the title of Data, I would assume that the ORM/ODM we will be using will be SQL. 
-	Some popular alternatives are MySQL and MongoDB.
Review the ER diagram in the tutorial (or see the link above). 
3.	How many entities are there?  What are the relationships between entities? 
-	There are 4 entities
-	 Mandatory one to Mandatory many (Books – Author)
-	Optional Many to Optional Many (Books – Genre)
-	Mandatory one to Optional Many (Books – BookInstance)
4.	What folder should this command be run in? (Hint: it's the root folder of your project.)
-	The project file
5.	In Windows, should you execute node commands in PowerShell as Admin or GitBash?
-	I use GitBash as Admin
6.	Open your project with VS Code. Open package.json - can you see mongoose? What version are you using?
-	5.9.7 
Process - Part 2  - Create Models
1.	Create a models folder in your project as shown in the tutorials repo. Is capitalization in folder names important? (Hint: yes; very)
-	Yes capitalization is important
2.	Using the tutorial repo as an example, create one file in your models folder for each entity. How many files will you have?  Follow all conventions - name each file exactly as they did. Is the name of the model file singular or plural? 
-	You will have 4 files. 
-	The name is plural
3.	Be able to read & understand code. Which model is the simplest? Which is the most complex? Why?  Can you determine what the additional code is doing for us? 
-	Genre seems to be the easiest. It is a simple get function
-	Author is the most complex. It is a large retrieval of multiple items.
Process - Part 4 - Update app.js to connect to your Atlas database
1.	What dependency are we requiring? 
-	express
2.	What is the development URL to your database?
-	 mongodb+srv://lewisA:password@cluster0-fogqp.azure.mongodb.net/test?retryWrites=true&w=majority

3.	Where do we call mongoose.connect()
-	App.js
4.	Where do we set mongoose.Promise to global.Promise?
-	App.js
5.	On getting a connection error, what logic is called? 
-	Bind 
6.	How do you start your app? 
-	Npm start
7.	How do you stop your app? 
-	CTRL + C
8.	Open a browser to localhost:3000 - what do you see? 
-	express
