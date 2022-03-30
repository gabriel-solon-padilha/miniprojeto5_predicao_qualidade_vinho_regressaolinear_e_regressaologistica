# Predição da qualidade do vinho usando algorítmos de regressão e classificação

---------------------------

## Introdução


Meu primeiro projeto de machine learning no qual faço uma análise da qualidade do vinho usando modelos de machine learning de regressão linear e de regressão logística. Os datasets são dados sobre vinhos tintos e vinhos brancos com as seguintes features e target:

Features:
- fixed acidity
- volatile acidity
- citric acid
- residual sugar
- chlorides
- free sulfur dioxide
- total sulfur dioxide
- density
- pH
- sulphates
- alcohol

Target:
- quality (score between 0 and 10)

Os dados foram retirados do repositorio de machine learnind da UCI e para mais informações sobre os datasets segue o link do mesmo:
https://archive.ics.uci.edu/ml/datasets/Wine+Quality

--------------

## Desenvolvimento

1) Análise exploratória dos dados (EDA)
2) Criação de um modelo de regressão linear multipla e posteriomente com as penalizações Lasso, Ridge e Elastic-net
3) Criação de um modelo de classificação usando a regressão logística com ajuste fino de threshold
4) Conclusões sobre o uso de cada um dos modelos e conclusão geral

## Resultados alcançados e conclusão

- Recall: 0,803
- Precision: 0,802

A predição do vinho a partir de um modelo de regressão claramente não foi a melhor escolha, um dos motivos é a qualidade do vinho ser uma medição discreta e a regressão linear fazer predições de valores contínuis, só isso já aumenta muito os resídulos e dificulta o aprendizado correto do modelo. Ao usar um modelo de classificação o problema de underfit que encontramos na regressão linear já é resolvido e começamos a ter % de acerto na base de teste muito superiores aos da regressão. Dessa forma, o caminho de adotar um modelo de classificação se torna muito mais adequado, sendo necessário somente adequar o threshold para se conseguir uma melhor precision (descartar vinhos ruins) ou recall (recomendar vinhos bons) de acordo com o objetivo do negócio ao criar esse modelo. Nesse projeto foi usada somente a regressão logística para a classificação, porém existem outros modelos que poderiam ser usados e que talvez fossem melhor para prever o comportamento da qualidade do vinho.


