# 🏠 House Prices — Análise de Dados & Machine Learning (Desafio C3)

Projeto completo de Ciência de Dados sobre o dataset **House Prices: Advanced Regression Techniques** (Ames, Iowa — Kaggle), cobrindo todo o ciclo: análise exploratória, engenharia de features, aprendizagem supervisionada e não supervisionada.

## 📊 Sobre o projeto

A partir de **1.460 casas** descritas por **79 características**, investigamos o que determina o preço de um imóvel e construímos modelos para prevê-lo. O notebook é narrado em formato de *storytelling*, contando a história que os dados revelam.

## 🗂️ Estrutura do repositório

```
.
├── House_Prices_Desafio_C3.ipynb   # Notebook principal (executar no Google Colab)
├── data/
│   ├── train.csv                   # Base de treino (Kaggle)
│   └── test.csv                    # Base de teste (Kaggle)
├── requirements.txt                # Dependências
└── README.md
```

## 🚀 Como executar

### Opção 1 — Google Colab (recomendado)
1. Abra o notebook no [Google Colab](https://colab.research.google.com/).
2. Execute a primeira célula (instala `mlxtend` e `xgboost`).
3. Quando solicitado, faça o **upload do arquivo `train.csv`** (baixe em [Kaggle House Prices](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data)).
4. Rode todas as células: `Ambiente de execução → Executar tudo`.

### Opção 2 — Local
```bash
pip install -r requirements.txt
jupyter notebook House_Prices_Desafio_C3.ipynb
```

## 🧪 Técnicas aplicadas

| Etapa | Técnicas |
|-------|----------|
| **Análise Exploratória** | Distribuições, correlações, mapa de calor, análise de faltantes e outliers |
| **Feature Engineering** | Tratamento de NA por domínio, criação de features (`TotalSF`, `TotalBath`, `HouseAge`...), one-hot encoding, transformação log |
| **Regressão** | Linear, Ridge, Lasso, Random Forest, Gradient Boosting, XGBoost |
| **Classificação** | Regressão Logística, KNN, Árvore de Decisão, Random Forest |
| **Clusterização** | K-Means (cotovelo + silhueta) |
| **Redução de Dimensionalidade** | PCA (variância explicada + projeção 2D) |
| **Associação** | Apriori (regras suporte/confiança/lift) |
| **Detecção de Outliers** | Local Outlier Factor (LOF) |

## 📈 Principais resultados

- **Regressão:** Gradient Boosting / XGBoost com **R² ≈ 0,90** (erro médio ~US$ 20 mil).
- **Classificação:** ~**93% de acurácia** e **AUC ≈ 0,98** separando casas caras de baratas.
- **Clusterização:** 3 perfis naturais — Econômicas, Padrão e Premium.
- **PCA:** poucas componentes retêm 95% da informação de 200+ colunas.
- **Apriori:** regras como *"Alta qualidade + grande → caro"* (lift > 1).

## 📚 Métricas de avaliação

- **Regressão:** RMSE, MAE, R².
- **Classificação:** Acurácia, Precisão, Recall, F1, AUC-ROC, matriz de confusão.
- **Clusterização:** Inércia (cotovelo) e Coeficiente de Silhueta.

## 👥 Equipe

- Adicione aqui os nomes dos integrantes do grupo.

---
*Desafio C3 — Data Analysis and Machine Learning Hackathon · FAESA Centro Universitário*
