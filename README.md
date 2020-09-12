# OTP_django
Quick and simple technique to implement the OTP functionality in your Django Project.

### Python Packages required: ```pyotp, base64, django, django-rest-framework```
OTP is generated via the random function with respect to current time in system.

## API Calls

#### GET 
This is to register the mobile number into the database and generate OTP.

```http://127.0.0.1:8000/verify/<phone_num>/```
eg.
```http://127.0.0.1:8000/verify/9140444258/```
![alt text](https://github.com/Saumitra-Shukla/OTP_Django/blob/master/photos/Screenshot from 2020-09-12 21-07-19.png?raw=true)

In the Django Admin Panel:
![alt text](https://github.com/Saumitra-Shukla/OTP_Django/blob/master/photos/Screenshot from 2020-09-12 21-22-24.png?raw=true)


#### POST
This is to verify the mobile number using OTP.

```http://127.0.0.1:8000/verify/<phone_num>/```
eg.
```http://127.0.0.1:8000/verify/9140444258/```

![alt text](https://github.com/Saumitra-Shukla/OTP_Django/blob/master/photos/Screenshot from 2020-09-12 21-16-05.png?raw=true)

Data: 
```
   {
    "otp":546036
   }
```

After POST req:
![alt text](https://github.com/Saumitra-Shukla/OTP_Django/blob/master/photos/Screenshot from 2020-09-12 21-16-15.png?raw=true)

In the Django Admin Panel:
![alt text](https://github.com/Saumitra-Shukla/OTP_Django/blob/master/photos/Screenshot from 2020-09-12 21-22-42.png?raw=true)


