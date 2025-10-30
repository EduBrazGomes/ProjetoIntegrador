# Projetos de Ciência de Dados

## Questão 5: Comparação de Modelos para Predição de Doença Cardíaca

Este projeto realiza a predição de **doença cardíaca** com base em indicadores clínicos de pacientes, comparando o desempenho de dois modelos de classificação.

**Objetivo:**  
Comparar a eficácia dos modelos `Random Forest` e `SVM (Support Vector Machine)` para identificar se um paciente apresenta risco de doença cardíaca.

**Dataset:**  
`dataset_doenca_cardiaca_realista_500.csv`  
Contém atributos como idade, colesterol, pressão arterial e frequência cardíaca.

**Técnicas Utilizadas:**

**Pré-processamento:**
- `SimpleImputer` (para tratamento de valores ausentes)
- `StandardScaler` (para padronização das features)

**Modelos de Classificação:**
- `RandomForestClassifier`
- `SVC` (SVM com kernel RBF)

**Divisão Treino/Teste:**
- 70% / 30% com estratificação

**Métricas de Avaliação:**
- Matrizes de Confusão  
- Precision, Recall, F1-score  
- Curva ROC + AUC

**Etapas Executadas:**
- Carregamento e exploração inicial dos dados  
- Separação em variáveis preditoras (`X`) e alvo (`y`)  
- Aplicação de pré-processamento (Imputação de média e Padronização)  
- Divisão dos dados em treino e teste (70% / 30%)  
- Treinamento dos modelos Random Forest e SVM  
- Predição sobre os dados de teste para ambos os modelos  
- Avaliação e comparação de desempenho (Matrizes, Relatórios e Curvas ROC)

**Conclusão:**  
Ambos os modelos apresentaram boa capacidade preditiva. O `SVM (AUC = 0.82)` mostrou um desempenho ligeiramente superior ao `Random Forest (AUC = 0.81)`, conforme visto na curva ROC. O SVM obteve melhor precisão na classificação de pacientes com doença (Classe 1), enquanto o Random Forest teve um recall ligeiramente melhor para essa mesma classe.

---

## Questão 6: Previsão de Preços de Casas

Este projeto busca prever o **preço de casas** com base em características estruturais e localidade.

**Objetivo:**  
Estimar o valor de venda de imóveis.

**Dataset:**  
Arquivo contendo variáveis como:
- Área útil  
- Número de quartos  
- Localização  
- Ano de construção, entre outras

**Modelos Avaliados:**
- Regressão Linear  
- `Multi-Layer Perceptron (MLP) Regressor`  
- `XGBoost Regressor`

**Etapas do Projeto:**
- Coleta e análise dos dados  
- Tratamento de valores faltantes e normalização  
- Treinamento individual dos três modelos  
- Avaliação utilizando:
  - RMSE  
  - MAE  
  - R² Score  
- Comparação dos desempenhos

**Conclusão:**  
O `XGBoost` apresentou o melhor desempenho geral, devido à sua capacidade de capturar relações não lineares e lidar com variáveis complexas.

---

## Questão 7: Regras de Associação para Supermercado

Este projeto implementa a **mineração de padrões de compra** em um supermercado.

**Objetivo:**  
Identificar produtos que são frequentemente comprados juntos para apoiar estratégias de recomendação e marketing.

**Dataset:**  
`dataset_supermercado_simulado.csv`  
Contém registros de compras, cada linha representando uma cesta de produtos.

**Técnicas Aplicadas:**
- Transformação dos dados em formato de transações  
- Algoritmo `Apriori` para identificação de itemsets frequentes  
- Geração de Regras de Associação usando como métrica principal o **Lift**

**Etapas do Projeto:**
- Pré-processamento: divisão e limpeza dos itens  
- One-Hot Encoding usando `TransactionEncoder`  
- Aplicação do `Apriori` com suporte mínimo de 1%  
- Extração e ordenação das regras por **Lift**

**Conclusão:**  
As regras encontradas permitem identificar oportunidades de ofertas combinadas, precificação estratégica e organização de prateleiras com maior conversão.

---

## Questão 8: Sistema de Recomendação de Filmes

Este projeto implementa um **sistema de recomendação** para sugerir filmes a usuários com base em avaliações passadas.

**Objetivo:**  
Construir e comparar modelos de recomendação.

**Dataset:**  
`MovieLens`

**Técnicas:**  
Foram implementados dois modelos de **Filtragem Colaborativa**:
- Baseado em similaridade entre usuários  
- Baseado em similaridade entre itens (filmes)

**Conclusão:**  
A abordagem baseada em **itens (Item-Based)** se mostrou mais eficiente, apresentando uma menor margem de erro (RMSE e MAE).

---

## Questão 9: Classificação de Imagens de Raio-X com CNNs

Este projeto desenvolve um modelo de **Deep Learning** para classificar radiografias de tórax como “Normal” ou com “Pneumonia”.

**Objetivo:**  
Criar um classificador de imagens médicas para auxiliar no diagnóstico de doenças pulmonares.

**Dataset:**  
`Chest X-ray (Pneumonia)` do Kaggle.

**Técnicas:**  
Foi construída uma **Rede Neural Convolucional (CNN)**, utilizando técnicas de **Data Augmentation** para melhorar a generalização do modelo.

**Conclusão:**  
O modelo alcançou uma alta acurácia, demonstrando grande eficácia na identificação de casos de pneumonia.

⚠️ **Necessário API do Kaggle:**  
Assim como no projeto anterior, para executar este notebook, você precisará fazer o upload de um arquivo na primeira etapa “# Etapa 1: Configurar o ambiente e baixar o dataset de imagens”.  
Esse arquivo está nomeado como `kaggle.json` para baixar o dataset da competição do Kaggle.

---

## Questão 10: Previsão de Vendas Mensais

Este projeto visa prever as **vendas diárias** de uma rede de varejo com base em dados históricos e características das lojas.

**Objetivo:**  
Prever o volume de vendas para otimizar o gerenciamento de estoque e recursos.

**Dataset:**  
`Rossmann Store Sales` do Kaggle.

**Técnicas:**  
Foram aplicados três modelos de regressão:
- Regressão Linear  
- Árvore de Decisão  
- `XGBoost`

Foi realizada uma extensa etapa de **Feature Engineering** para extrair informações relevantes dos dados.

**Conclusão:**  
O modelo `XGBoost` apresentou o melhor desempenho, com a menor margem de erro.  
As variáveis de maior impacto nas vendas foram a **presença de promoções (Promo)**, o **tipo de loja (StoreType)** e o **tipo de sortimento de produtos (Assortment)**.

⚠️ **Necessário API do Kaggle:**  
Assim como no projeto anterior, para executar este notebook, você precisará fazer o upload de um arquivo na primeira etapa “# Etapa 1: Configurar o ambiente e baixar o dataset de vendas”.  
Esse arquivo está nomeado como `kaggle.json` para baixar o dataset da competição do Kaggle.
