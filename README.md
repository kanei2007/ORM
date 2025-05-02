# Ex02 Django ORM Web Application
## Date:20/04/25 

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![Screenshot 2025-05-01 212734](https://github.com/user-attachments/assets/bb9d7efa-2f81-4eb2-b0a1-7508e4e135ad)


## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM:
admin.py

from django.contrib import admin 
from .models import Movie_DB, Movie_DBAdmin 
admin.site.register(Movie_DB, Movie_DBAdmin)

models.py

from django.db import models 
from django.contrib import admin 
class  Movie_DB(models.Model): 
    Actor = models.CharField(max_length=20, primary_key=True) 
    User = models.CharField(max_length=100) 
    Genre = models.CharField(max_length=20) 
    Tag= models.IntegerField( ) 
    Writer = models.CharField(max_length=15) 
    Director = models.DateField( ) 

class Movie_DBAdmin(admin.ModelAdmin): 
    list_display = ('Actor', 'User', 'Genre', 'Tag', 'Writer','Director')
## OUTPUT:
![image](https://github.com/user-attachments/assets/c537f016-baaf-499b-8c72-68aa8b568d1e)

## RESULT:
Thus the program for creating movies database using ORM hass been executed successfully
