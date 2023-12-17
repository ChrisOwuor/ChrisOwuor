<h1 align="center">Hi 👋, I'm Chrispine</h1>
<h3 align="center">A passionate software developer</h3>
- 🌱 I’m currently learning **Machine learning and cybersecurity**

- 👨‍💻 All of my projects are available at [https://github.com/ChrisOwuor](https://github.com/ChrisOwuor)
- 💬 Ask me about **react,django,node ,sql ,nosql and computer networking**

<h3 align="left">Connect with me:</h3>
<p align="left">
<a href="https://www.linkedin.com/in/chrispine-owuor-23363525b" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="chrispine owuor" height="30" width="40" /></a>
<a href="https://instagram.com/__lomoh" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/instagram.svg" alt="__lomo" height="30" width="40" /></a>
</p>

<h3 align="left">Languages and Tools:</h3>
<p align="center">  <a href="https://babeljs.io/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/babeljs/babeljs-icon.svg" alt="babel" width="40" height="40"/> </a> <a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/> </a> <a href="https://www.djangoproject.com/" target="_blank" rel="noreferrer"> <img src="https://cdn.worldvectorlogo.com/logos/django.svg" alt="django" width="40" height="40"/> </a> <a href="https://expressjs.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/express/express-original-wordmark.svg" alt="express" width="40" height="40"/> </a> <a href="https://git-scm.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="git" width="40" height="40"/> </a> <a href="https://www.w3.org/html/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> </a> <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> </a> <a href="https://www.mongodb.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mongodb/mongodb-original-wordmark.svg" alt="mongodb" width="40" height="40"/> </a> <a href="https://www.mysql.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="mysql" width="40" height="40"/> </a> <a href="https://nodejs.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original-wordmark.svg" alt="nodejs" width="40" height="40"/> </a>  <a href="https://www.postgresql.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original-wordmark.svg" alt="postgresql" width="40" height="40"/> </a> <a href="https://postman.com" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/getpostman/getpostman-icon.svg" alt="postman" width="40" height="40"/> </a> <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> <a href="https://reactjs.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" alt="react" width="40" height="40"/> </a> <a href="https://reactnative.dev/" target="_blank" rel="noreferrer"> <img src="https://reactnative.dev/img/header_logo.svg" alt="reactnative" width="40" height="40"/> </a> <a href="https://tailwindcss.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/tailwindcss/tailwindcss-icon.svg" alt="tailwind" width="40" height="40"/> </a> <a href="https://webpack.js.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/d00d0969292a6569d45b06d3f350f463a0107b0d/icons/webpack/webpack-original-wordmark.svg" alt="webpack" width="40" height="40"/> </a> </p>

# Microfinance API Documentation

## Introduction

Welcome to the Microfinance API designed to facilitate seamless communication between VisionFund Kenya's financial services and other microfinance institutions or related entities. This documentation provides an overview of the API's features, endpoints, and usage guidelines.

### API Base URL

`https://api.visionfundmicrofinance.com`

## 1. User Management

### 1.1 Create client Profile

**Endpoint:**

`POST /users`

**Description:**

Create a new client profile with personal details.

**Request:**

```json
{
  "name": "John Doe",
  "email": "john.doe@example.com",
  "role": "client",
  "id_number":"1234567"
}
```

**Response:**

``` json
{
  "id": 123,
  "name": "John Doe",
  "email": "john.doe@example.com",
  "role": "client",
//   generated acount number
  "a/c":"john1234567",
}
```

### 1.2 Create user Profile

**Endpoint:**

`POST /users`

**Description:**

Create a new user profile with personal details.

**Request:**

```json
{
  "name": "John Doe",
  "email": "john.doe@example.com",
  "role": "user",
}
```

**Response:**

``` json
{
  "id": 123,
  "name": "John Doe",
  "email": "john.doe@example.com",
  "role": "user",
//   generated acount number
}
```

### 1.3 Authentication

**Endpoint:**

`POST /auth/token`

**Description:**

Obtain an authentication token for API access.

**Request:**

```json
{
  "username": "john.doe@example.com",
  "password": "securepassword"
}
```

**Response:**

```json
{
  "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9..."
}

```

## 2. Transaction Handling

### **Transactions by client**

* ### Client Withdrawals

* ### Client Deposit

* ### Client Loan Repayment

### **Transactions by user**

* ### loan disbursment to either mpesa or account

### 2.1 All Transactions by  for an individual client

**Endpoint:**

`POST api/transactions/{client_id}`

**Description:**

Record a financial transaction for a client

**Request:**

``` json
{
  "token": "q1w2e3r4t5t65",
}
```

**Response:**

``` json
{
  "id": 456,
  "code":"qwerty12",
  "user_id": 123,
  "amount": 100.00,
  "type": "withdrawal / deposit / loan repayment ",
  "time":"12:23:45",
  "date":"2/3/2024"


}
```

### 2.1 loan disbursment transaction

**Endpoint:**

`POST api/transactions/disburse/{client_id}`

**Description:**

Make  loan disbursment to a client

**Request:**

``` json
{
  "amount":233,
  "user_token": "q1w2e3r4t5t65",
}
```

**Response:**.

``` json
{
  "id": 456,
  "by":"user_id",
  "code":"qwerty12",
  "user_id": 123,
  "amount": 233.00,
  "type": "disbursement",
  "time":"12:23:45",
  "date":"2/3/2024"

}
```

### 2.3 loan repayment by client transaction

**Endpoint:**

`POST api/transactions/loans/repayment/{client_id}`

**Description:**

Make  loan repayment by a client

**Request:**

``` json
{
"source":"mpesa /account",
  "amount":233,
  "client_token": "q1w2e3r4t5t65",
}
```

**Response:**.

``` json
{
  "id": 456,
  "code":"qwerty12",
  "amount": 233.00,
  "time":"12:23:45",
  "date":"2/3/2024",
  "balance":"289"

}
```

### 2.4 client deposit transaction

**Endpoint:**

`POST api/transactions/deposit/{client_id}`

**Description:**

Make  a deposit transaction by a client

**Request:**

``` json
{
"source":"mpesa",
  "amount":233,
  "client_token": "q1w2e3r4t5t65",
}
```

**Response:**.

``` json
{
  "id": 456,
  "code":"qwerty12",
  "time":"12:23:45",
  "date":"2/3/2024",
  "balance":"22"

}
```

### 2.5 client withdrawal transaction

**Endpoint:**

`POST api/transactions/deposit/{client_id}`

**Description:**

Make  a withdrawal transaction by a client

**Request:**

``` json
{
  "amount":233,
  "client_token": "q1w2e3r4t5t65",
}
```

**Response:**.

``` json
{
  "id": 456,
  "code":"qwerty12",
  "time":"12:23:45",
  "date":"2/3/2024",
  "balance":"22"

}
```

## 3. Loan Information

### **Loan information types**

* ### get all loans by client

* ### get pending loans by client

* ### get all loans both pending and previous for a single client by the third party

### 3.1 Loan Details

**Endpoint:**

`GET /loans/{user_id}`

**Description:**

Retrieve loan details for a specific user.

**Request:**

``` json
{
  "client_token": "q1w2e3r4t5t65",
}
```

**Response:**

``` json
{
  "user_id": 123,
  "loan_amount": 5000.00,
  "repayment_schedule": "monthly",
  "outstanding_amount": 2500.00,
  "status": "approved"
}
```


