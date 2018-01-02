# Create Resource Feeds

`POST /api/device/{PUBLIC_KEY}/resource/{ID_RESOURCE}/feeds`    

## Descrição

Insere um novo Registro de Feeds no Recurso.

## Parâmetros da URL

**PUBLIC_KEY** (String) - Chave Pública do Dispositivo.

**ID_RESOURCE** (Integer) - Id do Recurso do dispositivo.

## Parâmetros de Query

**silent** (Boolean) - Define se a operação deve ser feita em modo silencioso ou não.   
Caso seja verdadeiro o recurso não irá atualizar presença. **Ex:** silent = true | false.

**Valor Padrão**: **FALSE**

## Parâmetros do Body

**input** (Mixed) - Valor de Entrada.  

## Autenticação

**Obrigatória**

## Método

`POST`

## EndPoint

`/api/device/{PUBLIC_KEY}/resource/{ID_RESOURCE}/feeds`

## Exemplo

## Requisição

```
POST api/device/5D4161963252F0EABB435339/resource/73/feeds  HTTP/1.1  
Authorization: Bearer 2A192A93FA7E383AE98803C7  
Host: https://automacao-iot.com.br/api

Body:
{
"input":1
}
```

## Resposta

```
HTTP/1.1 200 OK

Content-Language: en
Content-Length: 154
Content-Type: application/json

{
    "success": true,
    "payload": {
        "raw_data": 1,
        "id_resource": 73,
        "created_at": "2018-01-02 17:31:03",
        "id_resource_feed": 510648
    },
    "message": "Resource Feed Created!"
}
```
