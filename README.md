# Ex02 Django ORM Web Application
## Date:20/04/25 

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![image](https://github.com/user-attachments/assets/7017f906-e4e3-44dc-a40e-22b113d5771e)



## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
'''
''' admin.py

from django.contrib import admin from .models import Employee,EmployeeAdmin admin.site.register(Employee,EmployeeAdmin)

models.py

from django.db import models from django.contrib import admin class Employee (models.Model): eid=models.IntegerField(primary_key=True) name=models.CharField(max_length=100) salary=models.IntegerField() age=models.IntegerField() email=models.EmailField()

class EmployeeAdmin(admin.ModelAdmin): list_display=('eid','name','salary','age','email') '''


## OUTPUT
![image](https://github.com/user-attachments/assets/ea09d513-f01d-4b6e-8c4d-b37bc3a3cfbb)



## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
