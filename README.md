📝 Questão 8: Sistema de Recomendação de Filmes
Este projeto implementa um sistema para sugerir filmes a usuários com base em avaliações passadas.

Objetivo: Construir e comparar modelos de recomendação.

Dataset: MovieLens.

Técnicas: Foram implementados dois modelos de Filtragem Colaborativa: um baseado em similaridade entre usuários e outro em similaridade entre itens (filmes).

Conclusão: A abordagem baseada em itens (Item-Based) se mostrou mais eficiente, apresentando uma menor margem de erro (RMSE e MAE).

🩺 Questão 9: Classificação de Imagens de Raio-X com CNNs
Este projeto desenvolve um modelo de Deep Learning para classificar radiografias de tórax como "Normal" ou com "Pneumonia".

Objetivo: Criar um classificador de imagens médicas para auxiliar no diagnóstico de doenças pulmonares.

Dataset: Chest X-ray (Pneumonia) do Kaggle.

Técnicas: Foi construída uma Rede Neural Convolucional (CNN), utilizando técnicas de Data Augmentation para melhorar a generalização do modelo.

Conclusão: O modelo alcançou uma alta acurácia, demonstrando grande eficácia na identificação de casos de pneumonia.

⚠️ Necessário API do Kaggle: Assim como no projeto anterior, para executar este notebook, você precisará fazer o upload de um arquivo na primeira etapa "# Etapa 1: Configurar o ambiente e baixar o dataset de imagens" esse arquivo está nomeado como "kaggle.json" para baixar o dataset da competição do Kaggle.

📈 Questão 10: Previsão de Vendas Mensais
Este projeto visa prever as vendas diárias de uma rede de varejo com base em dados históricos e características das lojas.

Objetivo: Prever o volume de vendas para otimizar o gerenciamento de estoque e recursos.

Dataset: Rossmann Store Sales do Kaggle.

Técnicas: Foram aplicados três modelos de regressão: Regressão Linear, Árvore de Decisão e XGBoost. Foi realizada uma extensa etapa de Feature Engineering para extrair informações relevantes dos dados.

Conclusão: O modelo XGBoost apresentou o melhor desempenho, com a menor margem de erro. As variáveis de maior impacto nas vendas foram a presença de promoções (Promo), o tipo de loja (StoreType) e o tipo de sortimento de produtos (Assortment).

⚠️ Necessário API do Kaggle: Assim como no projeto anterior, para executar este notebook, você precisará fazer o upload de um arquivo na primeira etapa " # Etapa 1: Configurar o ambiente e baixar o dataset de vendas" esse arquivo está nomeado como "kaggle.json" para baixar o dataset da competição do Kaggle.


