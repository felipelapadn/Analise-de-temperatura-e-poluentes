# Análise de temperatura e poluentes

O objetivo deste trabalho é estimar um modelo estilo _Random Forest Regressor_, com base no algoritmo de Florestas Aleatórias e relacionado à temperatura média. A elaboração do trabalho é baseada em três etapas, a primeira voltada à aquisição dos dados, a segunda etapa é referente à limpeza dos dados e a terceira é sobre o modelo, essa etapa apresenta alguns pontos importantes a serem observados, já que ocorreu a escolha das variáveis para construir o modelo e a sua validação. Apesar das buscas por parâmetros com o _GridSearchCV_ e _RandomSearchCV_ em dois espaços, os melhores resultados foram obtidos com o modelo _Random Forest Regressor_ treinado a partir dos parâmetros padrões, que alcançou um _score_ de 98,07%, um MSE de 0,0063 e um RMSE muito baixo.

## Resultados

Os melhores resultados foram obtidos com o modelo treinado a partir dos parâmetros padrões, ou seja, as buscas por parâmetros com o _GridSearchCV_ e _RandomSearchCV_ em ambos os espaços não geraram um bom resultado, o motivo dessa situação provavelmente se deve ao fato do espaço de parâmetros não ser escolhido de uma forma estratégica. As avaliações do modelo _Random Forest Regressor_ são apresentados na Tabela 1, o gráfico de dispersão, representado na Figura 1, ilustra os resultados das predições de acordo com reta de regressão, nesse gráfico, quanto mais ajustados forem os círculos a reta traçada, melhor será o desempenho do modelo. Já na Figura 2, é possível observar que os dados gerados pelo modelo, linha de cor ciano, apresentaram instabilidades em relação aos dados reais, linha tracejada, ou seja, em alguns momentos o modelo realizou a previsão de picos que nunca existiram. 

Tabela 1: Valores as métricas geradas com base no modelo _Random Forest Regressor_.
| **Métrica de avaliação**| **Resultado** |
| --- | --- |
| *Score* | 98,07% |       
| MSE | 0,0063 |
| RMSE | 4,0604065270581914.10 $^{-5}$ |
