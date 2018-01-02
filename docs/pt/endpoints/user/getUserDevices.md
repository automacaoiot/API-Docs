# Get User Devices

`GET api/user/{USERNAME}/devices`    

## Descrição

Obtém os dispositivos e seus respectivos recursos do Usuário. As informações do dispositivo são similares ao Endpoint do dispositivo individual.

## Parâmetros da URL

**USERNAME** (String) - Username.

## Autenticação

**Obrigatória**

## Método

`GET`
## EndPoint

`api/user/{USERNAME}/devices`

## Exemplo

## Requisição

```
GET api/user/testinho/devices  HTTP/1.1  
Authorization: Bearer 290C2EFB2BC98580E674FAJ9  
Host: https://automacao-iot.com.br/api
```

## Resposta

```
HTTP/1.1 200 OK

Content-Language: en
Content-Length: 2446
Content-Type: application/json

{
    "success": true,
    "payload": [
        {
            "id_device": 71,
            "id_user": 9,
            "id_last_syscall": null,
            "name": "Test Device",
            "icon_name": "bullhorn",
            "description": "This is a Test Device",
            "ip": "177.195.62.187",
            "timezone": "America/Fortaleza",
            "latitude": "-22.98",
            "longitude": "-43.088",
            "secret_key": "2A192A93FA7E383AE98803C7",
            "public_key": "5D4161963252F0EABB435339",
            "api_requests_usage": 17,
            "api_network_usage": 8794,
            "api_network_income_usage": 8685,
            "api_network_outgoing_usage": 109,
            "lifetime": 15,
            "lifetime_updated_at": "2018-01-02 18:01:02",
            "created_at": "2018-01-02 16:16:14",
            "updated_at": "2018-01-02 16:16:14",
            "active": 1,
            "is_alive": false,
            "is_dead": true,
            "resources": [
                {
                    "id_resource": 73,
                    "id_device": 71,
                    "id_resource_subtype": 3,
                    "id_last_feed": 510649,
                    "name": "Input Binary Resource",
                    "description": "This is a Resource wich type is Input and SubType Binary.",
                    "lifetime": 15,
                    "api_requests_usage": 5,
                    "api_network_usage": 1511,
                    "api_network_income_usage": 1496,
                    "api_network_outgoing_usage": 15,
                    "lifetime_updated_at": "2018-01-02 18:01:02",
                    "created_at": "2018-01-02 16:16:42",
                    "updated_at": "2018-01-02 16:17:54",
                    "active": 1,
                    "is_alive": false,
                    "is_dead": true,
                    "subtype": {
                        "id_resource_subtype": 3,
                        "id_resource_type": 1,
                        "name": "Binário",
                        "name_i18n": "Binary",
                        "description": null,
                        "data_format_operation": 0,
                        "data_restriction_regex": null,
                        "data_restriction_begin_range": 0,
                        "data_restriction_end_range": 1,
                        "created_at": "2017-05-10 00:00:00",
                        "updated_at": "2017-05-10 00:00:00"
                    },
                    "last_feed": {
                        "id_resource_feed": 510649,
                        "id_resource": 73,
                        "raw_data": "1",
                        "created_at": "2018-01-02 17:46:57"
                    },
                    "data_format": []
                },
                {
                    "id_resource": 74,
                    "id_device": 71,
                    "id_resource_subtype": 6,
                    "id_last_feed": 510650,
                    "name": "Input Digital Resource",
                    "description": "This is a Resource wich type is Input and SubType Digital.",
                    "lifetime": 15,
                    "api_requests_usage": 0,
                    "api_network_usage": 0,
                    "api_network_income_usage": 0,
                    "api_network_outgoing_usage": 0,
                    "lifetime_updated_at": "2018-01-02 18:01:02",
                    "created_at": "2018-01-02 16:17:35",
                    "updated_at": "2018-01-02 16:17:35",
                    "active": 1,
                    "is_alive": false,
                    "is_dead": true,
                    "subtype": {
                        "id_resource_subtype": 6,
                        "id_resource_type": 1,
                        "name": "Digital",
                        "name_i18n": "Digital",
                        "description": null,
                        "data_format_operation": 1,
                        "data_restriction_regex": null,
                        "data_restriction_begin_range": 0,
                        "data_restriction_end_range": 100,
                        "created_at": "2017-08-25 16:11:57",
                        "updated_at": "2017-08-30 22:20:22"
                    },
                    "last_feed": {
                        "id_resource_feed": 510650,
                        "id_resource": 74,
                        "raw_data": "65",
                        "created_at": "2018-01-02 17:46:57"
                    },
                    "data_format": []
                }
            ]
        }
    ],
    "message": ""
}
```
