Video On Demand Chat [ Project for COMP 307 (Web Development) ]

Matthew Etchells : 260680753
Adam Gilker : 260676031 
Chen Yue : 260909729

To run the project, enter the vodchat directory, then run:
    
    python3 manage.py makemigrations
    python3 manage.py migrate

Which will initialize the database with the appropriate tables, and create a new file called db.sqlite3. Then run:

    python3 manage.py runserver

To run a development server. By default, the server will run on port 8000. Visit localhost:8000 in the browser to check that the server is running.

VueJS is being used only at the videos/watch page for now as the others are simpler pages for now.

Note: Django-channels requires a redis instance to be running for it to work properly. It is being used for getting notifications of new comments at videos/watch. You can run redis through a docker container or just using the redis-server command line tool.

Note: The self study portion of the project (i.e., the email verification/password reset) is by default turned off. It can be turned on by changing the keyword argument require_email_confirmation in the signup function in accounts/views.py to True.
