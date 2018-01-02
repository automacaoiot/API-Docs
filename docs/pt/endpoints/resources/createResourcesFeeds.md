# Create Resources Feeds

`POST /api/device/{PUBLIC_KEY}/resources/feeds`    

## Descrição

Insere um novo Registro de Feeds em múltiplos recursos do Dispositivo.

## Parâmetros da URL

**PUBLIC_KEY** (String) - Chave Pública do Dispositivo.

## Parâmetros de Query

**silent** (Boolean) - Define se a operação deve ser feita em modo silencioso ou não.   
Caso seja verdadeiro o recurso não irá atualizar presença. **Ex:** silent = true | false.

**Valor Padrão**: **FALSE**

## Parâmetros do Body

* Tipo: **Json Array**

**id_resource** (Integer) - Id do Resource.  
**input** (Mixed) - Valor de Entrada.  

## Autenticação

**Obrigatória**

## Método

`POST`

## EndPoint

`/api/device/{PUBLIC_KEY}/resources/feeds`

## Exemplo

## Requisição

```
POST api/device/5D4161963252F0EABB435339/resources/feeds  HTTP/1.1  
Authorization: Bearer 2A192A93FA7E383AE98803C7  
Host: https://automacao-iot.com.br/api

Body:
[
	{
		"id_resource": 73,
		"input": 1
	},
	{
		"id_resource": 74,
		"input": 65
	}
]
```

## Resposta

```
HTTP/1.1 200 OK

Content-Language: en
Content-Length: 228
Content-Type: application/json

{
    "success": true,
    "payload": [
        {
            "raw_data": 1,
            "id_resource": 73,
            "created_at": "2018-01-02 17:46:57",
            "id_resource_feed": 510649
        },
        {
            "raw_data": 65,
            "id_resource": 74,
            "created_at": "2018-01-02 17:46:57",
            "id_resource_feed": 510650
        }
    ],
    "message": ""
}
```
