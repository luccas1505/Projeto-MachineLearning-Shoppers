# Projeto de Machine Learning – Intenção de Compra de Usuários Online

Esse projeto foi desenvolvido para analisar e prever a intenção de compra de usuários em um site de e-commerce, usando o dataset Online Shoppers Purchasing Intention. A ideia foi aplicar diferentes modelos de machine learning, avaliar o desempenho deles e entender melhor o comportamento dos dados com ferramentas de interpretabilidade.

## Etapas do projeto

### Questão 5 – Abertura e Pré-processamento
- Carreguei o dataset e criei a variável-alvo a partir da coluna Revenue.
- Separei os preditores do alvo e fiz o pré-processamento necessário (conversão de tipos, encoding de variáveis categóricas etc.).
- Aqui foi importante garantir que os dados estivessem prontos para os modelos sem causar vazamento de dados.

### Questão 6 – Decision Tree e Random Forest
- Treinei os dois modelos usando validação cruzada com 5 folds.
- Avaliei utilizando F1-score.
- Comparei os resultados para ver qual teve melhor desempenho.

### Questão 7 – SVM com kernel RBF
- Treinei um SVM com kernel RBF.
- Usei validação cruzada com F1-score.
- Comparei o desempenho com os modelos anteriores.

### Questão 8 – Ajuste de Hiperparâmetros no SVM
- Testei diferentes valores de C e gamma.
- Observei como esses parâmetros afetam a complexidade do modelo.
- Visualizei as fronteiras de decisão em dois cenários diferentes.

### Questão 9 – Boosting: CatBoost, LightGBM e XGBoost
- Treinei os três métodos de boosting com validação cruzada.
- Avaliei todos com F1-score.
- Comparei entre eles e com os modelos anteriores.

### Questão 10 – Interpretabilidade com SHAP
- Escolhi um dos modelos de Boosting e usei SHAP para entender o comportamento global e local.
- Listei as 3 variáveis mais importantes para o modelo.
- Escolhi uma instância com Revenue = 1 e expliquei a predição com SHAP.
- Comparei as explicações globais e locais.

### Questão 11 – SHAP vs. LIME
- Calculei a importância das variáveis com SHAP e LIME.
- Usei 3 instâncias diferentes para comparar os rankings.
- Comentei as diferenças e semelhanças entre os dois métodos.

### Questão 12 – Curva de aprendizado e análise final
- Avaliei o efeito do número de árvores (n_estimators) na performance de um modelo de Boosting.
- Verifiquei se havia sinais de overfitting.
- Comparei o modelo final com KNN (k=5) e Regressão Logística.
- Indiquei qual modelo entregaria como solução final e justifiquei a escolha.

## Tecnologias usadas

- Python
- Scikit-learn
- Pandas e NumPy
- Matplotlib e Seaborn
- XGBoost, LightGBM e CatBoost
- SHAP e LIME

## Dataset

- Online Shoppers Purchasing Intention: https://archive.ics.uci.edu/ml/datasets/Online+Shoppers+Purchasing+Intention+Dataset

---

Projeto feito como parte dos estudos de machine learning, com foco em experimentação, comparação entre modelos e análise interpretável.
