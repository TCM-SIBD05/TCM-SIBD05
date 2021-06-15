# C1 : Introdução


## Descrição do trabalho
No âmbito da cadeira de Sistemas de Informação e Bases de dados, foi proposto à turma criar uma base de dados para uma empresa fictícia criada por nós. Posto isto, decidimos criar a base de dados para um Supermercado, com o nome de Pingo Salgado. 

Este Supermercado tem o objetivo de trazer aos clientes os produtos mais frescos e com melhor preço-qualidade. Para este efeito o Supermercado é composto por vários funcionários. Cada funcionário tem um respetivo número de identificação, uma secção correspondente e uma escala, que identifica se o funcionário é trabalhador fixo, estagiário ou repositor. O número de identificação serve para facilitar a procura, identificação e organização de cada trabalhador fixo, estagiário ou repositor na base de dados e dentro do próprio Pingo Salgado. Os trabalhadores dividem-se por escalas, trabalhando em para-time ou full-time.

Os funcionários podem ter ou não formações, sendo estas de Higiene, Parafarmácia, Cortador de carne e amanhar peixe, podendo ter nenhuma, uma ou várias formações. Posto isto, na secção de Frente de Loja existe a divisão de Parafarmácia ou sem Parafarmácia.

Relativamente às secções, o Pingo Salgado é composto por Frente de Loja, Padaria, Café e Bolos, Frutas e Legumes, Talho, Peixaria, Charcutaria e Takeaway, Reposição, Limpeza, Gerência. Cada secção é identificada através de um código. A secção da Fruta e Legumes fecha mais cedo do que as restantes secções, portanto os horários dos funcionários vão também ser diferentes, sendo definidos pela sua secção e pela sua escala.

Os repositores externos não têm um horário fixo, assim sendo aparecem na loja quando é efetuado um pedido de reposição de Stock pois queremos proporcionar aos nossos clientes produtos frescos e com qualidade.

O Pingo Salgado armazena todos os dados referentes à gestão dos produtos, que se subdividem em quantidade, quantidade mínima e quantidade máxima. Isto com o intuito de cada produto ter obrigatoriamente uma determinada quantidade, para que quando o stock chegue a uma quantidade mínima os funcionários possam efetuar o pedido, e nunca faltarem produtos na loja. E é então através desta gestão que o funcionário percebe que é necessário efetuar um pedido de reposição de stock e o Supermercado Pingo Salgado se consegue manter organizado e com uma boa gestão de produtos, para que nunca deixemos ficar mal os clientes. 

Inicialmente começamos a colocar em prática tudo o que tínhamos idealizado, fazendo o Modelo Entidade Associação e o respetivo Diagrama. Com a evolução do trabalho constatamos que existiam vários erros e problemas nomeadamente os horários dos funcionários e dos estagiários que eram definidos pela sua secção, a divisão de repositores internos e externos, os horários dos funcionários, a inexistência de escala e classes de funcionários, e o horário dos camiões que era definido pelo Stock, não tendo nada que definisse o Stock em si. Posto isto, refizemos o enunciado e o respetivo Modelo Entidade Associação, alterando vários tópicos no trabalho, removendo alguns como o horário dos camiões e acrescentando tantos outros, nomeadamente criar classes para a diferenciação de funcionários em: trabalhador fixo, estagiário ou repositor; dividir o Stock em produto e pedido; criar escalas nos funcionários, podendo trabalhar em full-time ou part-time; e mencionar as diferentes formações que cada funcionário pode ou não ter, estando numa tabela à parte. Depois de todas estas mudanças conseguimos melhorar o nosso sistema e torná-lo mais completo, eficaz e informativo.

---
[< Previous](rei00.md) | [^ Main](https://github.com/TCM-SIBD05/TCM-SIBD05) | [Next >](rei02.md)
:--- | :---: | ---: 