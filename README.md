# Projetos de Ciência de Dados

---

## Questão 5: Predição de Doença Cardíaca com Random Forest

Este projeto realiza a predição de **doença cardíaca** com base em indicadores clínicos de pacientes.

**Objetivo:**  
Identificar se um paciente apresenta risco de doença cardíaca.

**Dataset:**  
`dataset_doenca_cardiaca_realista_500.csv`  
Contém atributos como idade, colesterol, pressão arterial e frequência cardíaca.

**Técnicas Utilizadas:**  
- `RandomForestClassifier` para classificação  
- Divisão Treino/Teste (70% / 30%)  
- Métricas de Avaliação:
  - Acurácia
  - Matrizes de Confusão
  - Precision, Recall, F1-score
  - Curva ROC + AUC

**Etapas Executadas:**  
1. Carregamento e exploração inicial dos dados  
2. Separação em variáveis preditoras e alvo  
3. Treinamento do modelo de Random Forest  
4. Predição sobre os dados de teste  
5. Avaliação do desempenho e interpretação da curva ROC

**Conclusão:**  
O modelo apresentou boa capacidade preditiva, com desempenho equilibrado entre precisão e recall, mostrando-se eficiente para análise clínica preliminar.

---

## Questão 6: Previsão de Preços de Casas

Este projeto busca prever o preço de casas com base em características estruturais e localidade.

**Objetivo:**  
Estimar o valor de venda de imóveis.

**Dataset:**  
Arquivo contendo variáveis como:  
- Área útil  
- Número de quartos  
- Localização  
- Ano de construção, entre outras.

**Modelos Avaliados:**  
- Regressão Linear  
- Multi-Layer Perceptron (MLP) Regressor  
- **XGBoost Regressor**

**Etapas do Projeto:**  
1. Coleta e análise dos dados  
2. Tratamento de valores faltantes e normalização  
3. Treinamento individual dos três modelos  
4. Avaliação utilizando:
   - RMSE
   - MAE
   - R² Score  
5. Comparação dos desempenhos

**Conclusão:**  
O **XGBoost** apresentou o melhor desempenho geral, devido à sua capacidade de capturar relações não lineares e lidar com variáveis complexas.

---

## Questão 7: Regras de Associação para Supermercado

Este projeto implementa a **mineração de padrões de compra** em um supermercado.

**Objetivo:**  
Identificar produtos que são frequentemente comprados juntos para apoiar estratégias de **recomendação e marketing**.

**Dataset:**  
`dataset_supermercado_simulado.csv`  
Contém registros de compras, cada linha representando uma cesta de produtos.

**Técnicas Aplicadas:**  
- Transformação dos dados em formato de transações  
- Algoritmo **Apriori** para identificação de itemsets frequentes  
- Geração de **Regras de Associação** usando como métrica principal o `Lift`

**Etapas do Projeto:**  
1. Pré-processamento: divisão e limpeza dos itens  
2. One-Hot Encoding usando `TransactionEncoder`  
3. Aplicação do Apriori com suporte mínimo de 1%  
4. Extração e ordenação das regras por `Lift`

**Conclusão:**  
As regras encontradas permitem identificar oportunidades de ofertas combinadas, precificação estratégica e organização de prateleiras com maior conversão.

---

## Questão 8: Sistema de Recomendação de Filmes

Este projeto implementa um sistema para sugerir filmes a usuários com base em avaliações passadas.

**Objetivo:**  
Construir e comparar modelos de recomendação.

**Dataset:**  
MovieLens.

**Técnicas:**  
Foram implementados dois modelos de Filtragem Colaborativa:  
- Baseado em similaridade entre usuários  
- Baseado em similaridade entre itens (filmes)

**Conclusão:**  
A abordagem baseada em itens (Item-Based) se mostrou mais eficiente, apresentando uma menor margem de erro (RMSE e MAE).

---

## Questão 9: Classificação de Imagens de Raio-X com CNNs

Este projeto desenvolve um modelo de Deep Learning para classificar radiografias de tórax como "Normal" ou com "Pneumonia".

**Objetivo:**  
Criar um classificador de imagens médicas para auxiliar no diagnóstico de doenças pulmonares.

**Dataset:**  
Chest X-ray (Pneumonia) do Kaggle.

**Técnicas:**  
Foi construída uma Rede Neural Convolucional (CNN), utilizando técnicas de Data Augmentation para melhorar a generalização do modelo.

**Conclusão:**  
O modelo alcançou uma alta acurácia, demonstrando grande eficácia na identificação de casos de pneumonia.

⚠️ **Necessário API do Kaggle:**  
Assim como no projeto anterior, para executar este notebook, você precisará fazer o upload de um arquivo na primeira etapa "# Etapa 1: Configurar o ambiente e baixar o dataset de imagens" esse arquivo está nomeado como `kaggle.json` para baixar o dataset da competição do Kaggle.

---

## Questão 10: Previsão de Vendas Mensais

Este projeto visa prever as vendas diárias de uma rede de varejo com base em dados históricos e características das lojas.

**Objetivo:**  
Prever o volume de vendas para otimizar o gerenciamento de estoque e recursos.

**Dataset:**  
Rossmann Store Sales do Kaggle.

**Técnicas:**  
Foram aplicados três modelos de regressão:  
- Regressão Linear  
- Árvore de Decisão  
- XGBoost  

Foi realizada uma extensa etapa de Feature Engineering para extrair informações relevantes dos dados.

**Conclusão:**  
O modelo XGBoost apresentou o melhor desempenho, com a menor margem de erro. As variáveis de maior impacto nas vendas foram a presença de promoções (`Promo`), o tipo de loja (`StoreType`) e o tipo de sortimento de produtos (`Assortment`).

⚠️ **Necessário API do Kaggle:**  
Assim como no projeto anterior, para executar este notebook, você precisará fazer o upload de um arquivo na primeira etapa "# Etapa 1: Configurar o ambiente e baixar o dataset de vendas" esse arquivo está nomeado como `kaggle.json` para baixar o dataset da competição do Kaggle.
