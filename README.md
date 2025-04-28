# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



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
class bankloan(models.Model):
    customer_name=models.CharField(max_length=100,primary_key=True)
    customer_id=models.CharField(max_length=100)
    loan_no=models.IntegerField()
    loan_amount=models.IntegerField()
    email=models.EmailField()
 
class userAdmin(admin.ModelAdmin):
    list_display=('customer_name','customer_id','loan_no','loan_amount','email')
```
```

from django.contrib import admin
from .models import bankloan,userAdmin
admin.site.register(bankloan,userAdmin)



```


## OUTPUT
![Screenshot 2025-04-28 152617](https://github.com/user-attachments/assets/4c225809-076a-4db8-90e3-7b323d201ce7)


![Screenshot 2025-04-28 152617](https://github.com/user-attachments/assets/e10d4104-13bc-4cbb-a783-7f0655983cd1)


![Screenshot 2025-04-28 154944](https://github.com/user-attachments/assets/2b638fa8-e7b0-4fe1-bd48-4c48565aafe5)

## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
