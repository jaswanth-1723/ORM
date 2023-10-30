# Ex02 Django ORM Web Application
## DATE:28/10/2023 

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

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

Model.py
```
from django.db import models
from django.contrib import admin
class Player(models.Model):
    Player_Name=models.CharField(max_length=50)
    Jersy_No=models.IntegerField()
    Team=models.CharField(max_length=20)
    Height=models.IntegerField()
    Position=models.CharField(max_length=100)

class Player_Admin(admin.ModelAdmin):
    list_display=('Player_Name','Jersy_No','Team','Height','Position')
```

Admin.py
```
from django.contrib import admin
from .models import Player,Player_Admin
admin.site.register(Player,Player_Admin)
```

## OUTPUT
![expp](https://github.com/jaswanth-1723/ORM/assets/127680667/ca1ac4e6-65a6-44c5-a6d0-21dcfe5f2e3b)

![exp 4](https://github.com/jaswanth-1723/ORM/assets/127680667/e802cde0-5953-4b88-825e-0ea235892df5)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
