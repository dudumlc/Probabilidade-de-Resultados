# Analise de Probabilidade de Resultados no Futebol - Abordagem Estatística

## 📊 O que é ?
Este projeto consiste em uma análise de probabilidades de resultados de partidas de futebol utilizando a distribuição de Poisson. Ele foi desenvolvido para ajudar na previsão de placares e no cálculo de pontos esperados para cada time com base em suas métricas de "expected goals" (xG).

Essa abordagem é útil para:
- Previsão de resultados esportivos.
- Planejamento estratégico de partidas.
- Análise estatística em estudos esportivos.

## 📈 Metodologia
### 1. Métrica de Expected Goals (xG)
O primeiro passo é pegar a métrica de Expected Goals (xG) dos times envolvidos na partida análise (Caso não saiba o que significa o xG, confira o meu projeto _ que eu explico esse conceito mais claramente). Porém, para a análise ficar ainda mais precisa, não é aconselhado utilizar o xG geral do time, mas sim o xG específico do campeonato que está sendo analisado e diferenciando se o jogo é em casa ou fora. Isso porque o modo com que cada time joga muda em relação à competição e em relação à estar jogando em casa ou fora, o que impacta diretamente as probabilidades de gols.
Ex.: Jogo Analisado - Cruzeiro e Grêmio pelo Brasileirão 2024. Usa-se o xG do Cruzeiro jogando em casa pelo Brasileirão e o xG do Grêmio sendo visitante também pelo Brasileirão.

### 2. Distribuição Poisson
A distribuição de Poisson é uma distribuição de probabilidade discreta que expressa a probabilidade de um determinado número de eventos ocorrer em um intervalo fixo. Dessa forma, com os gols esperados dos times em mãos, utilliza-se a distribuição Poisson para analisar qual a probabilidade do time fazer cada quantidade de gols.
Como resultado, gera-se dois vetores com as probabilidades de ocorrência de cada quantidade de gols de cada time.
###
![image](https://github.com/user-attachments/assets/b4d604dd-ece2-4d17-93b9-54e819267382)


### 3. Análise de Placares
Foram testados diferentes algoritmos de aprendizado de máquina, incluindo:
Regressão Linear
Árvore de Decisão
Random Forest
XGBoost
Cada modelo foi comparado usando métricas como RMSE (Root Mean Squared Error) e MAE (Mean Absolute Error) para determinar qual oferecia as previsões mais precisas.

5. Otimização dos Hiperparâmetros
Após a seleção do modelo com melhor desempenho, foi realizada uma otimização dos hiperparâmetros utilizando GridSearchCV e RandomizedSearchCV, melhorando ainda mais a precisão das previsões.

## 📊 Resultados e Conclusão
Ao final, o modelo otimizado mostrou-se eficaz para prever a presença do público nos jogos do Cruzeiro, com boa acurácia e uma margem de erro reduzida, ajudando a equipe de logística e planejamento do clube a se preparar de forma mais assertiva para os eventos.
