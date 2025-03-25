# Ex02 Django ORM Web Application
## Name: VASANTH N
## ROLL NO: 212224110060
## Date: 25-03-2025

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![Screenshot 2025-03-25 071413](https://github.com/user-attachments/assets/9fc62c1b-a371-4640-983f-6c96b2b867dc)


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
models.py

        from django.db import models
        from django.contrib import admin
        class customer (models.Model):
            c_id=models.IntegerField(primary_key=True)
            name=models.CharField(max_length=100)
            salary=models.IntegerField()
            age=models.IntegerField()
            email=models.EmailField()
         
        class customerAdmin(admin.ModelAdmin):
            list_display=('c_id','name','salary','age','email')
         
admin.py

        from django.contrib import admin
        from .models import customer,customerAdmin
        admin.site.register(customer,customerAdmin)
        
## OUTPUT
![Screenshot 2025-03-25 071431](https://github.com/user-attachments/assets/90cc1420-ecac-45a1-9b63-38bda8c76473)


## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
