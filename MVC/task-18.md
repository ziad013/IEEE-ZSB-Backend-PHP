1-The Controller's Job:

 If a user clicks a button to "View
Profile," what exactly does the Controller do before sending
the final page back to the user???

1.Receives the request
2.Processes the request ==> to check user has permission to view the profile and user is logged in.
3.Gets the data from the Model ==> Model retrieve data from database and send to controller
4.Passes data to the View ==> To display it via Html page

---------------------------------------------------------------------
2-Dynamic Views:

What is the difference between a static HTML file and a dynamic PHP View??

Static HTML File:
-Content is fixed
-Written only in HTML
-Cannot connect directly to databases
-ex ==> <h1>Welcome Ahmed</h1>

Dynamic PHP View:
-Content can change
-Written in PHP + HTML
-Can fetch data from databases and display it
-ex ==> <h1>Welcome <?php echo $Name; ?></h1>
-------------------------------------------------------------------------
3-Data Passing:

How does a Controller pass data (like a user's name fetched from the database)
into a View so it can be displayed on the screen??

1.Get Data from Model(Retrive data from database)
2.Storing in array or variable
3.pass data to View via function like this

public function User() {
    $userName = "Ziad";

    return view('profile', [
        'name' => $userName
    ]);  
};


-------------------------------------------------------------------------------------
4-Templating (Headers & Footers):

How does the MVC structure help you avoid copying and pasting the exact same
navigation bar and footer code on every single page of your website??

-By using layouts ==>Create Seperete file for header and file to footer 
and each page View includes these files
Write what you want and call them via (include)

so
-Void repeated code
-Clear and organise
-easy to maintain



---------------------------------------------------------------------------------
5-Logic in Views:

Why is it considered a bad practice to put complex if statements
and heavy data-processing loops directly inside your View files??

-Because View’s job is only to display data, not handle complex logic or processing

-existance php + html ==> Make Code complex and messy
-Slower Performance
-hard to maintain



















































