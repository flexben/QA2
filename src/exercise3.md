## Знакомство с функционалом Swagger
---
### GET api/banks

<br>

<span style="background-color: black">Curl:</span>

    curl -X 'GET' \
    'http://94.139.255.171:5000/api/banks' \
    -H 'accept: text/plain'

<span style="background-color: black">Request URL:</span>

    http://94.139.255.171:5000/api/banks

<br>
<span style="background-color: black">Response code:</span>

    200 OK

<span style="background-color: black">Response headers:</span>

    content-type: application/json; charset=utf-8 
    date: Wed,04 Jan 2023 10:56:42 GMT 
    server: Kestrel 
    transfer-encoding: chunked 

<span style="background-color: black">Response body:</span>

    [
    {
        "bankId": "26ca687f-fd4c-4ed8-8933-29674fa2a06e",
        "name": "   ",
        "description": "   ",
        "state": 2,
        "rating": 0,
        "shortName": "   "
    },
    {
        "bankId": "e3c31276-ceaf-46fc-9259-7d7bcf0edbd9",
        "name": "***",
        "description": "*****",
        "state": 2,
        "rating": 4.6153846,
        "shortName": "*"
    },
    {
        "bankId": "fbc66253-3248-4988-8182-11024592a977",
        "name": "A-Bank",
        "description": "Описание банка",
        "state": 2,
        "rating": 1,
        "shortName": "A"
    },
    {
        "bankId": "c1b6ca0f-3ee7-4f07-b98b-c1d8ad6d30c0",
        "name": "Bank-1",
        "description": "bank",
        "state": 2,
        "rating": 5,
        "shortName": "Bank"
    },
    {
        "bankId": "f59c2d34-f2e7-43a0-a92d-c09187e540b4",
        "name": "B-Bank",
        "description": "г9з",
        "state": 2,
        "rating": 3,
        "shortName": "B-Bank"
    },
    {
        "bankId": "231d52f0-91d6-4f00-87da-e2430ed59dc8",
        "name": "B-Bank",
        "description": "B-Bank",
        "state": 2,
        "rating": 0,
        "shortName": "B-Bank"
    },
    {
        "bankId": "794f2ead-0b49-4a06-90b7-fd5617865bf4",
        "name": "string",
        "description": "string",
        "state": 2,
        "rating": 4.5,
        "shortName": "string"
    },
    {
        "bankId": "06ddc00d-e128-4019-8abd-e6e5aaa759d0",
        "name": "VK-Bank",
        "description": "vbank",
        "state": 2,
        "rating": 0,
        "shortName": "VK"
    },
    {
        "bankId": "739f3d88-1a37-44d4-96ec-42ebb21ea0fc",
        "name": "БанкЪ",
        "description": "ок",
        "state": 2,
        "rating": 0,
        "shortName": "БанкЪ"
    },
    {
        "bankId": "6bcf96a7-5947-4698-9f00-ba777b0ac6c1",
        "name": "ПАО Главный банк",
        "description": "Самый главный банк",
        "state": 2,
        "rating": 5,
        "shortName": "ГлавБанк"
    },
    {
        "bankId": "ee3eadea-49e9-4a93-8537-6bf045e0554e",
        "name": "ПАО Просто Банк",
        "description": "Простой банк",
        "state": 2,
        "rating": 0,
        "shortName": "Просто Банк"
    },
    {
        "bankId": "356c87b3-b14d-4524-a982-98aa96967674",
        "name": "ПАО Сбербанк",
        "description": "Лучший банк",
        "state": 2,
        "rating": 2.2307692,
        "shortName": "Сбер"
    },
    {
        "bankId": "7169f4ee-a7c6-4b90-a4c0-77da1bae62c1",
        "name": "Публичное акционерное общество \"Scoleray\"",
        "description": "Банк мечты",
        "state": 2,
        "rating": 0,
        "shortName": "\"Scoleray\""
    },
    {
        "bankId": "99c07aba-78df-44dc-a8c5-983310d0342d",
        "name": "цу",
        "description": "Описание банка",
        "state": 2,
        "rating": 5,
        "shortName": "A"
    }
    ]

---

### POST api/banks

<br>

<span style="background-color: black">Curl:</span>

    curl -X 'POST' \
    'http://94.139.255.171:5000/api/banks' \
    -H 'accept: text/plain' \
    -H 'Content-Type: application/json' \
    -d '{
    "name": "string",
    "description": "string",
    "shortName": "string"
    }'

