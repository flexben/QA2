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
    http://94.139.255.171:5000/api/banks

## Ожидаемый результат:

    Получили ответ с кодом 201 и тело ответа, содержащее информацию о созданном банке. Параметры объекта: "bankId": "name": "description": "state": "rating": "shortName":


## Заголовки запроса:

    Authorization: Bearer eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTUxMiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI3Y2JiNWZiOS0zYmQzLTQ1MmYtOTc5NS02NmM3NDU4YmIzNTMiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoiQWRtaW4iLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9lbWFpbGFkZHJlc3MiOiJhZG1pbkBtYWlsLnJ1IiwiaHR0cDovL3NjaGVtYXMubWljcm9zb2Z0LmNvbS93cy8yMDA4LzA2L2lkZW50aXR5L2NsYWltcy9yb2xlIjoiQWRtaW4iLCJleHAiOjE2NzM0MzkwMTd9.XlvSTxKea7zVTmD9mikAY0NdYnkmBwMvOq7dJHSi5hYikpvAPTHBUWO2lE-eNO6TYF1LcwWEYyrZYXlWke5V3A
    Content-Type: application/json
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: 2c3377e6-2393-4cf2-82ba-8f4f41feea48
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=S33qGwM2PaaPgCQI3sBxSDVDqw8r5mlnKULAlYxif9dWX9KsObWpGML9%2FjjMRa6qI1t70beArCx97GQ8n%2BnW%2Bg%3D%3D

## Тело запроса:

    {
    "name": "TestBank",
    "description": "Bank for api tests",
    "shortName": "TBank"
    }

## Заголовки ответа:

    Content-Type: application/json; charset=utf-8
    Date: Wed, 11 Jan 2023 11:41:07 GMT
    Server: Kestrel
    Location: /api/banks/96240028-0382-4247-a71a-d69998ff9507
    Transfer-Encoding: chunked

## Тело ответа:

    {
        "bankId": "96240028-0382-4247-a71a-d69998ff9507",
        "name": "TestBank",
        "description": "Bank for api tests",
        "state": 2,
        "rating": 0,
        "shortName": "TBank"
    }

## Особенности запроса:

    Получить и использовать bearer token Администратора

---

# Отчёт по тест кейсу №54
## URL :
    http://94.139.255.171:5000/api/banks

## Ожидаемый результат:

    Получили 409 Conflict.


## Заголовки запроса:

    Authorization: Bearer eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTUxMiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI3Y2JiNWZiOS0zYmQzLTQ1MmYtOTc5NS02NmM3NDU4YmIzNTMiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoiQWRtaW4iLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9lbWFpbGFkZHJlc3MiOiJhZG1pbkBtYWlsLnJ1IiwiaHR0cDovL3NjaGVtYXMubWljcm9zb2Z0LmNvbS93cy8yMDA4LzA2L2lkZW50aXR5L2NsYWltcy9yb2xlIjoiQWRtaW4iLCJleHAiOjE2NzM0MzkwMTd9.XlvSTxKea7zVTmD9mikAY0NdYnkmBwMvOq7dJHSi5hYikpvAPTHBUWO2lE-eNO6TYF1LcwWEYyrZYXlWke5V3A
    Content-Type: application/json
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: d514e0a2-8014-47f5-ad97-38b8c400fc60
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=S33qGwM2PaaPgCQI3sBxSDVDqw8r5mlnKULAlYxif9dWX9KsObWpGML9%2FjjMRa6qI1t70beArCx97GQ8n%2BnW%2Bg%3D%3D

## Тело запроса:

    {
        "name": "apitest",
        "description": "apitest",
        "shortName": "apitest"
    }

## Заголовки ответа:

    Content-Type: application/json; charset=utf-8
    Date: Wed, 11 Jan 2023 12:02:56 GMT
    Server: Kestrel
    Location: /api/banks/23237caa-45bf-4e4f-ae2c-f64bf98e766d
    Transfer-Encoding: chunked

## Тело ответа:

    {
        "bankId": "96240028-0382-4247-a71a-d69998ff9507",
        "name": "TestBank",
        "description": "Bank for api tests",
        "state": 2,
        "rating": 0,
        "shortName": "TBank"
    }

## Особенности запроса:

    Получить и использовать bearer token Администратора

---

# Отчёт по тест кейсу №55
## URL :
    http://94.139.255.171:5000/api/banks

## Ожидаемый результат:

    Получили 409 Conflict.


## Заголовки запроса:

    Authorization: Bearer eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTUxMiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI3Y2JiNWZiOS0zYmQzLTQ1MmYtOTc5NS02NmM3NDU4YmIzNTMiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoiQWRtaW4iLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9lbWFpbGFkZHJlc3MiOiJhZG1pbkBtYWlsLnJ1IiwiaHR0cDovL3NjaGVtYXMubWljcm9zb2Z0LmNvbS93cy8yMDA4LzA2L2lkZW50aXR5L2NsYWltcy9yb2xlIjoiQWRtaW4iLCJleHAiOjE2NzM0MzkwMTd9.XlvSTxKea7zVTmD9mikAY0NdYnkmBwMvOq7dJHSi5hYikpvAPTHBUWO2lE-eNO6TYF1LcwWEYyrZYXlWke5V3A
    Content-Type: application/json
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: 443c37e8-a697-44b3-92d5-03e4cf46de6a
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=S33qGwM2PaaPgCQI3sBxSDVDqw8r5mlnKULAlYxif9dWX9KsObWpGML9%2FjjMRa6qI1t70beArCx97GQ8n%2BnW%2Bg%3D%3D

