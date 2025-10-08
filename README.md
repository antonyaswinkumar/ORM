# Ex02 Django ORM Web Application
## Date:08/10/2025 

## AIM
To develop a Django application to store and retrieve data from a Car Inventory Database using Object Relational Mapping(ORM).

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
 
 ```
 admin.py

 from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee, EmployeeAdmin)



models.py

from django.db import models
from django.contrib import admin

class Employee(models.Model):
    eid = models.CharField(max_length=20, help_text="Employee ID")
    name = models.CharField(max_length=100)
    salary = models.IntegerField()
    age = models.IntegerField()
    email = models.EmailField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display = ('eid', 'name', 'salary', 'age', 'email')


## OUTPUT


<img width="1920" height="1080" alt="Screenshot (46)" src="https://github.com/user-attachments/assets/3ec94817-94e7-4a4a-83e5-894a2fa6856f" />


<img width="1920" height="1080" alt="Screenshot (46)" src="https://github.com/user-attachments/assets/c5fa8bc9-f983-46bb-9099-f6fea64bf998" />

## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
