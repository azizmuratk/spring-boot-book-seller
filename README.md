#Spring Boot Book Seller

###Endpoints
####Sign-up
```
POST /api/authentication/sign-up HTTP/1.1
Host: localhost:8080
Content-Type: application/json
{
"name": "user",
"username": "user",
"password": "user"
}
```
####Sign-in
```
POST /api/authentication/sign-in HTTP/1.1
Host: localhost:8080
Content-Type: application/json
{
"username": "user",
"password": "user"
}
```

####Save Book

```
POST /api/book HTTP/1.1
Host: localhost:8080
Authorization: Bearer eyJhbGciOiJIUzUxMiJ9.eyJzdWIiOiJhZG1pbjEiLCJyb2xlcyI6IlJPTEVfVVNFUiIsInVzZXJJZCI6NCwiZXhwIjoxNjMwOTI0ODUzfQ.wSaMEYJvHynwdVjDF6XKafK8KKImjIov6TQ_-b7G1ovFU8nJ5QKJB84Iet8iBKvxgahn_-cktMkDE0N7sfddLw
Content-Type: application/json
Content-Length: 119

{
"title": "Test Book 4",
"price": 40,
"description": "Test Description 4",
"author": "Test Author 4"
}
```