## Aggregate
- Conjunto de entidades que são trabalhadas ao mesmo tempo. (criadas, atualizadas)
### Exemplo
Vamos supor que temos uma aplicação de e-commerce. 
Dentro dela, temos a parte de pagamento que está ligada com a entidade do pedido em si. 
Dentro dessa entidade, temos outras, como a lista de itens e as informações de entrega.
Não faria sentido eu ter a lista de itens sem ter o pedido em si.

## WatchedList
- É uma lista observada.
- Faz mais sentido na edição
- Pattern que permite a gente ter mais informações sobre itens contidos em uma lista
- É um array que também possuem informações se é um item novo, editado, ou deletado
### Exemplo
Ainda sobre a aplicação e-commerce, se a gente tiver junto com um produto um anexo, e queremos editá-lo, por exemplo, remover um anexo, criar, ou substituir por outro. 
se a gente tiver uma WatchedList de anexos, poderemos fazer essas operações de forma mais performática.