<span style="background-color: black">Request URL:</span>

    http://94.139.255.171:5000/api/banks

<span style="background-color: black">Request body:</span>

    {
    "name": "string",
    "description": "string",
    "shortName": "string"
    }

<br>

<span style="background-color: black">Response code:</span>

    401 Error: Unauthorized

<span style="background-color: black">Response headers:</span>

    content-length: 0 
    date: Wed,04 Jan 2023 11:07:58 GMT 
    server: Kestrel 
    www-authenticate: Bearer 

---

### PATCH api/banks/fbc66253-3248-4988-8182-11024592a977

<br>

<span style="background-color: black">Curl:</span>

    curl -X 'PATCH' \
    'http://94.139.255.171:5000/api/banks/fbc66253-3248-4988-8182-11024592a977' \
    -H 'accept: text/plain' \
    -H 'Content-Type: application/json' \
    -d '{
    "name": "string",
    "description": "string",
    "shortName": "string"
    }'

<span style="background-color: black">Request URL:</span>

    http://94.139.255.171:5000/api/banks/fbc66253-3248-4988-8182-11024592a977

<span style="background-color: black">Request body:</span>

    {
    "name": "string",
    "description": "string",
    "shortName": "string"
    }

<br>

<span style="background-color: black">Response code:</span>

    401 Error: Unauthorized

<span style="background-color: black">Response headers:</span>

    content-length: 0 
    date: Wed,04 Jan 2023 11:20:56 GMT 
    server: Kestrel 
    www-authenticate: Bearer  

---

### DELETE api/banks/fbc66253-3248-4988-8182-11024592a977

<br>

<span style="background-color: black">Curl:</span>

    curl -X 'DELETE' \
    'http://94.139.255.171:5000/api/banks/fbc66253-3248-4988-8182-11024592a977' \
    -H 'accept: */*'

<span style="background-color: black">Request URL:</span>

    http://94.139.255.171:5000/api/banks/fbc66253-3248-4988-8182-11024592a977

<br>

<span style="background-color: black">Response code:</span>

    401 Error: Unauthorized

<span style="background-color: black">Response headers:</span>

    content-length: 0 
    date: Wed,04 Jan 2023 11:30:18 GMT 
    server: Kestrel 
    www-authenticate: Bearer

---

### GET api/banks/fbc66253-3248-4988-8182-11024592a977

<br>

<span style="background-color: black">Curl:</span>

    curl -X 'GET' \
    'http://94.139.255.171:5000/api/banks/fbc66253-3248-4988-8182-11024592a977' \
    -H 'accept: text/plain'

<span style="background-color: black">Request URL:</span>

    http://94.139.255.171:5000/api/banks/fbc66253-3248-4988-8182-11024592a977

<br>

<span style="background-color: black">Response code:</span>

    200 OK

<span style="background-color: black">Response headers:</span>

    content-type: application/json; charset=utf-8 
    date: Wed,04 Jan 2023 11:32:12 GMT 
    server: Kestrel 
    transfer-encoding: chunked  

<span style="background-color: black">Response body:</span>

    {
    "bankId": "fbc66253-3248-4988-8182-11024592a977",
    "name": "A-Bank",
    "description": "Описание банка",
    "state": 2,
    "rating": 1,
    "shortName": "A"
    }

---

### GET api/banks/Name?name=A-Bank

<br>

<span style="background-color: black">Curl:</span>

    curl -X 'GET' \
    'http://94.139.255.171:5000/api/banks/Name?name=A-Bank' \
    -H 'accept: text/plain'

<span style="background-color: black">Request URL:</span>

    http://94.139.255.171:5000/api/banks/Name?name=A-Bank

<br>

<span style="background-color: black">Response code:</span>

    200 OK

<span style="background-color: black">Response headers:</span>

    content-type: application/json; charset=utf-8 
    date: Wed,04 Jan 2023 11:34:20 GMT 
    server: Kestrel 
    transfer-encoding: chunked 

<span style="background-color: black">Response body:</span>

    [
        {
            "bankId": "fbc66253-3248-4988-8182-11024592a977",
            "name": "A-Bank",
            "description": "Описание банка",
            "state": 2,
            "rating": 1,
            "shortName": "A"
        }
    ]

---

### GET api/banks/fbc66253-3248-4988-8182-11024592a977/feedbacks

<br>

