# Create Device Log

`POST api/device/{PUBLIC_KEY}/log`

## Descrição

Criação de Log do Dispositivo.

## Parâmetros da URL

**PUBLIC_KEY** (String) - Chave Pública do Dispositivo.

## Parâmetros do Body

**code** (Integer) - Código do Error.
**message** (String) - Mensagem de Error.

## Autenticação
**Obrigatória**

## Método
`POST`
## EndPoint
`api/device/{PUBLIC_KEY}/log`

## Exemplo

## Requisição

```
POST api/device/5D4161963252F0EABB435339/log  HTTP/1.1
Authorization: Bearer 2A192A93FA7E383AE98803C7
Host: https://automacao-iot.com.br/api

Body:
{
"code":<codeNumber>,
"message:<messageString>
}

```

## Resposta

```
HTTP/1.1 200 OK

Content-Language: en
Content-Length: 2655
Content-Type: application/json

{
  "success": true,
  "payload": null,
  "message": "Device Log Created"
}
```
