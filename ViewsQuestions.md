You may omit Book, BookInstance, and Author views
1.	To save time, if you like, you may implement only the genre (i.e., the "type" of book) views.
2.	You'll have to remove any code that references the parts you don't implement. 
3.	If you chose this option, ensure associated routing and controller logic is in place, along with the  following views:
1.	layout & index (important!)
2.	genre list
3.	genre details 
4.	genre form (for editing information)
First, Just Read and Understand
1.	Read Express Tutorial Part 5: Displaying library data (Links to an external site.)
2.	Read through each sub-article (there are 12). 
3.	Read Express Tutorial Part 6: Working with forms (Links to an external site.)
4.	Interactive forms are harder than just displaying information. We will only implement one form.
5.	Read Express Tutorial Part 6: Working with forms / Create genre form (Links to an external site.)
"Begin with the End in Mind"- Explore the Example Repo 
1.	The Example repo can be found at https://github.com/mdn/express-locallibrary-tutorial (Links to an external site.)
2.	Feel free to use the sample repo as much as you like
Then, Follow the Tutorials above
1.	Go through the process of adding the different features to display the required views..
2.	Work through the sub-articles, before moving on to the next one.
3.	Work through implementing the interactive genre form.
4.	As you go, make sure you can answer the following questions. 
Process 1 - async
1.	What is the async module? What does asynchronous mean? (You can look it up.)
-	The async is a utility that allows for functions to work at the same time.
2.	What are 3 of the most important methods in the async module? What do they do? (Hint: parallel(), series(), waterfall())
-	Parallel is when the tasks are run independently and does not wait for other tasks to finish.
-	Series is the same as Parallel but each task is dependent of the previous. The final callback is submitted at the end together
-	Waterfall is just like series but each task is passed to the next.
3.	Why do we want to avoid "callback hell" by using async? (Hint: deeply nested code is hard to read, maintain, and debug!)
-	It is when there are multiple nested callbacks which cause it to be hard to read and debug.
4.	What happens you run 'npm install async'? 
-	It gives you the decency’s associated with async.
Process 2 - Template primer
1.	What view engine do we use? (Hint: it used to be called Jade.)
-	Pug
2.	We set two key-value pairs to configure the view engine by calling app.set(). To use Pug, what are these 2 calls?
-	The variables are the views and pug.
3.	After doing so, in what folder must our views go?
-	The views folder
4.	Review the example template. Once you know HTML is the syntax hard?
-	No
5.	Review layout.pug. What typically goes in the layout view?
-	Views folder
6.	Review index.pug.  What is in this view?  
-	An Unordered list
7.	Does layout contain index?  (Or does index contain layout?) Hint: the first one is correct. 
-	Layout contains the index.
Process 3 - Base template (Implementation Required)
1.	Add your base template (layout.pug). What folder does it go in?
-	Views
2.	What external css files are we using?
-	Bootstrapcdn, style.css
3.	What local css file are we using? What is this local file named? What folder is it in?
-	Our local css is style.css and it is in the public/stylesheets folder
4.	Modify the local css file. What class are we styling? How do you know it's a class not an id? (hint: dot) What elements are assigned to this class?
-	We are styling the navigation bar. It is a class. I know it is a class because of the (.). If it was an id it would have been denoted by a #. The class is being applied to an unordered list in the layout.pug.
Process 4 - Home page (Implementation Required)
1.	Work through the content to create the home page. Route - Controller - View
2.	If you built web sites for a living, would you like to use a view engine like Pug? Or plain old HTML? Why?
-	Using a view engine like pug makes it easier to load many items with different content in the same layouts. It allows for multiple content and saves on data and space.
Process 5 - Book List page (Read & Understand)
1.	Work through the content.
2.	Understand how to show the list of books page. Same process: Controller - View. 
3.	What does find() do? 
-	It finds the content
4.	Do you like chaining functions together? (Rather than having to create many intermediate variable names?)
-	Yes it makes it look cleaner
5.	Chaining is very powerful and widely used - appreciating this style of coding can be very helpful! 
Process 6 - BookInstance List Page (Just Read & Understand - Implementation is optional)
1.	Understand how to display a list of book instances. Controller - View. 
2.	Note that building views is somewhat repetitive.
3.	It's so standard, people have written code that scaffolds controllers & views for CRUD - create/read/update/edit in a wide variety of programming languages. Optional: Lookup Loopback, Sails, Visual Studio Scaffolding for .NET MVC and more)
Process 7 - Date formatting (Recommended)
1.	Dates are very complex!  Think leap year, time zones, daylight savings time, etc.
2.	Install the moment module (if you haven't already - how can you tell?) (Hint: check your package.json)
-	It should be a dependency in the package.json
3.	Adjust your book instance model (if needed) to provide a due date & then show the nicely formatted date on your page. 
4.	Working with dates is very common & a very useful skill.
Process 8 - Author List (Read & Understand) & Genre List (Implementation Required)
1.	Understand how to display an Author list page (Controller - View) 
2.	Create your own Genre list by analogy - hint: follow all conventions & spell/capitalize carefully! (If you don't you'll get debugging practice, which is good too. :)
Process 9 - Detail Page
1.	Follow the process to create and test the detail page for: Genre 
2.	You can complete Author, Book, and Book Instance if you like. (Some variation, but somewhat repetitive.)
3.	Do detail pages allow editing? (Hint: no)
-	No
Process 10 - Edit Information with a Form (Genre)
1.	Follow the guide to implement a page for editing genre data. 
2.	Optional: complete the others if you like. Next week, we'll deploy our web app! 
Summary
Implement the following views. Make sure your routes & controllers are updated to display them:
1.	layout
2.	index
Four list pages (only genre required)
1.	book list
2.	book instance list
3.	author list
4.	genre list
One detail page required:
1.	genre detail
One form page required:
1.	genre form (allows editing!)
Test and verify that all required views work. 

