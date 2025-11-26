# Ex02 Django ORM Web Application
# Date:26-11-2025
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 cars

# PROGRAM
from django.contrib import admin
from.models import Car,CarAdmin
admin.site.register(Car,CarAdmin)

from django.db import models
from django.contrib import admin
class Car(models.Model):
    car_name= models.CharField()
    car_model = models.CharField()
    release_date = models.DateField()
    millage = models.IntegerField()
    color = models.CharField()

class CarAdmin(admin.ModelAdmin):
    list_display = ('car_name', 'car_model', 'release_date', 'millage', 'color')
# OUTPUT
Include the screenshot of your admin page.
![ORM output](https://github.com/user-attachments/assets/b5c49e4c-c94c-422a-bbb3-38687e0e6a59)

# RESULT
Thus the program for creating a database using ORM hass been executed successfully
