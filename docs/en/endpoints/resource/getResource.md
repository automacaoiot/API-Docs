# Get Resource

`GET /api/device/{PUBLIC_KEY}/resource/{ID_RESOURCE}`

## Descrição

Retorna todas as informações de um recurso do dispositivo.

## Parâmetros da URL

**PUBLIC_KEY** (String) - Chave Pública do Dispositivo.

**ID_RESOURCE** (Integer) - Id do Recurso do dispositivo.

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

`/api/device/{PUBLIC_KEY}/resource/{ID_RESOURCE}`

## Exemplo

## Requisição

```
GET api/device/5D4161963252F0EABB435339/resource/73?silent=false  HTTP/1.1
Opcional Authorization: Bearer 2A192A93FA7E383AE98803C7
Host: https://automacao-iot.com.br/api
```

## Resposta

```
HTTP/1.1 200 OK

Content-Language: en
Content-Length: 938
Content-Type: application/json

{
    "success": true,
    "payload": {
        "id_resource": 73,
        "id_device": 71,
        "id_resource_subtype": 3,
        "id_last_feed": 510648,
        "name": "Input Binary Resource",
        "description": "This is a Resource wich type is Input and SubType Binary.",
        "lifetime": 15,
        "api_requests_usage": 1,
        "api_network_usage": 169,
        "api_network_income_usage": 154,
        "api_network_outgoing_usage": 15,
        "lifetime_updated_at": "2018-01-02 17:31:03",
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
            "id_resource_feed": 510648,
            "id_resource": 73,
            "raw_data": "1",
            "created_at": "2018-01-02 17:31:03"
        },
        "data_format": []
    },
    "message": ""
}
```
