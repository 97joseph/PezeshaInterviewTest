## Payment Api

### Project setup
1. Rename `.env.example` file into `.env`. Edit data in this file if you want to (admin credentials, server port and et cetera).
2. Run `npm i` command to install dependencies from `package.json` file.
3. Run `npm start` shortcut command to start an API server.

### Route names with examples
#### /auth
Being called with login/password credentials and returns authorization token in response.
```
POST /auth
{
    "login": "admin",
    "password": "admin" 
}
```

#### /users
User creation/deletion/reading.
```
* requires authorization token (bearer) to be provided

POST /users
no query parameters or body data needed in request

DELETE /users
{
    "id": "887c6399-55e3-4b15-8c84-39b5ddb3e40c"
}

GET /users
* may be called with or without (!) query parameter (!) "id"
?id=887c6399-55e3-4b15-8c84-39b5ddb3e40c
```

#### /transactions
Transaction creation/deletion/reading.
```
* requires authorization token (bearer) to be provided

POST /transactions
{
    "from": "cc8c855f-8130-4473-9bb5-c5a8cdb149a8",
    "to": "9a76b67c-19bf-4310-ab7c-7c7ef4d18860",
    "amount": 100
}

GET /transactions
{
    "id": "887c6399-55e3-4b15-8c84-39b5ddb3e40c"
}

GET /transactions
* may be called with or without (!) query parameter (!) "id"
?id=887c6399-55e3-4b15-8c84-39b5ddb3e40c
```

#### /config
Config edit and project reset (data wipe).
```
* requires authorization token (bearer) to be provided

GET /config
no query parameters or body data needed in request

PATCH /config
* config options may be changed separately 
{
    "number_of_entries": 6,
    "initial_amount": 500
}


DELETE /config
no query parameters or body data needed in request
```



![Screenshot (121)](https://user-images.githubusercontent.com/33089347/218465146-707806c7-66fb-49e4-a93e-3a02a4a22be2.png)

## API Groupings

<img width="223" alt="API Structure" src="https://user-images.githubusercontent.com/33089347/218465156-955b9559-e7a1-45f9-b78a-0e5913c05da0.PNG">

