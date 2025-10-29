# ProjetoIntegrador

QUESTÃO 5 

Avaliação de Modelos de Classificação: Random Forest vs SVM

Neste exercício, utilizamos um conjunto de dados contendo 500 amostras, onde 30% (150 amostras) foram separadas para teste. O objetivo foi comparar o desempenho de dois modelos de classificação para prever a presença de uma doença:

Modelo 1: Random Forest

Modelo 2: SVM (Support Vector Machine)

A análise foi conduzida utilizando as métricas: Recall (Sensibilidade), Precision (Precisão), Accuracy (Acurácia), F1-Score, Support e a Matriz de Confusão, além da comparação da curva ROC (AUC).

Recall (Sensibilidade)

O recall mede a capacidade do modelo de identificar corretamente os casos positivos reais.

Modelo 1:

Classe 0 (sem doença): 77% dos 71 casos reais de pessoas sem doença foram classificados corretamente.

Classe 1 (com doença): 67% dos 79 casos reais de pessoas com doença foram identificados corretamente.

Modelo 2:

Classe 0 (sem doença): 82% dos 71 casos reais foram classificados corretamente.

Classe 1 (com doença): 70% dos 79 casos reais foram corretamente identificados.

Precision (Precisão)

A precisão mede quantos dos casos previstos como positivos realmente são positivos.

Modelo 1:

Classe 0: 68% das previsões de "sem doença" estavam corretas.

Classe 1: 77% das previsões de "com doença" estavam corretas.

Modelo 2:

Classe 0: 71% das previsões de "sem doença" estavam corretas.

Classe 1: 81% das previsões de "com doença" estavam corretas.

Accuracy (Acurácia)

Percentual total de acertos nos 150 testes:

Modelo 1: 72% de acertos (aprox. 108 previsões corretas)

Modelo 2: 75% de acertos (aprox. 112,5 previsões corretas)

F1-Score

Combina precisão e recall em uma única métrica balanceada.

Modelo 1:

Classe 0: 0,72

Classe 1: 0,72

Modelo 2:

Classe 0: 0,76

Classe 1: 0,75

Support

Quantidade de amostras por classe no conjunto de teste:

Classe 0 (sem doença): 71

Classe 1 (com doença): 79
(igual para ambos os modelos)

Matriz de Confusão

Modelo 1

[[55 16]
 [26 53]]


Modelo 2

[[58 13]
 [24 55]]

Curva ROC (AUC)

Modelo 1: AUC ≈ 0.80

Modelo 2: AUC ≈ 0.85

Interpretação de AUC:

0.80 – 0.90: Muito bom desempenho

Conclusão

O modelo SVM apresentou desempenho superior ao Random Forest, considerando:

Maior F1-Score em ambas as classes

Maior acurácia (75% contra 72%)

Melhor recall e precisão, especialmente para a classe positiva (com doença)

Maior área sob a curva ROC (0.85 vs 0.80)

Portanto, o SVM é o modelo mais adequado para este problema, demonstrando melhor equilíbrio entre detecção correta da doença e confiabilidade nas previsões.
