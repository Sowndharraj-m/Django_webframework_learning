How does Django working ? 
    Django followes the MVT (Model View Template) architecture pattern.

Model - The data you want to present, usually data from a database.
View - A request handler that returns the relevant template and content - based on the request from the user.
Template - A text file (like an HTML file) containing the layout of the web page, with logic on how to display the data.

Model - 
     The model provides data from a database.
     In Django, the data is delivered as an Object Relational Mapping (ORM), which is a technique designed to make it easier to work with databases.
     The most common way to extract data from a database is SQL , but one problem with SQL is that it is not object oriented, and it can be difficult to work with in Python.
     Django with ORM allows you to work with databases using Python code, which is more intuitive and easier to understand.
     **The modls is located in the models.py file of a Django app.**
View -
     A view is a function or method that takes http requests as arguments, imports the relevant model(s), and finds out what data to send to the template, and returns the final result.
     **The views are usually located in a file called views.py.** 
Template -
      A template is a file , where you describe how the data should be presented. It is usually an HTML file, but it can also be a text file or any other format.

      Django uses standard HTML to describe the layout, but uses Django tags to add logic:
        {% for %} - A loop that iterates over a list of items.
        {% if %} - A conditional statement that checks if a certain condition is true.
        {{ variable }} - A placeholder for a variable that will be replaced with the actual value when the template is rendered.
        <h1>My Homepage</h1>
        <p>My name is {{ firstname }}.</p>
        **The templates are usually located in a folder called templates.**
URLs - 
        The URL is the address of a web page. In Django, you can define the URLs for your web application in a file called urls.py. 
        The urls.py file contains a list of URL patterns that map to views. When a user requests a URL, Django looks for a matching pattern in the urls.py file and calls the corresponding view function.