<span style="background-color: black">Curl:</span>

    curl -X 'GET' \
    'http://94.139.255.171:5000/api/banks/fbc66253-3248-4988-8182-11024592a977/feedbacks' \
    -H 'accept: text/plain'

<span style="background-color: black">Request URL:</span>

    http://94.139.255.171:5000/api/banks/fbc66253-3248-4988-8182-11024592a977/feedbacks

<br>

<span style="background-color: black">Response code:</span>

    200 OK

<span style="background-color: black">Response headers:</span>

    content-type: application/json; charset=utf-8 
    date: Wed,04 Jan 2023 11:36:28 GMT 
    server: Kestrel 
    transfer-encoding: chunked 

<span style="background-color: black">Response body:</span>

    []

---

### GET api/banks/fbc66253-3248-4988-8182-11024592a977/employee

<br>

<span style="background-color: black">Curl:</span>

    curl -X 'GET' \
    'http://94.139.255.171:5000/api/banks/fbc66253-3248-4988-8182-11024592a977/employee' \
    -H 'accept: text/plain'

<span style="background-color: black">Request URL:</span>

    http://94.139.255.171:5000/api/banks/fbc66253-3248-4988-8182-11024592a977/employee

<br>

<span style="background-color: black">Response code:</span>

    401 Error: Unauthorized

<span style="background-color: black">Response headers:</span>

    content-length: 0 
    date: Wed,04 Jan 2023 11:38:03 GMT 
    server: Kestrel 
    www-authenticate: Bearer 

---

### GET api/banks/fbc66253-3248-4988-8182-11024592a977/products

<br>

<span style="background-color: black">Curl:</span>

    curl -X 'GET' \
    'http://94.139.255.171:5000/api/banks/fbc66253-3248-4988-8182-11024592a977/products' \
    -H 'accept: text/plain'

<span style="background-color: black">Request URL:</span>

    http://94.139.255.171:5000/api/banks/fbc66253-3248-4988-8182-11024592a977/products

<br>

<span style="background-color: black">Response code:</span>

    200 OK

<span style="background-color: black">Response headers:</span>

    content-type: application/json; charset=utf-8 
    date: Wed,04 Jan 2023 11:39:15 GMT 
    server: Kestrel 
    transfer-encoding: chunked 

<span style="background-color: black">Response body:</span>

    [
    {
        "productId": "974d93c8-5830-4b0f-9479-642d1cd810ea",
        "name": "Кредит",
        "description": "",
        "state": 2,
        "avgRating": 1,
        "bankId": "fbc66253-3248-4988-8182-11024592a977",
        "categoryId": "3d2e08da-5c02-41be-ba43-980058730621"
    },
    {
        "productId": "624fbd5b-8d04-496d-bb93-d1a6c7de2010",
        "name": "Кредит",
        "description": "",
        "state": 2,
        "avgRating": 1,
        "bankId": "fbc66253-3248-4988-8182-11024592a977",
        "categoryId": "3d2e08da-5c02-41be-ba43-980058730621"
    },
    {
        "productId": "8b804821-d66c-44f9-b5c4-e9c29631e7b5",
        "name": "Кредит",
        "description": "",
        "state": 2,
        "avgRating": 1,
        "bankId": "fbc66253-3248-4988-8182-11024592a977",
        "categoryId": "3d2e08da-5c02-41be-ba43-980058730621"
    },
    {
        "productId": "b10c2163-cd39-43a6-9854-dd776a954df3",
        "name": "Кредит",
        "description": "",
        "state": 2,
        "avgRating": 1,
        "bankId": "fbc66253-3248-4988-8182-11024592a977",
        "categoryId": "3d2e08da-5c02-41be-ba43-980058730621"
    },
    {
        "productId": "a8735191-8216-4930-a9d1-7e2ea71164aa",
        "name": "Кредит",
        "description": "",
        "state": 2,
        "avgRating": 1,
        "bankId": "fbc66253-3248-4988-8182-11024592a977",
        "categoryId": "3d2e08da-5c02-41be-ba43-980058730621"
    },
    {
        "productId": "fc478fca-1b55-4566-adc7-1ce4cb254199",
        "name": "Кредит",
        "description": "",
        "state": 2,
        "avgRating": 1,
        "bankId": "fbc66253-3248-4988-8182-11024592a977",
        "categoryId": "3d2e08da-5c02-41be-ba43-980058730621"
    }
    ]

---

### POST api/authorization/register

<br>

