Навигация по запросам:

|ex.5 |  
|---|
|[GET /api/banks](#get-apibanks)|

|ex.6 |   |
|---|---|
|[Тест-кейс №39](#отчёт-по-тест-кейсу-№39)|[Тест-кейс №59](#отчёт-по-тест-кейсу-№59)|
|[Тест-кейс №40](#отчёт-по-тест-кейсу-№40)|[Тест-кейс №60](#отчёт-по-тест-кейсу-№60)|
|[Тест-кейс №41](#отчёт-по-тест-кейсу-№41)|[Тест-кейс №61](#отчёт-по-тест-кейсу-№61)|
|[Тест-кейс №42](#отчёт-по-тест-кейсу-№42)|[Тест-кейс №62](#отчёт-по-тест-кейсу-№62)|
|[Тест-кейс №43](#отчёт-по-тест-кейсу-№43)|[Тест-кейс №63](#отчёт-по-тест-кейсу-№63)|
|[Тест-кейс №44](#отчёт-по-тест-кейсу-№44)|[Тест-кейс №64](#отчёт-по-тест-кейсу-№64)|
|[Тест-кейс №45](#отчёт-по-тест-кейсу-№45)|[Тест-кейс №65](#отчёт-по-тест-кейсу-№65)|
|[Тест-кейс №46](#отчёт-по-тест-кейсу-№46)|[Тест-кейс №66](#отчёт-по-тест-кейсу-№66)|
|[Тест-кейс №47](#отчёт-по-тест-кейсу-№47)|[Тест-кейс №67](#отчёт-по-тест-кейсу-№67)|
|[Тест-кейс №48](#отчёт-по-тест-кейсу-№48)|[Тест-кейс №68](#отчёт-по-тест-кейсу-№68)|
|[Тест-кейс №49](#отчёт-по-тест-кейсу-№49)|[Тест-кейс №69](#отчёт-по-тест-кейсу-№69)|
|[Тест-кейс №50](#отчёт-по-тест-кейсу-№50)|[Тест-кейс №70](#отчёт-по-тест-кейсу-№70)|
|[Тест-кейс №52](#отчёт-по-тест-кейсу-№52)|[Тест-кейс №71](#отчёт-по-тест-кейсу-№71)|
|[Тест-кейс №53](#отчёт-по-тест-кейсу-№53)|[Тест-кейс №72](#отчёт-по-тест-кейсу-№72)|
|[Тест-кейс №54](#отчёт-по-тест-кейсу-№54)|[Тест-кейс №73](#отчёт-по-тест-кейсу-№73)|
|[Тест-кейс №55](#отчёт-по-тест-кейсу-№55)|[Тест-кейс №74](#отчёт-по-тест-кейсу-№74)|
|[Тест-кейс №56](#отчёт-по-тест-кейсу-№56)|[Тест-кейс №75](#отчёт-по-тест-кейсу-№75)|
|[Тест-кейс №57](#отчёт-по-тест-кейсу-№57)|[Тест-кейс №76](#отчёт-по-тест-кейсу-№76)|
|[Тест-кейс №58](#отчёт-по-тест-кейсу-№58)|[Тест-кейс №77](#отчёт-по-тест-кейсу-№77)|

# GET /api/banks
## URL :

    http://94.139.255.171:5000/api/banks

## Ожидаемый результат:

    Ответ с кодом 200 и телом, содержащим список всех банков с параметрами "bankId": "name": "description": "state": "rating": "shortName":


## Заголовки запроса:

    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: 256b73f1-476b-4e15-bcad-7e86f85e698f
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive

## Тело запроса:

    -

## Заголовки ответа:

    Content-Type: application/json; charset=utf-8
    Date: Mon, 09 Jan 2023 20:00:43 GMT
    Server: Kestrel
    Transfer-Encoding: chunked

## Тело ответа (часть):

    [
        {
            "bankId": "50468565-602c-41e5-8562-fc124718bb5a",
            "name": "",
            "description": "",
            "state": 2,
            "rating": 0,
            "shortName": ""
        },
        {
            "bankId": "e3c31276-ceaf-46fc-9259-7d7bcf0edbd9",
            "name": "***",
            "description": "*****",
            "state": 2,
            "rating": 4.6153846,
            "shortName": "*"
        },
    ...

## Особенности запроса:
    
    Авторизация не требуется

---

# Отчёт по тест кейсу №39
## URL :

    http://94.139.255.171:5000/api/authorization/register

## Ожидаемый результат:

    Получен ответ с кодом 201 и телом, содержащим параметры "userId": "name": "birthaday": "sex": "email": "roleId": "bankId": "state":


## Заголовки запроса:

    Content-Type: application/json
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: c5958478-dc6c-4def-acad-23302c3eb3f4
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive

## Тело запроса:

    {
    "name": "newclient",
    "birthday": "2023-01-10T11:15:18.002Z",
    "sex": 0,
    "email": "usertest123@example.com",
    "password": "qweasd123",
    "roleId": "b6ac9a45-4032-4289-b439-2cc4d65c3f18"
    }

## Заголовки ответа:

    Content-Type: application/json; charset=utf-8
    Date: Tue, 10 Jan 2023 11:17:38 GMT
    Server: Kestrel
    Location: /api/users/830ea4d4-e70c-477c-b025-ab265cb20b4b
    Transfer-Encoding: chunked

## Тело ответа:

    {
        "userId": "830ea4d4-e70c-477c-b025-ab265cb20b4b",
        "name": "newclient",
        "birthaday": "2023-01-10T11:15:18.002Z",
        "sex": 0,
        "email": "usertest123@example.com",
        "roleId": "b6ac9a45-4032-4289-b439-2cc4d65c3f18",
        "bankId": null,
        "state": 0
    }

## Особенности запроса:
    
    Авторизация не требуется

---

# Отчёт по тест кейсу №40
## URL :

    http://94.139.255.171:5000/api/authorization/register

## Ожидаемый результат:

    Получен ответ с кодом 201 и телом, содержащим параметры "userId": "name": "birthaday": "sex": "email": "roleId": "bankId": "state":


## Заголовки запроса:

    Content-Type: application/json
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: a70c651e-4db2-43fc-ba3d-d6af5fed27e7
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive

## Тело запроса:

    {
    "name": "newemployee",
    "birthday": "2023-01-10T11:15:18.002Z",
    "sex": 0,
    "email": "usertestempl123@example.com",
    "password": "qweasd123",
    "roleId": "2258b464-f412-4ccd-80f4-6ec3053fd4a5",
    "bankId": "356c87b3-b14d-4524-a982-98aa96967674"
    }

## Заголовки ответа:

    Content-Type: application/json; charset=utf-8
    Date: Tue, 10 Jan 2023 11:25:47 GMT
    Server: Kestrel
    Location: /api/users/b7dd1bbe-ed77-4fd8-be7f-3d6678be1dc2
    Transfer-Encoding: chunked

## Тело ответа:

    {
        "userId": "b7dd1bbe-ed77-4fd8-be7f-3d6678be1dc2",
        "name": "newemployee",
        "birthaday": "2023-01-10T11:15:18.002Z",
        "sex": 0,
        "email": "usertestempl123@example.com",
        "roleId": "2258b464-f412-4ccd-80f4-6ec3053fd4a5",
        "bankId": "356c87b3-b14d-4524-a982-98aa96967674",
        "state": 1
    }

## Особенности запроса:
    
    Авторизация не требуется

---

# Отчёт по тест кейсу №41
## URL :

    http://94.139.255.171:5000/api/authorization/register

## Ожидаемый результат:

    Получен ответ с кодом 409 Conflict.


## Заголовки запроса:

    Content-Type: application/json
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: a9f2662a-5a6d-48a4-9dc8-6664695232ca
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive

## Тело запроса:

    {
        "name": "string",
        "birthday": "2023-01-06T12:54:39.545Z",
        "sex": 0,
        "email": "new123user@example.com",
        "password": "string",
        "roleId": "b6ac9a45-4032-4289-b439-2cc4d65c3f18"
    }

## Заголовки ответа:

    Content-Type: text/plain; charset=utf-8
    Date: Tue, 10 Jan 2023 11:29:03 GMT
    Server: Kestrel
    Transfer-Encoding: chunked

## Тело ответа:

    User with this email adress already exist

## Особенности запроса:
    
    Авторизация не требуется

---

# Отчёт по тест кейсу №42
## URL :

    http://94.139.255.171:5000/api/authorization/register

## Ожидаемый результат:

    Получен ответ с кодом 409 Conflict.


## Заголовки запроса:

    Content-Type: application/json
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: 335cf285-7452-4e09-81d1-1fd84338dd95
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive

## Тело запроса:

    {
        "name": "string",
        "birthday": "2023-01-06T12:54:39.545Z",
        "sex": 0,
        "email": "new123user@example.com",
        "password": "string",
        "roleId": "b6ac9a45-4032-4289-b439-2cc4d65c3f18",
        "bankId": "356c87b3-b14d-4524-a982-98aa96967674"
    }

## Заголовки ответа:

    Content-Type: text/plain; charset=utf-8
    Date: Tue, 10 Jan 2023 11:33:24 GMT
    Server: Kestrel
    Transfer-Encoding: chunked

## Тело ответа:

    User with this email adress already exist

## Особенности запроса:
    
    Авторизация не требуется

---

# Отчёт по тест кейсу №43
## URL :

    http://94.139.255.171:5000/api/authorization/register

## Ожидаемый результат:

    Получен ответ с кодом 400 Bad Request.


## Заголовки запроса:

    Content-Type: application/json
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: f4bf236a-7216-420e-b32b-9d91a0dbae3f
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive

## Тело запроса:

    {}

## Заголовки ответа:

    Content-Type: application/problem+json; charset=utf-8
    Date: Tue, 10 Jan 2023 13:04:29 GMT
    Server: Kestrel
    Transfer-Encoding: chunked

## Тело ответа:

    {
        "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
        "title": "One or more validation errors occurred.",
        "status": 400,
        "traceId": "00-7a296732afcf7a446500b991c7f7f839-34a69272d714fd43-00",
        "errors": {
            "Email": [
                "Invalid Email Address"
            ]
        }
    }

## Особенности запроса:
    
    Авторизация не требуется.

---

# Отчёт по тест кейсу №44
## URL :

    http://94.139.255.171:5000/api/authorization/register

## Ожидаемый результат:

    Получен ответ с кодом 400 Bad Request.


## Заголовки запроса:

    Content-Type: application/json
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: 28c7e787-02a5-4b56-8ecf-6d1a483d8bd3
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive

## Тело запроса:

    {
        "email": "user@mail.ru",
        "roleId": "b6ac9a45-4032-4289-b439-2cc4d65c3f18",
        "bankId": "356c87b3-b14d-4524-a982-98aa96967674"
    }

## Заголовки ответа:

    Content-Type: application/json; charset=utf-8
    Date: Tue, 10 Jan 2023 13:08:59 GMT
    Server: Kestrel
    Location: /api/users/eaba8dc6-1b36-4e31-8510-05d9e47e1c71
    Transfer-Encoding: chunked

## Тело ответа:

    {"userId":"eaba8dc6-1b36-4e31-8510-05d9e47e1c71","name":"","birthaday":"0001-01-01T00:00:00","sex":0,"email":"user@mail.ru","roleId":"b6ac9a45-4032-4289-b439-2cc4d65c3f18","bankId":"356c87b3-b14d-4524-a982-98aa96967674","state":0}

## Особенности запроса:
    
    Авторизация не требуется.

---

# Отчёт по тест кейсу №45
## URL :

    http://94.139.255.171:5000/api/authorization/register

## Ожидаемый результат:

    Получен ответ с кодом 400 Bad Request.


## Заголовки запроса:

    Content-Type: application/json
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: 656106ca-5e24-4ff0-bfa8-078dc5531259
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive

## Тело запроса:

    {
        "name": "string",
        "birthday": "2023-01-06T13:38:02.801Z",
        "sex": 0,
        "email": "user.com",
        "password": "string",
        "roleId": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
        "bankId": "3fa85f64-5717-4562-b3fc-2c963f66afa6"
    }

## Заголовки ответа:

    Content-Type: application/problem+json; charset=utf-8
    Date: Tue, 10 Jan 2023 14:06:33 GMT
    Server: Kestrel
    Transfer-Encoding: chunked

## Тело ответа:

    {
        "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
        "title": "One or more validation errors occurred.",
        "status": 400,
        "traceId": "00-da8d4357d75c8af7fbeb4a8f328769ab-f5fa2e1233e5a9c4-00",
        "errors": {
            "Email": [
                "Invalid Email Address"
            ]
        }
    }

## Особенности запроса:
    
    Авторизация не требуется.

---

# Отчёт по тест кейсу №46
## URL :

    http://94.139.255.171:5000/api/authorization/register

## Ожидаемый результат:

    Получен ответ с кодом 200 OK.


## Заголовки запроса:

    Content-Type: application/json
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: d7ebf18b-7767-46f8-9158-34fa1e8c9518
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive

## Тело запроса:

    {
        "email": "pobisa1270@subdito.com",
        "password": "qweasd123"
    }

## Заголовки ответа:

    Content-Type: text/plain; charset=utf-8
    Date: Tue, 10 Jan 2023 14:10:45 GMT
    Server: Kestrel
    Set-Cookie: refreshToken=nBMwHORa9AJCJbSscsNM0KmTDV3scvxUS2auu9Px3%2Fk94Jo2eLGi3k77kGv3fqyNrWp%2BpQIg3%2BxYyWs2v9iwBg%3D%3D; expires=Fri, 13 Jan 2023 14:10:45 GMT; path=/; httponly
    Transfer-Encoding: chunked

## Тело ответа:

    eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTUxMiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiJkODRiNzc5OC1kMjRiLTRkZDYtODQyZS1hOTA3YmIyYjgyYWQiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoiVXNlciIsImh0dHA6Ly9zY2hlbWFzLnhtbHNvYXAub3JnL3dzLzIwMDUvMDUvaWRlbnRpdHkvY2xhaW1zL2VtYWlsYWRkcmVzcyI6InBvYmlzYTEyNzBAc3ViZGl0by5jb20iLCJodHRwOi8vc2NoZW1hcy5taWNyb3NvZnQuY29tL3dzLzIwMDgvMDYvaWRlbnRpdHkvY2xhaW1zL3JvbGUiOiJDbGllbnQiLCJleHAiOjE2NzMzNjE2ODV9.MwxUWzRQOTQkeJfj14I_3xP2yPWJkMtmVY3F0uQUIZ2mW3yP6_-UTS5ut5k48RpSp1VoPwjikn7rkhwDmKDNZg

## Особенности запроса:
    
    -

---

# Отчёт по тест кейсу №47
## URL :

    http://94.139.255.171:5000/api/authorization/register

## Ожидаемый результат:

    Получен ответ с кодом 404 Not found.


## Заголовки запроса:

    Content-Type: application/json
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: 96e62f2a-e9b6-45e6-86fa-9bdf4f004b55
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=nBMwHORa9AJCJbSscsNM0KmTDV3scvxUS2auu9Px3%2Fk94Jo2eLGi3k77kGv3fqyNrWp%2BpQIg3%2BxYyWs2v9iwBg%3D%3D

## Тело запроса:

    {
        "email": "nonameuser@subdito.com",
        "password": "qweasd123"
    }

## Заголовки ответа:

    Content-Type: text/plain; charset=utf-8
    Date: Tue, 10 Jan 2023 14:13:20 GMT
    Server: Kestrel
    Transfer-Encoding: chunked

## Тело ответа:

    User not found.

## Особенности запроса:
    
    -

---

# Отчёт по тест кейсу №48
## URL :

    http://94.139.255.171:5000/api/authorization/register

## Ожидаемый результат:

    Получен ответ с кодом 400 Bad Request.


## Заголовки запроса:

    Content-Type: application/json
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: 96e62f2a-e9b6-45e6-86fa-9bdf4f004b55
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=nBMwHORa9AJCJbSscsNM0KmTDV3scvxUS2auu9Px3%2Fk94Jo2eLGi3k77kGv3fqyNrWp%2BpQIg3%2BxYyWs2v9iwBg%3D%3D

## Тело запроса:

    {
        "email": "pobisa1270@subdito.com"
    }

## Заголовки ответа:

    Content-Type: text/plain; charset=utf-8
    Date: Tue, 10 Jan 2023 14:17:35 GMT
    Server: Kestrel
    Transfer-Encoding: chunked

## Тело ответа:

    Email/Password combination if wrong

## Особенности запроса:
    
    -

---

# Отчёт по тест кейсу №49
## URL :

    http://94.139.255.171:5000/api/authorization/register

## Ожидаемый результат:

    Получен ответ с кодом 400 Bad Request.


## Заголовки запроса:

    Content-Type: application/json
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: 23a6dcd0-0647-4fe7-93ec-a44c959c6557
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=nBMwHORa9AJCJbSscsNM0KmTDV3scvxUS2auu9Px3%2Fk94Jo2eLGi3k77kGv3fqyNrWp%2BpQIg3%2BxYyWs2v9iwBg%3D%3D

## Тело запроса:

    {
        "password": "qweasd123"
    }

## Заголовки ответа:

    Content-Type: application/problem+json; charset=utf-8
    Date: Tue, 10 Jan 2023 14:26:26 GMT
    Server: Kestrel
    Transfer-Encoding: chunked

## Тело ответа:

    {"type":"https://tools.ietf.org/html/rfc7231#section-6.5.1","title":"One or more validation errors occurred.","status":400,"traceId":"00-a08e79ba0cc7220a6d699095f1c44aed-c112990ed7f05527-00","errors":{"Email":["Invalid Email Address"]}}

## Особенности запроса:
    
    -

---

# Отчёт по тест кейсу №50
## URL :

    http://94.139.255.171:5000/api/authorization/register

## Ожидаемый результат:

    Получен ответ с кодом 400 Bad Request.


## Заголовки запроса:

    Content-Type: application/json
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: baf70174-233f-4165-8612-b7fadd0d53fc
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=nBMwHORa9AJCJbSscsNM0KmTDV3scvxUS2auu9Px3%2Fk94Jo2eLGi3k77kGv3fqyNrWp%2BpQIg3%2BxYyWs2v9iwBg%3D%3D

## Тело запроса:

    {
        "email": "pobisa1270@",
        "password": "qweasd123"
    }

## Заголовки ответа:

    Content-Type: application/problem+json; charset=utf-8
    Date: Tue, 10 Jan 2023 14:30:21 GMT
    Server: Kestrel
    Transfer-Encoding: chunked

## Тело ответа:

    {"type":"https://tools.ietf.org/html/rfc7231#section-6.5.1","title":"One or more validation errors occurred.","status":400,"traceId":"00-4a42df51a6c2ad9931a4438c43d5827a-dd850612f0338484-00","errors":{"Email":["Invalid Email Address"]}}

## Особенности запроса:
    
    -

---

# Отчёт по тест кейсу №51
## URL :

    http://94.139.255.171:5000/api/authorization/refresh-token

## Ожидаемый результат:

    Получен ответ с кодом 200 OK. + новый токен в теле ответа.


## Заголовки запроса:

    Authorization: Bearer eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTUxMiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiJkODRiNzc5OC1kMjRiLTRkZDYtODQyZS1hOTA3YmIyYjgyYWQiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoiVXNlciIsImh0dHA6Ly9zY2hlbWFzLnhtbHNvYXAub3JnL3dzLzIwMDUvMDUvaWRlbnRpdHkvY2xhaW1zL2VtYWlsYWRkcmVzcyI6InBvYmlzYTEyNzBAc3ViZGl0by5jb20iLCJodHRwOi8vc2NoZW1hcy5taWNyb3NvZnQuY29tL3dzLzIwMDgvMDYvaWRlbnRpdHkvY2xhaW1zL3JvbGUiOiJDbGllbnQiLCJleHAiOjE2NzMzNjU4Mjl9.FUMFqIbil1RIRMyDvEykUliLWF7nbhvjnbF7ZUqc78Yu5B1Kt6ofaEXTVEkkLQD6_o_wCeVA4n8ZEdoNTmtEFA
    Content-Type: application/json
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: 89a3e2a3-cfcd-4230-9be2-7a1890c13c45
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=9Dc7m3l5OBcm8qKV%2FwIBWrP1lkLL%2BtE%2F2qYyZ%2BIbBej7DvJ5hIed1YsLeyOXpRLeVWkFo71Rb9JyYEAR9%2BtCOg%3D%3D

## Тело запроса:

    "eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTUxMiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiJkODRiNzc5OC1kMjRiLTRkZDYtODQyZS1hOTA3YmIyYjgyYWQiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoiVXNlciIsImh0dHA6Ly9zY2hlbWFzLnhtbHNvYXAub3JnL3dzLzIwMDUvMDUvaWRlbnRpdHkvY2xhaW1zL2VtYWlsYWRkcmVzcyI6InBvYmlzYTEyNzBAc3ViZGl0by5jb20iLCJodHRwOi8vc2NoZW1hcy5taWNyb3NvZnQuY29tL3dzLzIwMDgvMDYvaWRlbnRpdHkvY2xhaW1zL3JvbGUiOiJDbGllbnQiLCJleHAiOjE2NzMzNjU4Mjl9.FUMFqIbil1RIRMyDvEykUliLWF7nbhvjnbF7ZUqc78Yu5B1Kt6ofaEXTVEkkLQD6_o_wCeVA4n8ZEdoNTmtEFA"

## Заголовки ответа:

    Content-Type: text/plain; charset=utf-8
    Date: Tue, 10 Jan 2023 15:20:01 GMT
    Server: Kestrel
    Set-Cookie: refreshToken=ss%2FSbCbk2%2BQaxerBdU2KLLtZ2EYERPTgOmx%2F87ed4ICNlAScsN0EwaZgDxgLnT3flF2xeMkc5TebiD6Tt07sbg%3D%3D; expires=Fri, 13 Jan 2023 15:20:01 GMT; path=/; httponly
    Transfer-Encoding: chunked

## Тело ответа:

    eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTUxMiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiJkODRiNzc5OC1kMjRiLTRkZDYtODQyZS1hOTA3YmIyYjgyYWQiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoiVXNlciIsImh0dHA6Ly9zY2hlbWFzLnhtbHNvYXAub3JnL3dzLzIwMDUvMDUvaWRlbnRpdHkvY2xhaW1zL2VtYWlsYWRkcmVzcyI6InBvYmlzYTEyNzBAc3ViZGl0by5jb20iLCJodHRwOi8vc2NoZW1hcy5taWNyb3NvZnQuY29tL3dzLzIwMDgvMDYvaWRlbnRpdHkvY2xhaW1zL3JvbGUiOiJDbGllbnQiLCJleHAiOjE2NzMzNjU4NDF9.hQjxSXcbZkx2-GUMFEf1HLVntCBtWD2OA7a2Roq4d8fZDYRMLUUU6Tk8cO6pKwTu37L7PB0wCtOA7DeD0M1QFw

## Особенности запроса:
    
    В Authorization подставить bearer token полученный при авторизации.

---

# Отчёт по тест кейсу №52
## URL :

    http://94.139.255.171:5000/api/authorization/refresh-token

## Ожидаемый результат:

    Получен ответ с кодом 200 OK. + новый токен в теле ответа.


## Заголовки запроса:

    Authorization: Bearer eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTUxMiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiJkODRiNzc5OC1kMjRiLTRkZDYtODQyZS1hOTA3YmIyYjgyYWQiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoiVXNlciIsImh0dHA6Ly9zY2hlbWFzLnhtbHNvYXAub3JnL3dzLzIwMDUvMDUvaWRlbnRpdHkvY2xhaW1zL2VtYWlsYWRkcmVzcyI6InBvYmlzYTEyNzBAc3ViZGl0by5jb20iLCJodHRwOi8vc2NoZW1hcy5taWNyb3NvZnQuY29tL3dzLzIwMDgvMDYvaWRlbnRpdHkvY2xhaW1zL3JvbGUiOiJDbGllbnQiLCJleHAiOjE2NzMzNjU4Mjl9.FUMFqIbil1RIRMyDvEykUliLWF7nbhvjnbF7ZUqc78Yu5B1Kt6ofaEXTVEkkLQD6_o_wCeVA4n8ZEdoNTmtEFA
    Content-Type: application/json
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: 89a3e2a3-cfcd-4230-9be2-7a1890c13c45
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=9Dc7m3l5OBcm8qKV%2FwIBWrP1lkLL%2BtE%2F2qYyZ%2BIbBej7DvJ5hIed1YsLeyOXpRLeVWkFo71Rb9JyYEAR9%2BtCOg%3D%3D

## Тело запроса:

    "eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTUxMiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiJkODRiNzc5OC1kMjRiLTRkZDYtODQyZS1hOTA3YmIyYjgyYWQiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoiVXNlciIsImh0dHA6Ly9zY2hlbWFzLnhtbHNvYXAub3JnL3dzLzIwMDUvMDUvaWRlbnRpdHkvY2xhaW1zL2VtYWlsYWRkcmVzcyI6InBvYmlzYTEyNzBAc3ViZGl0by5jb20iLCJodHRwOi8vc2NoZW1hcy5taWNyb3NvZnQuY29tL3dzLzIwMDgvMDYvaWRlbnRpdHkvY2xhaW1zL3JvbGUiOiJDbGllbnQiLCJleHAiOjE2NzMzNjU4Mjl9.FUMFqIbil1RIRMyDvEykUliLWF7nbhvjnbF7ZUqc78Yu5B1Kt6ofaEXTVEkkLQD6_o_wCeVA4n8ZEdoNTmtEFA"

## Заголовки ответа:

    Content-Type: text/plain; charset=utf-8
    Date: Tue, 10 Jan 2023 15:20:01 GMT
    Server: Kestrel
    Set-Cookie: refreshToken=ss%2FSbCbk2%2BQaxerBdU2KLLtZ2EYERPTgOmx%2F87ed4ICNlAScsN0EwaZgDxgLnT3flF2xeMkc5TebiD6Tt07sbg%3D%3D; expires=Fri, 13 Jan 2023 15:20:01 GMT; path=/; httponly
    Transfer-Encoding: chunked

## Тело ответа:

    eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTUxMiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiJkODRiNzc5OC1kMjRiLTRkZDYtODQyZS1hOTA3YmIyYjgyYWQiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoiVXNlciIsImh0dHA6Ly9zY2hlbWFzLnhtbHNvYXAub3JnL3dzLzIwMDUvMDUvaWRlbnRpdHkvY2xhaW1zL2VtYWlsYWRkcmVzcyI6InBvYmlzYTEyNzBAc3ViZGl0by5jb20iLCJodHRwOi8vc2NoZW1hcy5taWNyb3NvZnQuY29tL3dzLzIwMDgvMDYvaWRlbnRpdHkvY2xhaW1zL3JvbGUiOiJDbGllbnQiLCJleHAiOjE2NzMzNjU4NDF9.hQjxSXcbZkx2-GUMFEf1HLVntCBtWD2OA7a2Roq4d8fZDYRMLUUU6Tk8cO6pKwTu37L7PB0wCtOA7DeD0M1QFw

## Особенности запроса:

    -

---

# Отчёт по тест кейсу №53
## URL :
    http

## Ожидаемый результат:

    Получен


## Заголовки запроса:

    Authorization: 

## Тело запроса:

    "eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZ

## Заголовки ответа:

    Content-Type: text/plain; charset=utf-8

## Тело ответа:

    eyJhbGciOiJodHRwOi8vd3

## Особенности запроса:

    -

---