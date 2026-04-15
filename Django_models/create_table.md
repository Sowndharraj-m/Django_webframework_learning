Django Models - 

       A django models is a class that represents a database table, and it is used to define the structure of the data that we want to store in the database. It is a way to interact with the database using Python code, and it provides an abstraction layer that allows us to work with the database without having to write raw SQL queries.

Creat (model) - 
    To create a model, navigate to the models.py file in the /members/ folder.
Open it, and add a Member table by creating a Member class, and describe the table fields in it:

from django.db import models

class Member(models.Model):
    firstname = models.CharField(max_length=255)
    lastname = models.CharField(max_length=255)
    
**SQLite Database -**
When we created the Django project, we got an empty SQLite database.
It was created in the my_tennis_club root folder, and has the filename db.sqlite3.
By default, all Models created in the Django project will be created as tables in this database.

Migrate -
Now when we have described a Model in the models.py file, we must run a command to actually create the table in the database.
Navigate to the /my_tennis_club/ folder and run this command:

python manage.py makemigrations

View SQL
As a side-note: you can view the SQL statement that were executed from the migration above. All you have to do is to run this command, with the migration number:

python manage.py sqlmigrate members 0001

