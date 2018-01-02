# Get Device

`GET api/device/{PUBLIC_KEY}`    

## Descrição

Obtém informações sobre um determinado Dispositivo. Este EndPoint retorna dados informacionais do Dispositivo, tal como id, dono, nome e descrição do dispositivo.

## Parâmetros

**PUBLIC_KEY** (String) - Chave Pública do Dispositivo.

## Autenticação
**Não Obrigatória**

**Nota:** Atualização de presença apenas com o Header de Autenticação.

## Método
`GET`

## EndPoint
`api/device/{PUBLIC_KEY}`

## Exemplo

## Requisição

```
GET api/device/5D4161963252F0EABB435339  HTTP/1.1  
Authorization: Bearer 2A192A93FA7E383AE98803C7  
Host: https://automacao-iot.com.br/api
```

## Resposta

```
HTTP/1.1 200 OK

Content-Language: en
Content-Length: 2142
Content-Type: application/json

{
    "success": true,
    "payload": {
        "id_device": 71,
        "id_user": 9,
        "id_last_syscall": null,
        "name": "Test Device",
        "icon_name": "bullhorn",
        "description": "This is a Test Device",
        "ip": null,
        "timezone": "America/Fortaleza",
        "latitude": "37.7510",
        "longitude": "-97.8220",
        "public_key": "5D4161963252F0EABB435339",
        "api_requests_usage": 0,
        "api_network_usage": 0,
        "api_network_income_usage": 0,
        "api_network_outgoing_usage": 0,
        "lifetime": 15,
        "lifetime_updated_at": null,
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
                "id_last_feed": null,
                "name": "Input Binary Resource",
                "description": "This is a Resource wich type is Input and SubType Binary.",
                "lifetime": 15,
                "api_requests_usage": 0,
                "api_network_usage": 0,
                "api_network_income_usage": 0,
                "api_network_outgoing_usage": 0,
                "lifetime_updated_at": null,
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
                "last_feed": null,
                "data_format": []
            },
            {
                "id_resource": 74,
                "id_device": 71,
                "id_resource_subtype": 6,
                "id_last_feed": null,
                "name": "Input Digital Resource",
                "description": "This is a Resource wich type is Input and SubType Digital.",
                "lifetime": 15,
                "api_requests_usage": 0,
                "api_network_usage": 0,
                "api_network_income_usage": 0,
                "api_network_outgoing_usage": 0,
                "lifetime_updated_at": null,
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
                "last_feed": null,
                "data_format": []
            }
        ]
    },
    "message": ""
}
```
