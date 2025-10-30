🩺 Questão 5 — Classificação de Doença Cardíaca

Nesta atividade foi utilizado um dataset médico contendo variáveis como idade, pressão arterial e colesterol para prever a presença de doença cardíaca.

Modelo: Random Forest Classifier

Avaliação: Acurácia, Matriz de Confusão, Relatório de Classificação e Curva ROC

Resultado: Acurácia aproximada de 0.72

Objetivo: Demonstrar como modelos de classificação podem auxiliar decisões clínicas.

🏠 Questão 6 — Previsão de Preços de Imóveis

Foi analisado um conjunto de dados contendo características estruturais e localização de imóveis para estimar seu preço de mercado.

Pré-processamento: StandardScaler (numéricas) + OneHotEncoder (categóricas)

Modelos avaliados:

Regressão Linear

XGBoost

Rede Neural (MLP)

Métricas: RMSE e R²

Conclusão: A Regressão Linear apresentou o melhor desempenho (R² ≈ 0.88).

🛒 Questão 7 — Regras de Associação em Supermercado

Utilizando um dataset de listas de compras, foram descobertos padrões de coocorrência entre produtos.

Técnicas: TransactionEncoder, Apriori, Regras de Associação (Lift)

Exemplo de padrão encontrado: iogurte ↔ manteiga ↔ pão

Aplicação prática: Estratégias de marketing e organização de prateleiras.

🎬 Questão 8 — Sistema de Recomendação de Filmes

Implementação de um sistema de recomendação baseado no dataset MovieLens.

Método: Filtragem Colaborativa

Abordagens comparadas:

Similaridade entre usuários (User-Based)

Similaridade entre itens (Item-Based)

Resultado: O modelo Item-Based apresentou menor erro (MAE / RMSE).

🩻 Questão 9 — Classificação de Imagens de Raio-X (CNN)

Desenvolvimento de um modelo para identificar pneumonia em radiografias.

Dataset: Chest X-ray (Pneumonia) — Kaggle

Modelo: Rede Neural Convolucional (CNN) com Data Augmentation

Resultado: Alta acurácia e boa capacidade de generalização

⚠️ Importante: É necessário fazer upload do arquivo kaggle.json para baixar o dataset.

🏪 Questão 10 — Previsão de Vendas Diárias (Time Series / ML)

Modelo para prever vendas de lojas utilizando dados históricos e características comerciais.

Dataset: Rossmann Store Sales — Kaggle

Modelos avaliados: Regressão Linear, Árvore de Decisão e XGBoost

Resultado: XGBoost apresentou o melhor desempenho

Variáveis mais importantes: Promo, StoreType e Assortment

⚠️ Importante: É necessário o arquivo kaggle.json para baixar os dados.

🛠️ Tecnologias Utilizadas
Biblioteca / Ferramenta	Uso
Python	Linguagem base
Pandas / NumPy	Manipulação e análise de dados
Scikit-Learn	Modelos de ML e pré-processamento
XGBoost	Regressão avançada e boosting
Mlxtend	Regras de associação (Apriori)
Matplotlib / Seaborn	Visualização de dados
TensorFlow / Keras	Redes neurais e CNNs


