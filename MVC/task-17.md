1-The MVC Pattern:

What does MVC stand for??
-MVC stands for Model - View - Controller.

What is the primary responsibility of each part (Model, View, Controller)??

1-Model ==>responsible for handling the data and business logic by
-Connecting to the database
-Retrieveing and stores data

2-View ==>responsible for the user interface by
-Displays data to the user
-Contains HTML/CSS

3-Controller ==>middleman between the Model and the View by
-Receives user requests
-Calls the Model to get data
-Sends data to the View
-------------------------------------------------------------------------------------
2-Routing:

what is a "Router"??
-Router is responsible for directing requests to the correct page  

Explain simply how it acts like a traffic cop for a website??
-It directs cars to different roads,the router directs website requests to the correct destination.

---------------------------------------------------------------------------------------
3-The Front Controller:

What does this mean compared to having dozens of separate files like about.php and contact.php??

-means the website uses one main file to handle all requests instead of having many separate files
and become
-More organized
-Easier to manage
-More secure

-----------------------------------------------------------------------------------------
4-Clean URLs:

Why??
1-Easier for Users
2-Easy to understand
3-Better for SEO ==> Search engines prefer clean and meaningful URLs
4-More Security ==>No alot of data in URL

--------------------------------------------------------------------------------------
5-Separation of Concerns:

Why is it considered a terrible idea to put database queries (SQL) directly inside your HTML files?؟

-HTML ==>handle Displaying content,Page design and User interface
-SQL  ==>handle Database operations

Mixing them together makes the code messy and hard to manage

It become bad because
1-Hard to Maintain and read
2-Less Secure

Solustion ==> Use MVC ==> keeps the project clean and organized












































