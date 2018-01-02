# Get User

`GET api/user/{USERNAME}`    

## Descrição

Obtém informações sobre um determinado Usuário. Este EndPoint retorna dados informacionais do Usuário, tal como id, Email, nome e etc.

## Parâmetros

**USERNAME** (String) - Username.

## Autenticação

**Obrigatória**

## Método

`GET`

## EndPoint

`api/user/{USERNAME}`

## Exemplo

## Requisição

```
GET api/user/testinho  HTTP/1.1  
Authorization: Bearer 290C2EFB2BC98580E674FAJ9  
Host: https://automacao-iot.com.br/api
```

## Resposta

```
HTTP/1.1 200 OK

Content-Language: en
Content-Length: 556
Content-Type: application/json;charset=utf8

{
    "success": true,
    "payload": {
        "id_user": 9,
        "id_user_pricing_plan": 9,
        "email": "test@test.com.br",
        "username": "testinho",
        "name": "Teste Testinho",
        "cpf": "",
        "country": null,
        "state": null,
        "city": null,
        "district": null,
        "street": null,
        "number": null,
        "latitude": null,
        "longitude": null,
        "zipcode": null,
        "timezone": "",
        "activation_code": "290C2EFB2BC98580E674FAJ9",
        "api_requests_usage": 17,
        "api_network_usage": 8794,
        "api_network_income_usage": 8685,
        "api_network_outgoing_usage": 109,
        "created_at": "2017-11-13 18:00:35",
        "updated_at": "2017-11-13 18:00:35",
        "active": 1,
        "admin": 0
    },
    "message": ""
}
```
