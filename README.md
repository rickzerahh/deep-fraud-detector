## DeepFraude
Sistema de detecção de fraudes em transações financeiras utilizando modelos supervisionados e Autoencoder.

## Sobre o Projeto
Este projeto de TCC tem como objetivo comparar algoritmos de aprendizado de máquina tradicionais com técnicas de aprendizado profundo (Autoencoder) na detecção de fraudes em transações com cartão de crédito. O sistema foi desenvolvido com foco em dados altamente desbalanceados e simula uma aplicação real de segurança digital no setor financeiro.

### Tecnologias Utilizadas:

- Python 3.10
- Scikit-learn
- Imbalanced-learn (SMOTE)
- TensorFlow / Keras
- Pandas & NumPy
- Matplotlib & Seaborn
- Jupyter Notebook

### Modelos Avaliados

- Regressão Logística
- Naive Bayes
- Árvore de Decisão
- Autoencoder (não supervisionado)

### Métricas de Avaliação
O desempenho dos modelos foi medido por meio de:

- AUC (Área sob a Curva ROC)
- F1-score
- Precisão
- Recall

_A acurácia não foi utilizada como métrica principal devido à sua ineficácia em bases desbalanceadas._

### Estrutura do Projeto

``notebooks/`` – notebooks separados por modelo

``dados/`` – dataset (não incluído, mas com link de download)

``utils/`` – funções auxiliares e pipeline

``resultados/`` – gráficos, curvas ROC e matrizes de confusão

### Base de Dados
Utilizou-se o dataset de transações disponibilizado pela Worldline/Kaggle, contendo 284.807 registros com apenas 0,17% de fraudes.

[Link para o dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

### Conclusão
Modelos supervisionados obtiveram bom desempenho, mas o Autoencoder se destacou na detecção de anomalias mesmo sem rótulo, mostrando-se uma solução promissora para cenários com escassez de dados rotulados.
