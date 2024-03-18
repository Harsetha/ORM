# Ex02 Django ORM Web Application
## Date: 11.03.24

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![312752025-38582397-61f3-44d7-ba5f-652d496fdfce](https://github.com/Harsetha/ORM/assets/149985878/b2c43da4-cdb6-4762-9c33-5317f6021f00)


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
from django.db import models
from django.contrib import admin
class Book_DB(models.Model):
      sno=models.IntegerField(primary_key="sno");
      name=models.CharField(max_length=50);
      author=models.CharField(max_length=70);
      price=models.IntegerField();
      publisher=models.CharField(max_length=60);

class Book_DBAdmin(admin.ModelAdmin):
    list_display=("sno","name","author","price","publisher");
```
### admin.py:
```
from django.contrib import admin
from .models import Book_DB,Book_DBAdmin
admin.site.register(Book_DB,Book_DBAdmin)
```

## OUTPUT
![312770060-c78cae4d-66f9-42f3-8014-e982941b685b](https://github.com/Harsetha/ORM/assets/149985878/921b4b31-0d0f-4180-b186-847b6463daae)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
