# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## ENTITY RELATINSHIP DIAGRAM

![Screenshot 2024-03-07 184932](https://github.com/tharunkumaran2006/ORM/assets/151625188/876939c4-9e42-4244-ade6-5ae8c187c3e0)


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
'from django.db import models
from django.contrib import admin
class Book(models.Model):
	bookno         = models.IntegerField(primary_key=True);
	bookname       = models.CharField(max_length=20);
	author         = models.CharField(max_length=20);
	pages          = models.IntegerField();
	published_date = models.DateField();
	bookprice      = models.IntegerField();
class BookAdmin(admin.ModelAdmin):
	list_display=("bookno","bookname","author","pages","published_date","bookprice"); '

## OUTPUT
![Screenshot 2024-03-07 182848](https://github.com/tharunkumaran2006/ORM/assets/151625188/fd7e3d80-d590-4095-af76-33bfbfe9c97c)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
