Add Records - Insert Data into the Database
The Members table created in the previous chapter is empty.
We will use the Python interpreter (Python shell) to add some members to it.
To open a Python shell, type this command:
python manage.py shell

Then, run the following code to add a member to the Members table:
from members.models import Member

Query set -
A query set is a collection of database queries that can be used to retrieve data from the database.
To create a query set, we can use the objects attribute of the model class.
