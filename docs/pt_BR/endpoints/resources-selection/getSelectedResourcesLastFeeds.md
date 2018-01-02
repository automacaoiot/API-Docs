# Get Selected Resources Last Feeds

`GET /api/device/{PUBLIC_KEY}/resources/{ID_RESOURCES}/feeds/last`

## Descrição

Retorna o Último Feeds de todos os Recursos Escolhidos de um Dispositivo.

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

`/api/device/{PUBLIC_KEY}/resources/{ID_RESOURCES}/feeds/last`

## Exemplo

## Requisição

```
GET api/device/5D4161963252F0EABB435339/resources/73,74/feeds/last  HTTP/1.1
Opcional: Authorization Bearer 2A192A93FA7E383AE98803C7
Host: https://automacao-iot.com.br/api
```

## Resposta

```
HTTP/1.1 200 OK

Content-Language: en
Content-Length: 232
Content-Type: application/json

{
    "success": true,
    "payload": [
        {
            "id_resource_feed": 510649,
            "id_resource": 73,
            "raw_data": "1",
            "created_at": "2018-01-02 17:46:57"
        },
        {
            "id_resource_feed": 510650,
            "id_resource": 74,
            "raw_data": "65",
            "created_at": "2018-01-02 17:46:57"
        }
    ],
    "message": ""
}
```
