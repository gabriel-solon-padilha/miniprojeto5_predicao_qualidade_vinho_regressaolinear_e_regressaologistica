# miniprojeto5_predicao_qualidade_vinho_regressaolinear_e_regressaologistica
Meu quinto miniprojeto em python no qual faço uma análise da qualidade do vinho usando modelos de machine learning de regressão linear e de regressão logística

Os datasets são dados sobre vinhos tintos e vinhos brancos com as seguintes features e target:

Attribute Information:

Input variables (based on physicochemical tests):
- 1 - fixed acidity
- 2 - volatile acidity
- 3 - citric acid
- 4 - residual sugar
- 5 - chlorides
- 6 - free sulfur dioxide
- 7 - total sulfur dioxide
- 8 - density
- 9 - pH
- 10 - sulphates
- 11 - alcohol

Output variable (based on sensory data): <br>
- 12 - quality (score between 0 and 10)

Os dados foram retirados do repositorio de machine learnind da UCI e para mais informações sobre os datasets segue o link do mesmo:

https://archive.ics.uci.edu/ml/datasets/Wine+Quality

Esse miniprojeto foi dividido em 4 grandes etapas:

1) Análise exploratória dos dados (EDA)
2) Criação de um modelo de regressão linear multipla e posteriomente com as penalizações Lasso, Ridge e Elastic-net
3) Criação de um modelo de classificação usando a regressão logística com ajuste fino de threshold
4) Conclusões sobre o uso de cada um dos modelos e conclusão geral
