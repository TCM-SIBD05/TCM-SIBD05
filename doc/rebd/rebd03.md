# C3 : Normalização

## Relações

Funcionários
| Id | Nome | Idade | Sexo | Salário | Entrada | Saída | Secção | Classe | Escala | #id -> Secção |
| :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: |

Formação
| Id | Nome |
| :----: | :----: |

| Id | Nome | HoraAbertura | HoraFecho | #id -> Formação |
| :----: | :----: | :----: | :----: | :----: |

ConstituidoPor
| #id -> Pedido | #id -> Produto | Quantidade |
| :----: | :----: | :----: |

Faz
| #id -> Funcionário | #id -> Formação |
| :----: | :----: |


## Normalização do Esquema Relacional

Funcionários

Id | Nome | Idade | Sexo | Salário | Entrada | Saída | Secção | Classe | Escala |
:---: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: |
250 | Raul Dias | 65 | M | 1500 | 08:30:00 | 21:30:00 | Gerência | Funcionário | Full-time |
251 | Carlos Ferreira | 36 | M | 1000 | 11:00:00 | 20:00:00 | Gerência | Funcionário | Full-time |
252 | Ana Sousa | 54 | F | 635 | 07:00:00 | 16:00:00 | Limpeza | Funcionário | Full-time |
253 | Tânia Fonseca | 42 | F | 635 | 13:00:00 | 22:00:00 | Limpeza | Funcionário | Full-time |
254 | Teresa Moreira | 45 | F | 320 | 10:00:00 | 14:00:00 | Reposição | Funcionário | Part-time |
255 | Rita Vaz | 19 | F | 635 | 06:00:00 | 15:00:00 | Reposição | Funcionário | Full-time |
256 | João Silva | 24 | M | 635 | 10:00:00 | 19:00:00 | Reposição | Funcionário | Full-time |
257 | Fábio Ferreira | 39 | M | 650 | 09:00:00 | 18:00:00 | Reposição | Funcionário | Full-time |
258 | Joana Lamelas | 25 | F | 320 |17:00:00 | 21:00:00 | Reposição | Funcionário |Part-time |

Formação

| Id | Nome |
| :----: | :----: |
| 50 | Cortador de Carne |
| 51 | Amanhar peixe |
| 52 | Higiene |
| 53 | Parafarmácia |

Secção
| Id | Nome | Hora Abertura | Hora Fecho
| :----: | :----: | :----: | :----: | 
| 54 | Gerência| 08:30:00 | 21:030:00
| 55 | Limpeza | 07:00:00 | 22:00:00
| 56 | Reposição | 06:00:00 | 21:00:00
| 57 | Charcutaria e Take-Away | 08:30:00 | 21:30:00
| 58 | Peixaria| 07:00:00 | 22:00:00
| 59 | Talho| 07:00:00 | 22:00:00
| 60 | Frutas e Legumes| 08:30:00 | 21:30:00
| 61 | Padaria | 08:00:00 | 21:00:00
| 62 | Frente Loja| 08:00:00 | 21:30:00

Produto

| Id | Nome | Quantidade Mínima | Quantidade Maxima
| :----: | :----: | :----: | :----: | 
| 63 | Lenços| 50 | 100
| 64 | Coca-cola| 200| 500
| 65 | Bolacha Maria| 150| 250
| 66 | Chá Preto| 60| 120
| 67 | Ração Cão| 130 | 21
| 68 | Arroz| 300 | 600
| 69 | Leite| 100 | 200
| 70 | Vassoura| 10 | 20
| 71 | Papel Higiénico| 150| 250
| 72 | Cerveja| 300 | 50

Pedido
| Id | dataPedido | dataReposição |
| :---: | :----: | :----: |
| 1 | 05-01-2021 | 15-01-2021 |
| 3 | 18-02-2021 | 20-02-2021 |
| 5 | 31-05-2021 | 02-06-2021 |
| 7 | 06-01-2021 | 22-01-2021 |
| 2 | 24-09-2021 | 28-09-2021 |
| 9 | 22-12-2021 | 24-12-2021 |
| 3 | 05-05-2021 | 10-05-2021 |
| 3 | 10-09-2021 | 16-09-2021 |
| 1 | 15-02-2021 |15-03-2021 |
| 10 | 27-02-2021 | 28-02-2021 |


---
[< Previous](rebd02.md) | [^ Main](https://github.com/TCM-SIBD05/TCM-SIBD05) | [Next >](rebd04.md)
:--- | :---: | ---: 






