### test code for submit test backnd

# How to run

1. git code this repo
2. npm install
3. copy .env.test .env
4. npm run dev

result in below
```bash
[INFO] 06:07:08 ts-node-dev ver. 2.0.0 (using ts-node ver. 10.9.2, typescript ver. 5.4.5)
Server is listening on port 3000
```

# How to test [ need install 'REST Client' in vscode.]

go to test directory


```code
@baseUrl = http://localhost:3000
### create new users
POST {{baseUrl}}/signup
Content-Type: application/json

{
    "username": "wirat",
    "email" : "test@email.com",
    "password": "P@ssword"
}

### login by email
POST {{baseUrl}}/signin
Content-Type: application/json

{
    "email" : "test@email.com",
    "password": "P@ssword"
}

### get all users
GET {{baseUrl}}/users
Content-Type: application/json

### get a singer user by id
GET {{baseUrl}}/users/bf3f9532-c09e-406a-aa7a-86b251317d67
Content-Type: application/json

### update user by id
PUT {{baseUrl}}/users/bf3f9532-c09e-406a-aa7a-86b251317d67
Content-Type: application/json

{
    "username": "sample",
    "email" : "update@email.com",
    "password": "P@ssword"
}

### delete user by enter id {{}}
DELETE  {{baseUrl}}/users/{{?}}
Content-Type: application/json

```

