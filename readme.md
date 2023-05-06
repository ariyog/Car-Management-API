# Challenge - 5
Membuat Open API Documentation dari REST API dengan Authentikasi

## Link Dokumentasi Public API
https://documenter.getpostman.com/view/25191103/2s93eX2Dka

## Email dan Password Login SuperAdmin
email : ariyogi@superadmin.com
password : 123456

## Endpoint
### (POST) Login Superadmin
> http://localhost:5000/v1/api/login
* Example request

{
    "email": "ariyogi@superadmin.com",
    "password": "123456"
}

### (POST) Login Member
> http://localhost:5000/v1/api/login
* Example Request
{
    "email": "member1@gmail.com",
    "password": "123456"
}

### (POST) Login Admin
> http://localhost:5000/v1/api/login
* Example Request
{
    "email": "admin1@gmail.com",
    "password": "123456"
}   

### (GET) Get User Data
> http://localhost:5000/v1/api/users
* need barier token auth

### Logout
> http://localhost:5000/v1/api/logout
* need barier token auth

### (GET) Get All Data Cars
> http://localhost:5000/v1/api/cars
* Example Request
curl --location --request GET 'http://localhost:5000/v1/api/cars' \
--data-raw '{
    "email": "ariyogi@superadmin.com",
    "password": "123456"
}'

### (GET) Get Car by ID
> http://localhost:5000/v1/api/car/1
* Example Request
curl --location --request GET 'http://localhost:5000/v1/api/car/1' \
--data-raw '{
    "email": "ariyogi@superadmin.com",
    "password": "123456"
}'

### (PUT) Delete Car
> http://localhost:5000/v1/api/car/1
* Example Request
curl --location --request PUT 'http://localhost:5000/v1/api/car/8' \
--data-raw '{
    "email": "ariyogi@superadmin.com",
    "password": "123456"
}'

### (PUT) Update Car
> http://localhost:5000/v1/api/updatecar/1
* Example Request
curl --location --request PUT 'http://localhost:5000/v1/api/updatecar/3' \
--data '{
    "nama":"jazz update2",
    "harga":"200000"
}'

### (POST) Create Car
> http://localhost:5000/v1/api/createcar
* Example Request
curl --location 'http://localhost:5000/v1/api/createcar' \
--header 'nama: jazz2' \
--header 'harga: 15000' \
--data '{
    "nama":"L-300",
    "harga":"190888"
}'

### (GET) Deleted Car
> http://localhost:5000/v1/api/deletedcar
* Example Request
curl --location --request GET 'http://localhost:5000/v1/api/deletedcar' \
--data-raw '{
    "email": "ariyogi@superadmin.com",
    "password": "123456"
}'
