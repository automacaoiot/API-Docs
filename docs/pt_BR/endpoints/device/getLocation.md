# Get Device Location

`GET api/device/{PUBLIC_KEY}/geolocation`    

## Descrição

Obtém informações da GeoLocalização do Dispositivo.

## Parâmetros

**PUBLIC_KEY** (String) - Chave Pública do Dispositivo.

## Autenticação
**Obrigatória**

## Método
`GET`

## EndPoint
`api/device/{PUBLIC_KEY}/geolocation`

## Exemplo

## Requisição

```
GET api/device/5D4161963252F0EABB435339/geolocation  HTTP/1.1  
Authorization: Bearer 2A192A93FA7E383AE98803C7  
Host: https://automacao-iot.com.br/api
```

## Resposta

```
HTTP/1.1 200 OK

Content-Length: 85
Content-Type: application/json;charset=utf8

{
    "success": true,
    "payload": {
        "latitude": "37.7510",
        "longitude": "-97.8220"
    },
    "message": ""
}
```
