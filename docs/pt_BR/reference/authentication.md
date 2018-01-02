# Autenticação

## Tokens de Autenticação

Tokens de autenticação são passados via Headers especiais de **Autenticação** para autenticar e validar a operação e garantir com que tudo seja feito em segurança na API!

Os Tokens também são responsáveis por fazer a atualização da Presença do Dispositivo, ou seja, permitir que o sistema saiba que seu dispositivo está conectado.

*  Todas as operações exceto as de **GET** são necessárias a inclusão do Header Especial da operação, caso contrário não irá ter acesso.
*  Para obter presença do dispositivo é necessário que o Header de Autenticação esteja presente em todas as operações. Caso contrário o dispositivo irá demonstrar-se desligado.

## Header de Autenticação

  <style type="text/css">
  .tg  {border-collapse:collapse;border-spacing:0;border-color:#999;}
  .tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:#999;color:#444;background-color:#F7FDFA;}
  .tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:#999;color:#fff;background-color:#26ADE4;}
  .tg .tg-baqh{text-align:center;vertical-align:top}
  .tg .tg-yw4l{vertical-align:top}
  </style>
  <table class="tg">
  <tr>
    <th class="tg-baqh">Header</th>
    <th class="tg-baqh">Valor</th>
    <th class="tg-baqh">Descrição</th>
  </tr>
  <tr>
    <td class="tg-yw4l">Authorization</td>
    <td class="tg-yw4l">Bearer {PRIVATE_KEY}</td>
    <td class="tg-yw4l">Usado para Autenticar a operação. ( Exemplo: Autenticar o dispositivo com a Chave Privada )</td>
  </tr>
  </table>
  <br>

## Exemplo de Chamada
`$ curl -H 'Authorization: Bearer {TOKEN}' https://automacao-iot.com.br/api/device/{public_key}/`

## Aonde eu encontro a Chave Privada ( Private Key ) ?

Ao criar um [dispositivo](https://automacao-iot.com.br/iot/web/device/device-cadastrar) em sua conta, no canto direito há uma opção chamada **Modificar Dispositivo**.

Na tela que irá abrir, vai ter um campo chamado **Secret Key** e é esta chave que você usará em seu **Token de Autenticação**.