## Тело запроса:

    {
        "name": "",
        "description": "",
        "shortName": ""
    }

## Заголовки ответа:

    Content-Type: application/json; charset=utf-8
    Date: Wed, 11 Jan 2023 12:02:56 GMT
    Server: Kestrel
    Location: /api/banks/23237caa-45bf-4e4f-ae2c-f64bf98e766d
    Transfer-Encoding: chunked

## Тело ответа:

    {
        "bankId": "23237caa-45bf-4e4f-ae2c-f64bf98e766d",
        "name": "",
        "description": "",
        "state": 2,
        "rating": 0,
        "shortName": ""
    }

## Особенности запроса:

    Получить и использовать bearer token Администратора

---

# Отчёт по тест кейсу №56
## URL :
    http://94.139.255.171:5000/api/banks

## Ожидаемый результат:

    Получили 403 Forbidden.


## Заголовки запроса:

    Authorization: Bearer eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTUxMiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiJkODRiNzc5OC1kMjRiLTRkZDYtODQyZS1hOTA3YmIyYjgyYWQiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoiVXNlciIsImh0dHA6Ly9zY2hlbWFzLnhtbHNvYXAub3JnL3dzLzIwMDUvMDUvaWRlbnRpdHkvY2xhaW1zL2VtYWlsYWRkcmVzcyI6InBvYmlzYTEyNzBAc3ViZGl0by5jb20iLCJodHRwOi8vc2NoZW1hcy5taWNyb3NvZnQuY29tL3dzLzIwMDgvMDYvaWRlbnRpdHkvY2xhaW1zL3JvbGUiOiJDbGllbnQiLCJleHAiOjE2NzM0NDA5MTF9.FwabtGNkaUxxnw3Pyf__TUlxiGwftuMxW7UVMnjw_074ulJsUNuBb1fFCk2fOkihA5XdPv0tcF7hbEBss8GESA
    Content-Type: application/json
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: 7fc9c758-5923-4ec6-b60d-fd83a679ec73
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=6hXkp5UjGksfuYHFvO1MMZcfyPypuTWy%2Bx5ldnkmEmgG9qrhUt4eOsdH5YKy0vWZ3qtzpOgW9cXC06mtD%2F%2F7WQ%3D%3D

## Тело запроса:

    {
        "name": "Bank",
        "description": "Cool bank",
        "shortName": "B"
    }

## Заголовки ответа:

    Content-Length: 0
    Date: Wed, 11 Jan 2023 12:11:34 GMT
    Server: Kestrel

## Особенности запроса:

    Получить и использовать bearer token Обычного пользователя.

---

# Отчёт по тест кейсу №57
## URL :
    http://94.139.255.171:5000/api/banks

## Ожидаемый результат:

	Получили ответ с кодом 200 и телом ответа, содержащим список всех банков с параметрами "bankId": "name": "description": "state": "rating": "shortName":


## Заголовки запроса:

    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: f1c5ba27-1b98-41dc-96a0-12422af476e9
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=6hXkp5UjGksfuYHFvO1MMZcfyPypuTWy%2Bx5ldnkmEmgG9qrhUt4eOsdH5YKy0vWZ3qtzpOgW9cXC06mtD%2F%2F7WQ%3D%3D

## Тело запроса:

    {
    "name": "TestBank",
    "description": "Bank for api tests",
    "shortName": "TBank"
    }

## Заголовки ответа:

    Content-Type: application/json; charset=utf-8
    Date: Wed, 11 Jan 2023 12:14:59 GMT
    Server: Kestrel
    Transfer-Encoding: chunked

