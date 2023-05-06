# Ex02 Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a student database using Object Relational Mapping(ORM).

# Entity Relationship Diagram

![image](https://user-images.githubusercontent.com/113497104/236615099-4de261d9-bba1-48f8-bc97-dd076b8fbfc6.png)

## DESIGN STEPS

### STEP 1:
Clone the repository from github.

### STEP 2:
Create an admin interfacefor Django.

### STEP 3:
Create an app and edit settings.py.

### Step 4:
Makemigrations and migrate the changes.

### Step 5:
Create admin user and write pythoncode for admin and models.

### STEP 6:
Make all the migrations to 'myapp'.

### STEP 7:
Create an student database with 10 feilds using runserver command.

# PROGRAM
```
admin.py 

from django.contrib import admin
from .models import student,studentAdmin 
admin.site.register(student,studentAdmin)

models.py

from django.db import models
from django.contrib import admin
class student (models.Model):
    sid=models.CharField(max_length=28)
    name=models.CharField(max_length=30)
    regno=models.IntegerField()
    marks=models.IntegerField()
    email=models.EmailField()

class studentAdmin(admin.ModelAdmin):
    list_display=('sid','name','regno','marks','email')

```
## OUTPUT

![image](https://user-images.githubusercontent.com/113497104/236615256-a6d401ff-591e-48de-9f94-a9c526975382.png)


## RESULT
The code executed successfully
