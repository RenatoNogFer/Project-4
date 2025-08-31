# Project-4

## Introdução

Este repositório foi criado para o desenvolvimento de uma solução para o desafio técnico "Projeto 4: modelo de propensão a fraude em financiamento veicular", cuja essência é a detecção de fraudes de pagamento através da previsão do ```First Payment Default```, o não pagamento da primeira parcela do financiamento.

## Modelo Final

Utilizou-se ao final de um modelo LGBM com o objetivo de gerar *scores* que sejam proporcionais ao risco envolvido naquele financiamento, i.e, maior o *score*, maior o risco envolvendo aquele financiamento.

## Métricas-Chave

A descrição do projeto afirma "O nosso objetivo aqui é mapear e alertar os clientes fraudadores trazendo o mínimo de impacto e o máximo de retorno financeiro à operação do cliente (portanto, alertando poucos casos, mas com alta precisão).". Mediante isso, estaríamos olhando primariamente para:

* Precisão
* Recall
* F-beta Score
* AUC-PR

Porém, trazendo para o contexto de problemas de crédito e levando em conta a natureza desbalanceada do conjunto de dados para o problema, adotamos métricas que buscam mostrar a capacidade da variável de risco gerada pelo modelo, o *score*, de discernir os casos positivos dos negativos na base de dados, priorizando então:

* KS%
* Lift

Além disso, propõe-se uma métrica de estimativa de retorno financeiro do modelo, baseada no valor que deixou de ser financiado corretamente pelo valor que deixou de ser financiado incorretamente. 

## To-Do

[X] Análise exploratória dos dados<br>
[X] Modelagem<br>
[X] Validação<br>
[X] Apresentação
[ ] Refatoração

## Links relevantes

* [Descrição do projeto](https://github.com/Neurolake/challenge-data-scientist/blob/main/credit/README.md#projeto-4-modelo-de-propens%C3%A3o-a-fraude-em-financiamento-veicular)
* [Base de Dados](https://github.com/Neurolake/challenge-data-scientist/blob/main/datasets/base_antifraude.gz)