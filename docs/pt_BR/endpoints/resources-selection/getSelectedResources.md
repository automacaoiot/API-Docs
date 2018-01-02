# Get Selected Resources

`GET /api/device/{PUBLIC_KEY}/resources/{ID_RESOURCES}`

## Descrição

Retorna todos os Recursos Escolhidos de um Dispositivo.

## Parâmetros da URL

**PUBLIC_KEY** (String) - Chave Pública do Dispositivo.

**ID_RESOURCES** (Int Array) - Lista de Id's dos Recursos. ( **Ex:** 1,50,150,30 )

## Parâmetros de Query

**silent** (Boolean) - Define se a operação deve ser feita em modo silencioso ou não.
Caso seja verdadeiro o recurso não irá atualizar presença. **Ex:** silent = true | false.

**Valor Padrão**: **FALSE**

## Autenticação

**Não Obrigatória**

**Nota:** Atualização de presença apenas com o Header de Autenticação.

## Método

`GET`

## EndPoint

`/api/device/{PUBLIC_KEY}/resources/{ID_RESOURCES}`

## Exemplo

## Requisição

```
GET api/device/5D4161963252F0EABB435339/resources/19,29  HTTP/1.1
Opcional: Authorization Bearer 2A192A93FA7E383AE98803C7
Host: https://automacao-iot.com.br/api
```

## Resposta

```
HTTP/1.1 200 OK

Content-Language: en
Content-Length: 1834
Content-Type: application/json

{
    "success": true,
    "payload": [
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
            "lifetime_updated_at": "2018-01-02 17:54:30",
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
            "lifetime_updated_at": "2018-01-02 17:54:30",
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
    ],
    "message": ""
}
```
