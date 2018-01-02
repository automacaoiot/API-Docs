# Get Resource Feeds

`GET/api/device/{PUBLIC_KEY}/resource/{ID_RESOURCE}/feeds`    

## Descrição

Recupera todos os Registros de Feeds do Recurso.

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

`/api/device/{PUBLIC_KEY}/resource/{ID_RESOURCE}/feeds`

## Exemplo

## Requisição

```
GET api/device/5D4161963252F0EABB435339/resource/73/feeds  HTTP/1.1  
Opcional: Authorization: Bearer 2A192A93FA7E383AE98803C7
Host: https://automacao-iot.com.br/api
```

## Resposta

```
HTTP/1.1 200 OK

Content-Language: en
Content-Length: 136
Content-Type: application/json

{
    "success": true,
    "payload": [
        {
            "id_resource_feed": 510648,
            "id_resource": 73,
            "raw_data": "1",
            "created_at": "2018-01-02 17:31:03"
        }
    ],
    "message": ""
}
```