<span style="background-color: black">Curl:</span>

    curl -X 'POST' \
    'http://94.139.255.171:5000/api/authorization/register' \
    -H 'accept: text/plain' \
    -H 'Content-Type: application/json' \
    -d '{
    "name": "User",
    "birthday": "2023-01-04T12:04:38.597Z",
    "sex": 0,
    "email": "user1234@example.com",
    "password": "string",
    "roleId": "b6ac9a45-4032-4289-b439-2cc4d65c3f18"
    }'

<span style="background-color: black">Request URL:</span>

    http://94.139.255.171:5000/api/authorization/register

<span style="background-color: black">Request body:</span>

    {
    "name": "User",
    "birthday": "2023-01-04T12:04:38.597Z",
    "sex": 0,
    "email": "user1234@example.com",
    "password": "string",
    "roleId": "b6ac9a45-4032-4289-b439-2cc4d65c3f18"
    }

<br>

<span style="background-color: black">Response code:</span>

    201

<span style="background-color: black">Response headers:</span>

    content-type: application/json; charset=utf-8 
    date: Wed,04 Jan 2023 12:04:29 GMT 
    location: /api/users/fe9ee77a-f434-4bc9-b1b0-fc10253b6a0c 
    server: Kestrel 
    transfer-encoding: chunked  

<span style="background-color: black">Response body:</span>

    {
    "userId": "fe9ee77a-f434-4bc9-b1b0-fc10253b6a0c",
    "name": "User",
    "birthaday": "2023-01-04T12:04:38.597Z",
    "sex": 0,
    "email": "user1234@example.com",
    "roleId": "b6ac9a45-4032-4289-b439-2cc4d65c3f18",
    "bankId": null,
    "state": 0
    }

---

### POST api/authorization/login

<br>

<span style="background-color: black">Curl:</span>

    curl -X 'POST' \
    'http://94.139.255.171:5000/api/authorization/login' \
    -H 'accept: text/plain' \
    -H 'Content-Type: application/json' \
    -d '{
    "email": "admin@mail.ru",
    "password": "Admin"
    }'

<span style="background-color: black">Request URL:</span>

    http://94.139.255.171:5000/api/authorization/login

<span style="background-color: black">Request body:</span>

    {
    "email": "admin@mail.ru",
    "password": "Admin"
    }

<br>

<span style="background-color: black">Response code:</span>

    200

<span style="background-color: black">Response headers:</span>

    content-type: text/plain; charset=utf-8 
    date: Wed,04 Jan 2023 11:49:37 GMT 
    server: Kestrel 
    transfer-encoding: chunked 

<span style="background-color: black">Response body:</span>

    eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTUxMiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI3Y2JiNWZiOS0zYmQzLTQ1MmYtOTc5NS02NmM3NDU4YmIzNTMiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoiQWRtaW4iLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9lbWFpbGFkZHJlc3MiOiJhZG1pbkBtYWlsLnJ1IiwiaHR0cDovL3NjaGVtYXMubWljcm9zb2Z0LmNvbS93cy8yMDA4LzA2L2lkZW50aXR5L2NsYWltcy9yb2xlIjoiQWRtaW4iLCJleHAiOjE2NzI4MzQ4MTd9.6D2DVK50IZXoZgrLzp-5Ica4XSSWmktSDSlZrPeBM0oaV8u8osrDaOzLeABMQ_d43usj_ai1KEzt8VhIsUD1mw

---

### POST api/banks

<br>

<span style="background-color: black">Curl:</span>

    curl -X 'POST' \
    'http://94.139.255.171:5000/api/banks' \
    -H 'accept: text/plain' \
    -H 'Authorization: bearer eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTUxMiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI3Y2JiNWZiOS0zYmQzLTQ1MmYtOTc5NS02NmM3NDU4YmIzNTMiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoiQWRtaW4iLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9lbWFpbGFkZHJlc3MiOiJhZG1pbkBtYWlsLnJ1IiwiaHR0cDovL3NjaGVtYXMubWljcm9zb2Z0LmNvbS93cy8yMDA4LzA2L2lkZW50aXR5L2NsYWltcy9yb2xlIjoiQWRtaW4iLCJleHAiOjE2NzI4MzQ4MTd9.6D2DVK50IZXoZgrLzp-5Ica4XSSWmktSDSlZrPeBM0oaV8u8osrDaOzLeABMQ_d43usj_ai1KEzt8VhIsUD1mw' \
    -H 'Content-Type: application/json' \
    -d '{
    "name": "NewBank",
    "description": "Description",
    "shortName": "Shortname"
    }'

