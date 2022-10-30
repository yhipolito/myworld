# Overview

I want to demonstrate the application of Django features on the creation of a WebApp.

I have created a WebApp that interacts with a SQL databases that came with Django, to start a test server on my laptop I used the command "python3 manage.py runserver". after that I am able to use the following URL on my browser http://127.0.0.1:8000/members/

The purpose of writing this software is to keep a basic track of my family members. This is a basic sample that maybe used to create a larger WebApp to register users.

[Software Demo Video](https://youtu.be/gVQvVZ_cz3w)

# Web Pages

I have created the add.html page which allows us to create a new record for our database members. Another page I have created besides index.html is update.html which allows to change some of the previous created records. We transition between pages thanks to members.urls.py which has a urlsPatterns list, One of those is "path('update/<int:id>', views.update, name='update')," This path call views.update function and pass the parameter of id which an integer. On views we can find python functions that call templates. In update funtion we pass an argument ({{ x.id }}), Then we call the record related to that id to send a HttpResponse which will render update.html template with the respective context.

# Development Environment

I used Django version 4.1.2 and Python 3.10.7 to develop the software.

# Useful Websites

* [W3schools](https://www.w3schools.com/django/index.php)
* [Django](https://www.djangoproject.com)

# Future Work

* I would like to improve the design of the wev app.
* I would like to created a web app that can upload, upload, delete and update pdf files. With this I will be able to store important information of Helipads features for Helicopter pilots in United Nations mission in Africa.
* I would like to improve my understanding of the differents tags we can use on Django.