## Тело ответа (часть):

    [
        {
            "bankId": "23237caa-45bf-4e4f-ae2c-f64bf98e766d",
            "name": "",
            "description": "",
            "state": 2,
            "rating": 0,
            "shortName": ""
        },
        {
            "bankId": "50468565-602c-41e5-8562-fc124718bb5a",
            "name": "",
            "description": "",
            "state": 2,
            "rating": 0,
            "shortName": ""
        }
    ...

## Особенности запроса:

    -

---

# Отчёт по тест кейсу №58
## URL :
    http://94.139.255.171:5000/api/banks/e3c31276-ceaf-46fc-9259-7d7bcf0edbd9

## Ожидаемый результат:

    Получили ответ с кодом 200 и телом ответа, содержащим изменённые параметры банка "name": "description": "shortName":


## Заголовки запроса:

    Authorization: Bearer eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTUxMiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI3Y2JiNWZiOS0zYmQzLTQ1MmYtOTc5NS02NmM3NDU4YmIzNTMiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoiQWRtaW4iLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9lbWFpbGFkZHJlc3MiOiJhZG1pbkBtYWlsLnJ1IiwiaHR0cDovL3NjaGVtYXMubWljcm9zb2Z0LmNvbS93cy8yMDA4LzA2L2lkZW50aXR5L2NsYWltcy9yb2xlIjoiQWRtaW4iLCJleHAiOjE2NzM0NDE3NDV9._M-Eyy_cuTopv8cvqDB9CFcFfoWxmj2yB74aLnBJie713JtVJlKSJF55RtrJGZ-aAFpu8ZCdEFYakMFqb8knjw
    Content-Type: application/json
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: 31826f06-9f97-43a3-aec3-75857caa222d
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=rH0gRs4M5esAYjOzA5Qi92sf1gpH6vIdLN2dmDAk3gBTpm7%2ByhsBbmU0GUBY2ceYZNipAXtc8P654eRKe2M0hQ%3D%3D

## Тело запроса:

    {
        "name": "apitest123",
        "description": "apitest123",
        "shortName": "apitest123"
    }

## Заголовки ответа:

    Content-Type: application/json; charset=utf-8
    Date: Wed, 11 Jan 2023 12:25:51 GMT
    Server: Kestrel
    Transfer-Encoding: chunked

## Тело ответа:

    {
        "bankId": "e3c31276-ceaf-46fc-9259-7d7bcf0edbd9",
        "name": "apitest123",
        "description": "apitest123",
        "state": 2,
        "rating": 0,
        "shortName": "apitest123"
    }

## Особенности запроса:

    Получить и использовать bearer token Администратора

---

# Отчёт по тест кейсу №59
## URL :
    http://94.139.255.171:5000/api/banks/2dca687f-f14c-4ed8-8933-29674fa2a061

## Ожидаемый результат:

    Получили ответ с кодом 404 Not Found.


## Заголовки запроса:

    Authorization: Bearer eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTUxMiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI3Y2JiNWZiOS0zYmQzLTQ1MmYtOTc5NS02NmM3NDU4YmIzNTMiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoiQWRtaW4iLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9lbWFpbGFkZHJlc3MiOiJhZG1pbkBtYWlsLnJ1IiwiaHR0cDovL3NjaGVtYXMubWljcm9zb2Z0LmNvbS93cy8yMDA4LzA2L2lkZW50aXR5L2NsYWltcy9yb2xlIjoiQWRtaW4iLCJleHAiOjE2NzM0NDE3NDV9._M-Eyy_cuTopv8cvqDB9CFcFfoWxmj2yB74aLnBJie713JtVJlKSJF55RtrJGZ-aAFpu8ZCdEFYakMFqb8knjw
    Content-Type: application/json
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: 44a8b213-77f9-49db-b615-91a06978d076
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=rH0gRs4M5esAYjOzA5Qi92sf1gpH6vIdLN2dmDAk3gBTpm7%2ByhsBbmU0GUBY2ceYZNipAXtc8P654eRKe2M0hQ%3D%3D

## Тело запроса:

    {
        "name": "apitest123",
        "description": "apitest123",
        "shortName": "apitest123"
    }

## Заголовки ответа:

    Content-Type: text/plain; charset=utf-8
    Date: Wed, 11 Jan 2023 12:28:28 GMT
    Server: Kestrel
    Transfer-Encoding: chunked

## Тело ответа:

    Bank not found

## Особенности запроса:

    Получить и использовать bearer token Администратора

---

# Отчёт по тест кейсу №60
## URL :
    http://94.139.255.171:5000/api/banks/e3c31276-ceaf-46fc-9259-7d7bcf0edbd9

## Ожидаемый результат:

    Получили ответ с кодом 403 Forbidden.


## Заголовки запроса:

    Authorization: Bearer eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTUxMiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiJkODRiNzc5OC1kMjRiLTRkZDYtODQyZS1hOTA3YmIyYjgyYWQiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoiVXNlciIsImh0dHA6Ly9zY2hlbWFzLnhtbHNvYXAub3JnL3dzLzIwMDUvMDUvaWRlbnRpdHkvY2xhaW1zL2VtYWlsYWRkcmVzcyI6InBvYmlzYTEyNzBAc3ViZGl0by5jb20iLCJodHRwOi8vc2NoZW1hcy5taWNyb3NvZnQuY29tL3dzLzIwMDgvMDYvaWRlbnRpdHkvY2xhaW1zL3JvbGUiOiJDbGllbnQiLCJleHAiOjE2NzM0NDA5MTF9.FwabtGNkaUxxnw3Pyf__TUlxiGwftuMxW7UVMnjw_074ulJsUNuBb1fFCk2fOkihA5XdPv0tcF7hbEBss8GESA
    Content-Type: application/json
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: 1f6c565a-eb09-41f1-a142-0633f26da185
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=rH0gRs4M5esAYjOzA5Qi92sf1gpH6vIdLN2dmDAk3gBTpm7%2ByhsBbmU0GUBY2ceYZNipAXtc8P654eRKe2M0hQ%3D%3D

## Тело запроса:

    {
        "name": "apitest123",
        "description": "apitest123",
        "shortName": "apitest123"
    }

## Заголовки ответа:

    Content-Length: 0
    Date: Wed, 11 Jan 2023 12:33:29 GMT
    Server: Kestrel

## Особенности запроса:

    Получить и использовать bearer token Обычного пользователя

---

# Отчёт по тест кейсу №61
## URL :
    http://94.139.255.171:5000/api/banks/e3c31276-ceaf-46fc-9259-7d7bcf0edbd9

## Ожидаемый результат:

    Получили ответ с кодом 400 Bad Request.


## Заголовки запроса:

    Authorization: Bearer eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTUxMiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI3Y2JiNWZiOS0zYmQzLTQ1MmYtOTc5NS02NmM3NDU4YmIzNTMiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoiQWRtaW4iLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9lbWFpbGFkZHJlc3MiOiJhZG1pbkBtYWlsLnJ1IiwiaHR0cDovL3NjaGVtYXMubWljcm9zb2Z0LmNvbS93cy8yMDA4LzA2L2lkZW50aXR5L2NsYWltcy9yb2xlIjoiQWRtaW4iLCJleHAiOjE2NzM0NDE3NDV9._M-Eyy_cuTopv8cvqDB9CFcFfoWxmj2yB74aLnBJie713JtVJlKSJF55RtrJGZ-aAFpu8ZCdEFYakMFqb8knjw
    Content-Type: application/json
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: 4ec249ef-3902-458e-9107-8a7338254e4c
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=rH0gRs4M5esAYjOzA5Qi92sf1gpH6vIdLN2dmDAk3gBTpm7%2ByhsBbmU0GUBY2ceYZNipAXtc8P654eRKe2M0hQ%3D%3D

## Тело запроса:

    {
        "name": "",
        "description": "",
        "shortName": ""
    }

## Заголовки ответа:

    Content-Type: application/json; charset=utf-8
    Date: Wed, 11 Jan 2023 12:37:26 GMT
    Server: Kestrel
    Transfer-Encoding: chunked

## Тело ответа:

    {
        "bankId": "e3c31276-ceaf-46fc-9259-7d7bcf0edbd9",
        "name": "",
        "description": "",
        "state": 2,
        "rating": 0,
        "shortName": ""
    }

## Особенности запроса:

    Получить и использовать bearer token Администратора

---

# Отчёт по тест кейсу №62
## URL :
    http://94.139.255.171:5000/api/banks/e3c31276-ceaf-46fc-9259-7d7bcf0edbd9

## Ожидаемый результат:

    Получили ответ с кодом 204. Банк удален.

## Заголовки запроса:

    Authorization: Bearer eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTUxMiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI3Y2JiNWZiOS0zYmQzLTQ1MmYtOTc5NS02NmM3NDU4YmIzNTMiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoiQWRtaW4iLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9lbWFpbGFkZHJlc3MiOiJhZG1pbkBtYWlsLnJ1IiwiaHR0cDovL3NjaGVtYXMubWljcm9zb2Z0LmNvbS93cy8yMDA4LzA2L2lkZW50aXR5L2NsYWltcy9yb2xlIjoiQWRtaW4iLCJleHAiOjE2NzM0NDE3NDV9._M-Eyy_cuTopv8cvqDB9CFcFfoWxmj2yB74aLnBJie713JtVJlKSJF55RtrJGZ-aAFpu8ZCdEFYakMFqb8knjw
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: a10defed-4c1c-454f-a7c8-a130b936fe13
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=rH0gRs4M5esAYjOzA5Qi92sf1gpH6vIdLN2dmDAk3gBTpm7%2ByhsBbmU0GUBY2ceYZNipAXtc8P654eRKe2M0hQ%3D%3D

## Заголовки ответа:

    Date: Wed, 11 Jan 2023 12:45:03 GMT
    Server: Kestrel

## Особенности запроса:

    Получить и использовать bearer token Администратора

---

# Отчёт по тест кейсу №63
## URL :
    http://94.139.255.171:5000/api/banks/e3c31276-ceaf-46fc-9259-7d7bcf0edbd9

## Ожидаемый результат:

    Получили ответ с кодом 403 Forbidden.


## Заголовки запроса:

    Authorization: Bearer eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTUxMiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiJkODRiNzc5OC1kMjRiLTRkZDYtODQyZS1hOTA3YmIyYjgyYWQiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoiVXNlciIsImh0dHA6Ly9zY2hlbWFzLnhtbHNvYXAub3JnL3dzLzIwMDUvMDUvaWRlbnRpdHkvY2xhaW1zL2VtYWlsYWRkcmVzcyI6InBvYmlzYTEyNzBAc3ViZGl0by5jb20iLCJodHRwOi8vc2NoZW1hcy5taWNyb3NvZnQuY29tL3dzLzIwMDgvMDYvaWRlbnRpdHkvY2xhaW1zL3JvbGUiOiJDbGllbnQiLCJleHAiOjE2NzM0NDMxMDF9.MPSP8epMZ7z_htXT7mq8tluShi3TTmYPsejowThbfhRh32sYPahFIt-zCI8PVxIM44BQPE67gEdkKbNihnjM2A
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: bc960223-61dc-4e60-81ff-54ba6c05fd28
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=mah3X%2FRktB9CkMLTz2C5BCdGN6NBnpjcdKxTOqE1utY4iQQ%2Fha3UfbrQsscBykQAKVU5pDOMANCd%2BAOH5WCV9w%3D%3D

## Заголовки ответа:

    Content-Length: 0
    Date: Wed, 11 Jan 2023 12:47:59 GMT
    Server: Kestrel

## Особенности запроса:

    Получить и использовать bearer token Обычного пользователя

---

# Отчёт по тест кейсу №64
## URL :
    http://94.139.255.171:5000/api/banks/2dca687f-f14c-4ed8-8933-29674fa2a061

## Ожидаемый результат:

    Получили ответ с кодом 200 и тело ответа, содержащее параметры банка "bankId":, "name":, "description":, "state":, "rating":, "shortName":.


## Заголовки запроса:

    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: d707d623-0d11-4f26-8af5-0e2ce50ebb2e
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=mah3X%2FRktB9CkMLTz2C5BCdGN6NBnpjcdKxTOqE1utY4iQQ%2Fha3UfbrQsscBykQAKVU5pDOMANCd%2BAOH5WCV9w%3D%3D

## Заголовки ответа:

    Content-Type: application/json; charset=utf-8
    Date: Wed, 11 Jan 2023 12:53:57 GMT
    Server: Kestrel
    Transfer-Encoding: chunked

## Тело ответа:

    {
        "bankId": "e3c31276-ceaf-46fc-9259-7d7bcf0edbd9",
        "name": "",
        "description": "",
        "state": 2,
        "rating": 0,
        "shortName": ""
    }

## Особенности запроса:

    -

---

# Отчёт по тест кейсу №65
## URL :
    http://94.139.255.171:5000/api/banks/e3c21271-ceaf-43fc-9244-7d7bcf0edbd1

## Ожидаемый результат:

    Получили ответ с кодом 404 Not Found


## Заголовки запроса:

    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: 19e71eb1-fd0e-4ce5-806c-460d945d5261
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=mah3X%2FRktB9CkMLTz2C5BCdGN6NBnpjcdKxTOqE1utY4iQQ%2Fha3UfbrQsscBykQAKVU5pDOMANCd%2BAOH5WCV9w%3D%3D

## Заголовки ответа:

    Content-Type: application/problem+json; charset=utf-8
    Date: Wed, 11 Jan 2023 12:59:11 GMT
    Server: Kestrel
    Transfer-Encoding: chunked

## Тело ответа:

    {
        "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
        "title": "Not Found",
        "status": 404,
        "traceId": "00-5509d687f5235f81e7d24d0b63a1cc2a-a712778d696b01b9-00"
    }

## Особенности запроса:

    -

---

# Отчёт по тест кейсу №66
## URL :
    http://94.139.255.171:5000/api/banks/Name?name=A-Bank

## Ожидаемый результат:

    Получили ответ с кодом 200 и телом, содержащим найденные банки.


## Заголовки запроса:

    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: 4160ce93-a435-4de6-86e4-6a9c27b1046f
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=mah3X%2FRktB9CkMLTz2C5BCdGN6NBnpjcdKxTOqE1utY4iQQ%2Fha3UfbrQsscBykQAKVU5pDOMANCd%2BAOH5WCV9w%3D%3D

## Заголовки ответа:

    Content-Type: application/json; charset=utf-8
    Date: Wed, 11 Jan 2023 13:09:43 GMT
    Server: Kestrel
    Transfer-Encoding: chunked

## Тело ответа:

    [
        {
            "bankId": "fbe52e4b-6d8d-4cf5-8194-d98e730634f3",
            "name": "A-Bank",
            "description": "Описание банка",
            "state": 2,
            "rating": 0,
            "shortName": "A"
        }
    ]

## Особенности запроса:

    -

---

# Отчёт по тест кейсу №67
## URL :
    http://94.139.255.171:5000/api/banks/Name?name=A-Ba

## Ожидаемый результат:

    Получили ответ с кодом 200 и телом, содержащим найденные банки.


## Заголовки запроса:

    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: 09a54b6e-6db9-4d5d-aae8-b7dbf7bda372
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=mah3X%2FRktB9CkMLTz2C5BCdGN6NBnpjcdKxTOqE1utY4iQQ%2Fha3UfbrQsscBykQAKVU5pDOMANCd%2BAOH5WCV9w%3D%3D

## Заголовки ответа:

    Content-Type: application/json; charset=utf-8
    Date: Wed, 11 Jan 2023 13:12:41 GMT
    Server: Kestrel
    Transfer-Encoding: chunked

## Тело ответа:

    [
        {
            "bankId": "fbe52e4b-6d8d-4cf5-8194-d98e730634f3",
            "name": "A-Bank",
            "description": "Описание банка",
            "state": 2,
            "rating": 0,
            "shortName": "A"
        }
    ]

## Особенности запроса:

    -

---

# Отчёт по тест кейсу №68
## URL :
    http://94.139.255.171:5000/api/banks/Name?name=Aboba1488Bank

## Ожидаемый результат:

    Получили ответ с кодом 404 Not Found.


## Заголовки запроса:

    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: d557d7ba-9f46-45c1-b759-eb8e695686db
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=mah3X%2FRktB9CkMLTz2C5BCdGN6NBnpjcdKxTOqE1utY4iQQ%2Fha3UfbrQsscBykQAKVU5pDOMANCd%2BAOH5WCV9w%3D%3D

## Заголовки ответа:

    Content-Type: application/json; charset=utf-8
    Date: Wed, 11 Jan 2023 13:15:14 GMT
    Server: Kestrel
    Transfer-Encoding: chunked

## Особенности запроса:

    -

---

# Отчёт по тест кейсу №69
## URL :
    http://94.139.255.171:5000/api/banks/e3c31276-ceaf-46fc-9259-7d7bcf0edbd9/feedbacks

## Ожидаемый результат:

    Получили ответ с кодом 200 и тело ответа, содержащее отзывы о банке с параметрами "feedbackId":,"rating":, "text":, "date":, "state":, "isLatest":, "pruductId":, "userId":


## Заголовки запроса:

    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: 392f7623-719d-463a-9e37-3c7ba9b23021
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=mah3X%2FRktB9CkMLTz2C5BCdGN6NBnpjcdKxTOqE1utY4iQQ%2Fha3UfbrQsscBykQAKVU5pDOMANCd%2BAOH5WCV9w%3D%3D

## Заголовки ответа:

    Content-Type: application/json; charset=utf-8
    Date: Wed, 11 Jan 2023 13:18:04 GMT
    Server: Kestrel
    Transfer-Encoding: chunked

## Тело ответа (часть):

    [
        {
            "feedbackId": "9483a5c1-e6c6-4771-b77d-2eddb2078fb8",
            "rating": 5,
            "text": "Лучший",
            "date": "2022-12-19T19:43:20.958089Z",
            "state": 2,
            "isLatest": true,
            "pruductId": "0abcbbd3-4f65-443d-98fd-b62d31eabe69",
            "userId": "7cbb5fb9-3bd3-452f-9795-66c7458bb353"
        },
        {
            "feedbackId": "f2932072-a597-48f1-b2da-759c5ba7e7bf",
            "rating": 5,
            "text": "ок",
            "date": "2022-12-20T16:20:23.025243Z",
            "state": 2,
            "isLatest": true,
            "pruductId": "d4afca6a-eac8-4498-841c-2c206b3c1e3b",
            "userId": "7cbb5fb9-3bd3-452f-9795-66c7458bb353"
        },
    ...

## Особенности запроса:

    -

---

# Отчёт по тест кейсу №70
## URL :
    http://94.139.255.171:5000/api/banks/6bcf96a7-5947-4698-9f00-ba777b0ac6c1/employee

## Ожидаемый результат:

    Получили ответ с кодом 200 и телом, содержащим информацию о сотрудниках банка. "userId":, "name":, "birthaday":, "sex":, "email":, "roleId":, "bankId":, "state":


## Заголовки запроса:

    Authorization: Bearer eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTUxMiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI3Y2JiNWZiOS0zYmQzLTQ1MmYtOTc5NS02NmM3NDU4YmIzNTMiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoiQWRtaW4iLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9lbWFpbGFkZHJlc3MiOiJhZG1pbkBtYWlsLnJ1IiwiaHR0cDovL3NjaGVtYXMubWljcm9zb2Z0LmNvbS93cy8yMDA4LzA2L2lkZW50aXR5L2NsYWltcy9yb2xlIjoiQWRtaW4iLCJleHAiOjE2NzM0NDUzNjB9.KNo88_NqC8Zo8PzqcSxroYFYqGLfdzkRiStb2jkeTjVCSO9yGJK0QQyxeVSGoXFyO4LUfTIVItOkJ11Gf8eOrg
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: ddd2a325-00ba-4723-86e1-24ac153de2ca
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=MWeebBG1cWwaZJ4eXWuZq%2BzzuMRi2ZMEiZy%2FtxE%2FyWQ99WCH%2FqJqqiI6LZvqnbiE82ExSLJYQ43q4ZqHZss5Xw%3D%3D

## Заголовки ответа:

    Content-Type: application/json; charset=utf-8
    Date: Wed, 11 Jan 2023 13:25:42 GMT
    Server: Kestrel
    Transfer-Encoding: chunked

## Тело ответа (часть):

    [
        {
            "userId": "779ac7fa-b1a5-4c64-bfab-22ce51258a67",
            "name": "string",
            "birthaday": "2022-12-02T13:29:28.643Z",
            "sex": 0,
            "email": "user@example.com",
            "roleId": "b6ac9a45-4032-4289-b439-2cc4d65c3f18",
            "bankId": "6bcf96a7-5947-4698-9f00-ba777b0ac6c1",
            "state": 0
        }
    ]

## Особенности запроса:

    Получить и использовать bearer token Администратора

---

# Отчёт по тест кейсу №71
## URL :
    http://94.139.255.171:5000/api/banks/6bcf96a7-5947-4698-9f00-ba777b0ac6c2/employee

## Ожидаемый результат:

    Получили ответ с кодом 404 Not Found.


## Заголовки запроса:

    Authorization: Bearer eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTUxMiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI3Y2JiNWZiOS0zYmQzLTQ1MmYtOTc5NS02NmM3NDU4YmIzNTMiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoiQWRtaW4iLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9lbWFpbGFkZHJlc3MiOiJhZG1pbkBtYWlsLnJ1IiwiaHR0cDovL3NjaGVtYXMubWljcm9zb2Z0LmNvbS93cy8yMDA4LzA2L2lkZW50aXR5L2NsYWltcy9yb2xlIjoiQWRtaW4iLCJleHAiOjE2NzM0NDUzNjB9.KNo88_NqC8Zo8PzqcSxroYFYqGLfdzkRiStb2jkeTjVCSO9yGJK0QQyxeVSGoXFyO4LUfTIVItOkJ11Gf8eOrg
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: cab388ba-8674-4ad6-99a9-c96537c8fb5c
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=MWeebBG1cWwaZJ4eXWuZq%2BzzuMRi2ZMEiZy%2FtxE%2FyWQ99WCH%2FqJqqiI6LZvqnbiE82ExSLJYQ43q4ZqHZss5Xw%3D%3D

## Заголовки ответа:

    Content-Type: text/plain; charset=utf-8
    Date: Wed, 11 Jan 2023 13:30:10 GMT
    Server: Kestrel
    Transfer-Encoding: chunked

## Тело ответа (часть):

    Bank with id = 6bcf96a7-5947-4698-9f00-ba777b0ac6c2 not found

## Особенности запроса:

    Получить и использовать bearer token Администратора

---

# Отчёт по тест кейсу №72
## URL :
    http://94.139.255.171:5000/api/banks/6bcf96a7-5947-4698-9f00-ba777b0ac6c1/employee

## Ожидаемый результат:

    Получили ответ с кодом 401 Error: Unauthorized.


## Заголовки запроса:

    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: d91a9ada-7e75-4595-9831-0495c5a8cc3b
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=MWeebBG1cWwaZJ4eXWuZq%2BzzuMRi2ZMEiZy%2FtxE%2FyWQ99WCH%2FqJqqiI6LZvqnbiE82ExSLJYQ43q4ZqHZss5Xw%3D%3D

## Заголовки ответа:

    Content-Length: 0
    Date: Wed, 11 Jan 2023 13:31:59 GMT
    Server: Kestrel
    WWW-Authenticate: Bearer

## Особенности запроса:

    -

---

# Отчёт по тест кейсу №73
## URL :
    http://94.139.255.171:5000/api/banks/6bcf96a7-5947-4698-9f00-ba777b0ac6c1/employee

## Ожидаемый результат:

    Получили ответ с кодом 403 Forbidden.


## Заголовки запроса:

    Authorization: Bearer eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTUxMiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiJkODRiNzc5OC1kMjRiLTRkZDYtODQyZS1hOTA3YmIyYjgyYWQiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoiVXNlciIsImh0dHA6Ly9zY2hlbWFzLnhtbHNvYXAub3JnL3dzLzIwMDUvMDUvaWRlbnRpdHkvY2xhaW1zL2VtYWlsYWRkcmVzcyI6InBvYmlzYTEyNzBAc3ViZGl0by5jb20iLCJodHRwOi8vc2NoZW1hcy5taWNyb3NvZnQuY29tL3dzLzIwMDgvMDYvaWRlbnRpdHkvY2xhaW1zL3JvbGUiOiJDbGllbnQiLCJleHAiOjE2NzM0NDU4NTd9.QAM-9lERLPWFLg1sHAHyLuZ9dupOxHklhMTaVUICDZDtCanUWKOE5PS2xxA7fWsFeVV6WwMHzNKkPIIj5ZH3YQ
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: cfc539e1-5ef9-4cf2-a3c0-296681667ed9
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=nQfOQgeaGlPEpm2zZGYCyULoWFFEw3LejRoJaYt%2FRoJvJLfybwrr%2Fap5zvNdkg3XnXppKasy6SqEu7ih88cKlQ%3D%3D

## Заголовки ответа:

    Content-Length: 0
    Date: Wed, 11 Jan 2023 13:33:50 GMT
    Server: Kestrel

## Особенности запроса:

    Использовать bearer token Обычного пользователя.

---

# Отчёт по тест кейсу №74
## URL :
    http://94.139.255.171:5000/api/banks/6bcf96a7-5947-4698-9f00-ba777b0ac6c1/employee

## Ожидаемый результат:

    Получили ответ с кодом 403 Forbidden.


## Заголовки запроса:

    Authorization: Bearer eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTUxMiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiIwZGM2YTE2ZC04ODQzLTQ3YjgtODEyMS05ZTBkMTgyODM5MzAiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoidGVzdF93b3JrZXIyIiwiaHR0cDovL3NjaGVtYXMueG1sc29hcC5vcmcvd3MvMjAwNS8wNS9pZGVudGl0eS9jbGFpbXMvZW1haWxhZGRyZXNzIjoidGVzdF93b3JrZXIyQHRlc3QucnUiLCJodHRwOi8vc2NoZW1hcy5taWNyb3NvZnQuY29tL3dzLzIwMDgvMDYvaWRlbnRpdHkvY2xhaW1zL3JvbGUiOiJFbXBsb3llZSIsImV4cCI6MTY3MzQ0NjAxN30.qVkEJkAhaJS8OHrDBSsvUCHy4OAlDjSIxH_qCdjgYdacFK-T1i-9h7POyTnnjOSj-rlR9US5Xirv84XCSF1Aeg
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: da49f1e9-1cfd-40d2-a26d-11c5bb91d438
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=lA0CXoCQ7lSV8tZu3rh8inPIsp%2F8RSRogUy3a25YhG6m6l0rgUGU6zty5bD%2BQtDtriEiskOvDxp3aIESPnRe0Q%3D%3D

## Заголовки ответа:

    Content-Type: application/json; charset=utf-8
    Date: Wed, 11 Jan 2023 13:36:40 GMT
    Server: Kestrel
    Transfer-Encoding: chunked

## Тело ответа:

    [
        {
            "userId": "779ac7fa-b1a5-4c64-bfab-22ce51258a67",
            "name": "string",
            "birthaday": "2022-12-02T13:29:28.643Z",
            "sex": 0,
            "email": "user@example.com",
            "roleId": "b6ac9a45-4032-4289-b439-2cc4d65c3f18",
            "bankId": "6bcf96a7-5947-4698-9f00-ba777b0ac6c1",
            "state": 0
        }
    ]

## Особенности запроса:

    Использовать bearer token Сотрудника другого банка.

---

# Отчёт по тест кейсу №75
## URL :
    http://94.139.255.171:5000/api/banks/6bcf96a7-5947-4698-9f00-ba777b0ac6c1/employee

## Ожидаемый результат:

    Получили ответ с кодом 200 и телом, сожержащим список сотрудников банка с параметрами: "userId":, "name":, "birthaday":, "sex":, "email":, "roleId":, "bankId":, "state":


## Заголовки запроса:

    Authorization: Bearer eyJhbGciOiJodHRwOi8vd3d3LnczLm9yZy8yMDAxLzA0L3htbGRzaWctbW9yZSNobWFjLXNoYTUxMiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiJjNmU1ZTkzYy0zNThhLTQ5NjktOThiZC01MWQ4MzA1Njg3ZDYiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoidXNlcnRlc3QxMjMiLCJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9lbWFpbGFkZHJlc3MiOiIxMjN0ZXN0QG1haWwucnUiLCJodHRwOi8vc2NoZW1hcy5taWNyb3NvZnQuY29tL3dzLzIwMDgvMDYvaWRlbnRpdHkvY2xhaW1zL3JvbGUiOiJFbXBsb3llZSIsImV4cCI6MTY3MzQ1MTc1N30.z6Z0pxCbVARuFQ5gS1DcWIi54c62t8fpYtNQS3I3FwRhCdfkohG7ii34VbWe8RFlOH3w06Rk-3NwaIgLcjuS_A
    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: 10cd3f57-b631-4676-b891-f3460dacbddd
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=UWRU80GVxQh1F6PZMc06eQDzoNW4LDtXgz2%2Fk0sRBATMEgV9tXr5dxnBGzD%2FMYuyOAGaNV07kwg%2FaW6ZfeAN6A%3D%3D


## Заголовки ответа:

    Content-Type: application/json; charset=utf-8
    Date: Wed, 11 Jan 2023 15:12:07 GMT
    Server: Kestrel
    Transfer-Encoding: chunked

## Тело ответа (часть):

    [
        {
            "userId": "72dcfad0-d2cd-45ff-8798-52ae3fddb310",
            "name": "",
            "birthaday": "0001-01-01T00:00:00",
            "sex": 0,
            "email": "user12@mail.ru",
            "roleId": "b6ac9a45-4032-4289-b439-2cc4d65c3f18",
            "bankId": "356c87b3-b14d-4524-a982-98aa96967674",
            "state": 0
        },
    ...

## Особенности запроса:

    Использовать bearer token Сотрудника другого банка.

---

# Отчёт по тест кейсу №76
## URL :
    http://94.139.255.171:5000/api/banks/6bcf96a7-5947-4698-9f00-ba777b0ac6c1/products

## Ожидаемый результат:

    Получен ответ 200 с телом, содержащим список продуктов банка с параметрами: "productId":, "name":, "description":, "state":, "avgRating":, "bankId":, "categoryId":


## Заголовки запроса:

    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: c5d5388d-66f7-42ce-a73d-e92863a3c3f0
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=UWRU80GVxQh1F6PZMc06eQDzoNW4LDtXgz2%2Fk0sRBATMEgV9tXr5dxnBGzD%2FMYuyOAGaNV07kwg%2FaW6ZfeAN6A%3D%3D

## Заголовки ответа:

    Content-Type: application/json; charset=utf-8
    Date: Wed, 11 Jan 2023 15:15:16 GMT
    Server: Kestrel
    Transfer-Encoding: chunked

## Тело ответа (часть):

    [
        {
            "productId": "64c73f15-db30-4627-afff-73acae31deb9",
            "name": "авп",
            "description": "",
            "state": 2,
            "avgRating": 5,
            "bankId": "6bcf96a7-5947-4698-9f00-ba777b0ac6c1",
            "categoryId": "bd342d90-ec77-48df-aab4-be518e351253"
        },
    ...

## Особенности запроса:

    -

---

# Отчёт по тест кейсу №77
## URL :
    http://94.139.255.171:5000/api/banks/6bcf96a7-5947-4698-9f00-ba777b0ac6c1/products

## Ожидаемый результат:

    Получен ответ 404 Not Found.

## Заголовки запроса:

    User-Agent: PostmanRuntime/7.30.0
    Accept: */*
    Cache-Control: no-cache
    Postman-Token: 1fc2ef8e-1946-4fa7-bd7e-d6a789d7c8d4
    Host: 94.139.255.171:5000
    Accept-Encoding: gzip, deflate, br
    Connection: keep-alive
    Cookie: refreshToken=UWRU80GVxQh1F6PZMc06eQDzoNW4LDtXgz2%2Fk0sRBATMEgV9tXr5dxnBGzD%2FMYuyOAGaNV07kwg%2FaW6ZfeAN6A%3D%3D


## Заголовки ответа:

    Content-Length: 0
    Date: Wed, 11 Jan 2023 15:22:09 GMT
    Server: Kestrel
    WWW-Authenticate: Bearer

## Тело ответа:

    Bank with id = 6bcf96a7-5947-4698-9f00-ba777b0ac6c2 not found

## Особенности запроса:

    -

---