# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![Screenshot 2024-03-07 133620](https://github.com/Narasimhan05/ORM/assets/132819871/bc9e80f5-e89c-461b-9da7-14f7e108dd89)


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
models.py

from django.db import models
from django.contrib import admin
class Book(models.Model):
    bookid = models.IntegerField(primary_key=True);
    bookname = models.CharField(max_length=50);
    author = models.CharField(max_length=50);
    published = models.DateField();
    price = models.IntegerField();
class BookAdmin(admin.ModelAdmin):
    list_display = ("bookid","bookname","author","published","price");


admin.py
from django.contrib import admin
from .models import Book,BookAdmin
admin.site.register(Book,BookAdmin)

```

## OUTPUT

![Screenshot 2024-03-15 114345](https://github.com/Narasimhan05/ORM/assets/132819871/85055533-7014-446e-be61-c582d453b411

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
