<h1>Getting Started</h1>

## Guia Básico

A API possui uma variedade de EndPoints para serem utilizados, porém este guia visa apresentar um **quickstart** para que você consiga de maneira rápida e prática conectar a sua aplicação ao nosso sistema.

`Atenção:`

> Se você utiliza um **ESP8266**, confira nossa [SDK]() que transparece e facilita todas as operações citadas aqui!

`Observação:`

> **A aplicação em questão pode estar rodando em um sistema embarcado ( ESP8266, Arduino, Orange PI, Linux ...) ou em qualquer plataforma que você esteja trabalhando, porém nosso foco maior aqui será para sistemas embarcados.**

Basicamente você apenas irá precisar de dois **EndPoints** em sua aplicação: [getResourceLastFeeds](../endpoints/resource/getResourceLastFeeds.html) e [createResourceFeeds](../endpoints/resource/createResourceFeeds.html)

O uso destes EndPoints vai depender dos recursos que sua Aplicação está utilizando, bem como se os recursos são do tipo **Entrada** ou do tipo **Saida**.

Para entender melhor o que é um recurso de **entrada** ou **saida** clique [aqui]().

### Recurso de Entrada

Se o seu sistema apenas possuir recursos de **entrada**, você irá utilizar apenas [getResourceLastFeeds](../endpoints/resource/getResourceLastFeeds.html).

**Basicamente, um recurso de entrada é aquele que apenas recebe informações do sistema e não envia nada.**

`Exemplo`



### Recurso de Saida

Se o seu sistema apenas possuir recursos de **saida**, você irá utilizar apenas [createResourceFeeds](../endpoints/resource/createResourceFeeds.html).

**Basicamente, um recurso de saida é aquele que apenas envia informações para sistema e não recebe nada.**

`Exemplo`



### Múltiplos Recursos

Para evitar um **overhead** de chamadas em sua plataforma embarcada, há variações para chamadas na API para o acesso de múltiplos recursos e para o envio de múltiplos dados de diversos recursos, sendo as principais apresentadas abaixo:

[getResourcesLastFeeds](../endpoints/resources/getResourcesFeeds.html)

[getSelectedResourcesLastFeeds](../endpoints/resources/getResourcesLastFeeds.html)

[createResourcesFeeds](../endpoints/resources/createResourcesFeeds.html).

**Os exemplos para Recurso de Entrada e Recurso de Saida são válidos aqui, a única diferença é que este é para múltiplos recursos em um Dispositivo.**

`Apesar dos exemplos serem individuais, um dispositivo pode conter vários tipos de recursos ao mesmo tempo.`

### Tudo Pronto e Conectado!

Os EndPoints e explicações apresentadas acima são o necessário para começar a conectar sua aplicação ao nosso sistema. Os EndPoints apresentados aqui são apenas os principais, possuimos uma variedade de EndPoints com diversas funcionalidades.

Confira a página de [Autenticação](../reference/authentication.html) para entender como funciona nosso sistema de **Presença de Dispositivos**.
