# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![ERdiagram](https://github.com/Bhagath118/django-orm-app/assets/147473779/8238d53e-6aaf-4bb8-9ebd-33227ec17c36)


## DESIGN STEPS

### STEP 1:
create folder 'ex02' under the directory 'unit2'
### STEP 2:
clone the Github repository into the directory 'ex02' using the command "git clone "
### STEP 3:
 under the folder "django-orm-app", enter the directory titled "dataproject" and enter the folder "dataproject" and go to the file "setting.py", "os" in line 14, set ALLOWED_HOST=['*'] and add 'myapp' under the list INSTALLED_APPS.
Write your own steps

## PROGRAM
```
models.py:
from django.db import models from django.contrib import admin

class Student (models.Model): referencenumber=models.CharField(primary_key=True,max_length=20,help_text="reference number") name=models.IntegerField() age=models.IntegerField() email=models.IntegerField() phonenumber=models.IntegerField()

class StudentAdmin(admin.ModelAdmin): list_display=('referencenumber','name', 'age', 'email')

admin.py:
from django.contrib import admin from .models import Student,StudentAdmin

admin.site.register(Student,StudentAdmin)
```

## OUTPUT
![image](https://github.com/Bhagath118/django-orm-app/assets/147473779/5d774846-c378-4008-9f40-d68a4d411fd6)



## RESULT
The Program is Executed Successfully.
