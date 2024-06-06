Olushola Whenu(0850286)
Web app created with VS2022 .NET 8
2024-05-16


Modified the ASP .NET MVC Core application
Using .Net 8, with no authentication

1350
Program loaded successfully using default URL:
https://localhost:7164/
Modified the index.cshtml title to MVC MOVIE 
Created README.txt to document all changes
Tested the appication to confirm all changes


1420
Confirm that part 1 is complete and moved to part 2
Part 2
Added a Controller

1425
Added new index method and changed the content to "This is my default action..."
Tested and confirmed the changes worked
https://localhost:7164/HelloWorld


1500
Added another method "This is the Welcome action method..."
Confirmed with the following URL:
https://localhost:7164/HelloWorld/welcome

1510
Modified the Welcome method to include two parameters (name,numtimes)
I commented out the previous methods but got an error
I looked through and corrected the typo
Confirmed the changes with the following URL:
https://localhost:7164/HelloWorld/Welcome?name=Whorms&numtimes=3
Completed Part 2


2024-05-23
0137
Started Part 3
Modified the HelloWorldController class to use Razor view Files
Replaced the Index method with IActionResult Index

0150
Added a New Folder "HelloWorld" to the views folder
Added a new item "Razor View - Empty"in the HelloWorld Folder 
Replaced the content of "Views/HelloWorld/Index.cshtml"
Tested by navigating to "https://localhost:7164/HelloWorld"
Changes were successful!

0200
Change Views and Layout pages
Replaced the content of the Views/Shared/_Layout.cshtml
Changed MvcMovie to Movie App
Changed the anchor element 
Saved changes and tested successfully.

0215
Created a loop in the Welcome.cshtml view template that displays "Hello" NumTimes
Replaced the contents of Views/HelloWorld/Welcome.cshtml 
Saved Changes
Tested by browsing to https://localhost:7164/HelloWorld/Welcome?name=Rick&numtimes=
Changes were successful

0245
Added a data model class
Updated the Models/Movie.cs
Added a NuGet Package
Used the scaffolding tool to produce Create, Read, Update, and Delete (CRUD) pages for the movie model
Used the EF Core Migrations feature to create the database
Performed initial migration with the following commands:

Add-Migration InitialCreate
Update-Database

Tested the app with no errors

0300
Examined the generated databases
Migrations/20240523184715_InitialCreate.cs
20240523184715_InitialCreate
Controllers/MoviesController.cs


2024-05-30

0130
Seeded the database
Created a new class "SeedData" in the Models folder
Added the seed Initializer
Replace the contents of Program.cs with the new code
Deleted all records in the database
Tested the app by forcing it to reinitialize, calling the code in program.cs
Refreshed the app
Changes didn't reflect
Sigh!
Went through the tutorial again
Oops...I didn't close the command prompt window
Closed the command prompt window
Refreshed the application
App successfully shows seeded data.
Yesssssssssssssssssssssssss!
Completed part 5


0150
Started Part 6
Controller methods and views
Opened the Models\movies.cs file and added new code
Open the Movies controller 
Examined the two Edit action methods
verified the input validation for date and price
Completed part 6

0215
Started Part 7
Add search
Add search compatibility by genre and name to the index method
Updated the Index method found inside Controllers/MoviesController.cs with new code
Saved and tested the app
Navigated to /Movies/Index. 
https://localhost:7164/Movies/Index
Appended a query string "?searchString=Ghost"" to the URL
The filtered movies are displayed.
Changed the signature of the Index method to have a parameter named "id"
Changed all occurrences of searchString to id
Saved changes
Tested by navigating to URL "https://localhost:7164/Movies/Index/Ghost"
Search displayed on the Ghost movie

0245
Added UI elements to help filter movies
Changed all occurrences of id back to searchString
Added a form tag to the Views/Movies/Index.cshtml file
Updated form with new code
Tested the application
Got an error message
Returned to the tutorial and found a fix in the next step.
Updated the Index.cshtml file found in the Views/Movies/, specifying that the request should be "HTTP GET" 
Added search by Genre







