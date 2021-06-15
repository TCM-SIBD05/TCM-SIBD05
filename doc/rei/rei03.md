# C3 : Esquema conceptual

## Modelo E/A
Entidades:

FUNCIONARIO (Id, nome, idade, sexo, salario, entrada, saida, seccao, classe, escala)
FORMACAO (Id, nome)
SECCAO (Id, nome, horaAbertura, horaFecho)
PRODUTO (Id, quantidade, quantidadeMinima, quantidadeMaxima)
PEDIDO (Id, dataPedido, dataReposicao)

Associações:

atribuidoA (FUNCIONARIO, SECCAO)   N:1   T/P                       
dependeDe (FORMACAO, SECCAO)   1:1   P/P
constituidoPor (PEDIDO, PRODUTO, quantidade)   N:M   T/P
executa (FUNCIONARIO, PEDIDO)   1:N   T/P
faz (FUNCIONARIO, FORMAÇÃO)   N:M   P/P


![Diagrama Modelo EA] (images/Diagrama.png)


---
[< Previous](rei02.md) | [^ Main](https://github.com/TCM-SIBD05/TCM-SIBD05) | Next >
:--- | :---: | ---: 
