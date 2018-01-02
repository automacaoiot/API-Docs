# Erros e Exceções

Pode ser que ao decorrer do uso da API você se depare com algum erro ou exceção no corpo da resposta, como por exemplo, tentar acessar um recurso não existente.

A API está preparada para lidar com esses tipos de situações e aqui nesta seção descreveremos o comportamento de erro para estas situações.

Primeiramente, qualquer operação que não possua o código HTTP de 2.x.x ( Ex: 200 ) é considerado uma situação de exceção.

O único código de erro especial é o 500 ( Erro Interno ), mas não se preocupe caso isso aconteça, nosso sistema de Log nos avisará rapídamente para que possamos analisar a situação!

## Códigos HTTP

Aqui listaremos os possíveis códigos HTTP em que a API utiliza em sua resposta e sua semântica nela.
