# Ex02 Django ORM Web Application
## Date: 18/02/2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![Screenshot 2024-04-24 190055](https://github.com/Narasimhan05/ORM/assets/151625188/f29578ae-5ea4-4749-be80-0e1cf3e7c750)

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
class Books(models.Model):
    bookid = models.IntegerField(primary_key=True);
    bookname = models.CharField(max_length=50);
    author = models.CharField(max_length=50);
    published = models.DateField();
    price = models.IntegerField();
class BooksAdmin(admin.ModelAdmin):
    list_display = ("bookid","bookname","author","published","price");


admin.py
from django.contrib import admin
from .models import Books,BooksAdmin
admin.site.register(Books,BooksAdmin)

```

## OUTPUT

![Screenshot 2024-03-15 114345](https://github.com/Narasimhan05/ORM/assets/132819871/5881c5cd-f573-4542-b2f7-915447edfb33)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
