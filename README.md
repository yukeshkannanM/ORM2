# Ex02 Django ORM Web Application
## Date: 17.12.2025

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
Execute Django admin and create details for 5 Car 

## PROGRAM
 ```
from django.db import models
from django.contrib import admin
class Car(models.Model):
    brand_name=models.CharField(max_length=20)
    car_name=models.CharField(max_length=10)
    enginenum=models.IntegerField()
    release_date=models.DateField()

class CarAdmin(admin.ModelAdmin):
 list_display=('brand_name', 'car_name', 'enginenum', 'release_date')

admin.py:

from django.contrib import admin
from.models import Car,CarAdmin
admin.site.register(Car,CarAdmin)
```

Include Your program

## OUTPUT
<img width="1919" height="1079" alt="Screenshot 2026-01-04 164536" src="https://github.com/user-attachments/assets/23ec6843-7f5d-4a4e-9152-15afe0a8df72" />




## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
