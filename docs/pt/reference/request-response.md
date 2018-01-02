# Requisição e Resposta

Todas as chamadas da API devem ser feitas para `/api/endPoint` e irão retornar uma resposta no formato de **JSON**.

Clique [aqui](/index.html#EndPoints) para visualizar os EndPoints da API.

## Exemplo

`$ curl -i https://automacao-iot.com.br/api/`

```
HTTP/1.0 200 OK
Date Mon, 27 Mar 2017 01:39:36 GMT
Content-Type: application/json
Content-Language: en
Allow: GET

{
	"success": true,
	"payload": {
		"version": "1.0.0"
	},
	"message": "This is the ultimate API!"
}
```
## Métodos HTTP

Tentamos seguir as convenções de HTTP ao máximo, mas as vezes podemos estar sacrificando a formalidade por funcionalidades.  

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;border-color:#999;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:#999;color:#444;background-color:#F7FDFA;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:#999;color:#fff;background-color:#26ADE4;}
.tg .tg-baqh{text-align:center;vertical-align:top}
</style>
<table class="tg" style="undefined;table-layout: fixed; width: 718px">
<colgroup>
<col style="width: 124px">
<col style="width: 594px">
</colgroup>
  <tr>
    <th class="tg-baqh">Método</th>
    <th class="tg-baqh">Descrição</th>
  </tr>
  <tr>
    <td class="tg-baqh">GET</td>
    <td class="tg-baqh">Usado para consulta de dados.</td>
  </tr>
  <tr>
    <td class="tg-baqh">POST</td>
    <td class="tg-baqh">Usado para criação de dados</td>
  </tr>
  <tr>
    <td class="tg-baqh">PUT</td>
    <td class="tg-baqh">Usado para atualização de dados</td>
  </tr>
  <tr>
    <td class="tg-baqh">DELETE</td>
    <td class="tg-baqh">Usado para deletar dados</td>
  </tr>
</table>
<br>

## Códigos HTTP

O código de operação da requisição HTTP indica a situação da operação em questão.

Você pode conferir esses códigos [aqui](error-exception.html#codigos-http).

## Resposta

Para todas as requisições a API irá retornar uma resposta no formato de um **JSON**. Essas respostas seguem um modelo padronizado que explicaremos abaixo.

Veja [aqui](response-models.html) os **Response Models** que a API pode retornar.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;border-color:#999;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:#999;color:#444;background-color:#F7FDFA;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:#999;color:#fff;background-color:#26ADE4;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-amwm{font-weight:bold;text-align:center;vertical-align:top}
.tg .tg-9ewa{color:#fe0000;text-align:center;vertical-align:top}
.tg .tg-i218{color:#009901;text-align:center;vertical-align:top}
</style>
<table class="tg" style="undefined;table-layout: fixed; width: 716px">
<colgroup>
<col style="width: 124px">
<col style="width: 174px">
<col style="width: 103px">
<col style="width: 315px">
</colgroup>
  <tr>
    <th class="tg-baqh">Chave</th>
    <th class="tg-baqh">Tipo</th>
    <th class="tg-baqh">Anulável</th>
    <th class="tg-baqh">Significado</th>
  </tr>
  <tr>
    <td class="tg-baqh">success</td>
    <td class="tg-amwm">boolean</td>
    <td class="tg-9ewa">Não</td>
    <td class="tg-baqh">Operação da Requisição foi feita com Sucesso.</td>
  </tr>
  <tr>
    <td class="tg-baqh">payload</td>
    <td class="tg-amwm">Nested Json Object<br>ou<br>Nested Json Array</td>
    <td class="tg-i218"><br>Sim</td>
    <td class="tg-baqh">Resultado da Operação que podem vir na forma de um JSON Object ou um JSON Array.</td>
  </tr>
  <tr>
    <td class="tg-baqh">message</td>
    <td class="tg-amwm">string</td>
    <td class="tg-9ewa">Não</td>
    <td class="tg-baqh">Mensagem Informacional.</td>
  </tr>
</table>
<br>
