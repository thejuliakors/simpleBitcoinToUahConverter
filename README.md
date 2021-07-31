# Software Engineering School Test Task
## Simple Web API

Web API для сервісу, який дозволить зареєструвати та аутентифікувати користувача, а для аутентифікованих користувачів дізнатись поточний курс біткоіну (BTC) у гривні (UAH)

## Versions
node: v10.19.0

npm: 7.19.0

Other packages' versions specified in package.json file.

## Installation
```
https://github.com/thejuliakors/simpleAPITestTask.git
```
```
npm install
```
```
npm start
```

## Routes
Url: [localhost:3000](localhost:3000)
```
/user/create
```
Register new user with email and password. Email must be unique and valid.
```
/user/login
```
Sign in with previously registered user by email and password combination. 

⚠️ In case of successful login, you'll receive a JWT token, which should be used as a value of Authorization header for the next route.
```
/btcRate
```
Get BTC rate relatively to UAH for logged in users.

## Data storage
All user data will be saved to users.json file (specified in constants.js).

## Currency rate API
In this project [Kuna API v3](https://github.com/kunadevelopers/api-docs) was used.