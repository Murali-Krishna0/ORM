# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here
![image](https://github.com/Murali-Krishna0/ORM/assets/149054535/d524f8e1-4cdf-43e2-bc56-081e46c208df)


## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create 10 Football players

## PROGRAM

Include your code here
```
admin.py
from django.contrib import admin
from .models import student,studentAdmin
admin.site.register(student,studentAdmin)

models.py
from django.db import models
from django.contrib import admin
class student (models.Model):
    name=models.CharField(max_length=20,help_text="student")
    rollno=models.IntegerField()
    refno=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
class studentAdmin(admin.ModelAdmin):
    list_display=('name','rollno','refno','age','email')
```

## OUTPUT

Include the screenshot of your admin page.
![image](https://github.com/Murali-Krishna0/ORM/assets/149054535/41683bd2-b858-4567-a238-69806cd0a071)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
