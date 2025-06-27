# 🏠 Previsão de Preço de Imóveis - King County

Este repositório apresenta um projeto de Machine Learning para prever o preço de imóveis residenciais no condado de King (Seattle, WA).

## 📌 Descrição

- **Dataset:** kc_house_data.csv
- **Modelos:** Regressão Linear, Árvore de Decisão, KNN Regressor
- **Ferramentas:** Python, scikit-learn, Pandas, Matplotlib
- **Avaliação:** R², RMSE, gráficos de Previsão vs Valor Real

## ⚙️ Pipeline

1. **Leitura e Análise Explorátoria**
2. **Pré-processamento:**
   - Conversão de datas
   - Extração de ano, mês e dia
   - Escalonamento para KNN
3. **Divisão treino/teste**
4. **Modelagem:**
   - GridSearchCV para otimizar hiperparâmetros
   - Comparação de desempenho
5. **Visualização de resultados**

## 📈 Resultados

| Modelo              | R² Treino | R² Teste |
|---------------------|-----------|----------|
| Linear Regression   | 0.6864    | 0.7019   | 
| Decision Tree       | 0.6950    | 0.6987   | 
| KNN Regressor       | 0.6987    | 0.6922   |


## 🚀 Como Executar

```bash
# Instale dependências
pip install -r requirements.txt

/king-county-house-prices/
├── data/
│   └── kc_house_data.csv
├── notebooks/
│   └── 01_data_preprocessing.ipynb
│   └── 02_model_training.ipynb
│   └── 03_visualization.ipynb
├── outputs/
│   ├── models/
│   │   └── knn_model.pkl
│   │   └── dtree_model.pkl
│   │   └── linreg_model.pkl
│   ├── figures/
│   │   └── knn_real_vs_pred.png
│   │   └── dtree_real_vs_pred.png
│   │   └── linreg_real_vs_pred.png
├── requirements.txt
├── README.md
└── .gitignore

# Execute o notebook ou script principal