<span style="background-color: black">Request URL:</span>

    http://94.139.255.171:5000/api/banks

<br>

<span style="background-color: black">Response code:</span>

    201

<span style="background-color: black">Response headers:</span>

    content-type: application/json; charset=utf-8 
    date: Wed,04 Jan 2023 11:50:47 GMT 
    location: /api/banks/62ab904e-af94-4da5-83a5-38c6c0177924 
    server: Kestrel 
    transfer-encoding: chunked 

<span style="background-color: black">Response body:</span>

    {
    "bankId": "62ab904e-af94-4da5-83a5-38c6c0177924",
    "name": "NewBank",
    "description": "Description",
    "state": 2,
    "rating": 0,
    "shortName": "Shortname"
    }

---

### PATCH api/banks/fbc66253-3248-4988-8182-11024592a977

<br>

<span style="background-color: black">Curl:</span>

    curl -X 'PATCH' \
    'http://94.139.255.171:5000/api/banks/fbc66253-3248-4988-8182-11024592a977' \
    -H 'accept: text/plain' \
    -H 'Authorization: bearer eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTUxMiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI3Y2JiNWZiOS0zYmQzLTQ1MmYtOTc5NS02NmM3NDU4YmIzNTMiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoiQWRtaW4iLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9lbWFpbGFkZHJlc3MiOiJhZG1pbkBtYWlsLnJ1IiwiaHR0cDovL3NjaGVtYXMubWljcm9zb2Z0LmNvbS93cy8yMDA4LzA2L2lkZW50aXR5L2NsYWltcy9yb2xlIjoiQWRtaW4iLCJleHAiOjE2NzI4MzQ4MTd9.6D2DVK50IZXoZgrLzp-5Ica4XSSWmktSDSlZrPeBM0oaV8u8osrDaOzLeABMQ_d43usj_ai1KEzt8VhIsUD1mw' \
    -H 'Content-Type: application/json' \
    -d '{
    "name": "A-Bank",
    "description": "New des",
    "shortName": "A"
    }'

<span style="background-color: black">Request URL:</span>

    http://94.139.255.171:5000/api/banks/fbc66253-3248-4988-8182-11024592a977

<br>

<span style="background-color: black">Response code:</span>

    200 Success

<span style="background-color: black">Response headers:</span>

    content-type: application/json; charset=utf-8 
    date: Wed,04 Jan 2023 11:52:12 GMT 
    server: Kestrel 
    transfer-encoding: chunked 

<span style="background-color: black">Response body:</span>

    {
    "bankId": "fbc66253-3248-4988-8182-11024592a977",
    "name": "A-Bank",
    "description": "New des",
    "state": 2,
    "rating": 0,
    "shortName": "A"
    }

---

### GET api/banks/356c87b3-b14d-4524-a982-98aa96967674/employee

<br>

<span style="background-color: black">Curl:</span>

    curl -X 'GET' \
    'http://94.139.255.171:5000/api/banks/356c87b3-b14d-4524-a982-98aa96967674/employee' \
    -H 'accept: text/plain' \
    -H 'Authorization: bearer eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTUxMiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI3Y2JiNWZiOS0zYmQzLTQ1MmYtOTc5NS02NmM3NDU4YmIzNTMiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoiQWRtaW4iLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9lbWFpbGFkZHJlc3MiOiJhZG1pbkBtYWlsLnJ1IiwiaHR0cDovL3NjaGVtYXMubWljcm9zb2Z0LmNvbS93cy8yMDA4LzA2L2lkZW50aXR5L2NsYWltcy9yb2xlIjoiQWRtaW4iLCJleHAiOjE2NzI4MzQ4MTd9.6D2DVK50IZXoZgrLzp-5Ica4XSSWmktSDSlZrPeBM0oaV8u8osrDaOzLeABMQ_d43usj_ai1KEzt8VhIsUD1mw'

<span style="background-color: black">Request URL:</span>

    http://94.139.255.171:5000/api/banks/356c87b3-b14d-4524-a982-98aa96967674/employee

<br>

<span style="background-color: black">Response code:</span>

    200 Success

<span style="background-color: black">Response headers:</span>

    content-type: application/json; charset=utf-8 
    date: Wed,04 Jan 2023 11:56:50 GMT 
    server: Kestrel 
    transfer-encoding: chunked 

<span style="background-color: black">Response body:</span>

    []

---