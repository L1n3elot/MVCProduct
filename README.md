# App Description
The app displays the home page which allows the user to navigate through other pages such as the privacy and products page. In the products page, the webpage displays a row that allows the user to create a product and add it to their list. They can input the title, release date, genre and price of their choosing and edit/delete if they want to. 

# Running the app
1. Download Visual Studio with ASP.NET and web development workload
2. In the Get Started section, click on Clone a Repository
3. In the upper right hand corner of the GitHub repository, click the green button labeled "Code" then copy the url shown
4. Paste the url in Visual studio under Repository location, then click clone
5. Launch the app by clicking the green triangle on the upper side of the page or by clicking F5

# Dependencies
Dependencies from the app includes multiple analyzers such as:

1. AspNetCore.Analyzers
2. Microsoft.AspNetCore.App.Analyzers
3. Microsoft.AspNetCore.App.CodeFixes
4. Microsoft.AspNetCore.Components.Analyzers
5. Microsoft.AspNetCore.Mvc.Analyzers etc...

The frameworks section includes:
1. Microsoft.AspNetCore.App
2. Microsoft.NETCore.App

Packages include:
1. microsoft.entityframeworkcore.sqlserver(9.0.0)
2. microsoft.entityframeworkcore.tools(9.0.0)
3. microsoft.visualstudio.web.codegeneration.design(9.0.0)

# DI
I have grouped the service and controller as loosely coupled in order to keep everything organized and maintainable. I have injected all methods from product services into the controller so that the controller can take user requiests based on what the methods call for. For example, the Create action method takes a request from users who decides to add a product based on the method call coming from the service classes and interface.

# Main products page:

https://localhost:7132/products

# Example for first movie on list:
The road map for the first movie works for id 14 rather than id 1 along with other movie ids increased by 13.

https://localhost:7132/products/details/14

# Example for 3rd movie

https://localhost:7132/products/details/16

# Examples of road map leading to specific movie genres:

https://localhost:7132/products/bygenre/comedy

https://localhost:7132/products/bygenre/western

https://localhost:7132/products/bygenre/romantic%20comedy

# Examples of road map leading to movies based on release date:

https://localhost:7132/products/released/1989

https://localhost:7132/products/released/1959

# Going to movie create page example:

https://localhost:7132/products/create
