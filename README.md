# Detecção de Anomalias em Transações em Python (ML)

Detecção de Fraudes em Cartões de Crédito com Machine Learning
Este projeto visa desenvolver um modelo de inteligência artificial capaz de identificar transações fraudulentas em cartões de crédito. O foco principal é lidar com o desafio de dados extremamente desbalanceados, onde o número de fraudes é muito inferior ao de transações legítimas.

## 1. Visão Geral do Projeto
Transações fraudulentas representam uma pequena fração de todas as transações, mas geram prejuízos bilionários. Este notebook explora desde o pré-processamento de dados até a explicabilidade do modelo, utilizando algoritmos como Regressão Logística, Random Forest e XGBoost.

## 2. Estrutura do Projeto
O fluxo de trabalho foi dividido nas seguintes etapas:

Análise Exploratória e Pré-processamento: Carregamento dos dados e normalização da variável Amount (valor da transação).

Tratamento de Dados Desbalanceados: Aplicação de técnicas de Undersampling e Oversampling (SMOTE).

Modelagem: * Regressão Logística (Baseline)

Random Forest Classifier

XGBoost Classifier

Avaliação: Uso de métricas apropriadas para fraude, como Precision-Recall Curve, AUC-ROC e F1-Score.

Otimização: Ajuste de hiperparâmetros via GridSearchCV.

Explicabilidade: Uso da biblioteca SHAP para entender quais variáveis (features) mais influenciam a decisão do modelo.

## 3. Tecnologias Utilizadas
Linguagem: Python 3.12

Bibliotecas de Manipulação e Visualização: Pandas, Numpy, Matplotlib, Seaborn.

Machine Learning: Scikit-learn, XGBoost.

Balanceamento de Dados: Imbalanced-learn (SMOTE).

Explicabilidade: SHAP.

## 4. Principais Resultados
O modelo final demonstrou alta capacidade de identificação de fraudes, com destaque para:

Recall: Melhorado através do balanceamento, garantindo que menos fraudes passem despercebidas.

Curva Precision-Recall: Utilizada como métrica principal devido ao desbalanceamento severo da classe positiva.

Importância de Variáveis: Identificação das componentes principais (V1, V2, ... V28) que possuem maior peso na detecção de anomalias.

## 5. Conclusão
A detecção de fraudes exige um equilíbrio delicado entre identificar o máximo de crimes possíveis (Recall) sem bloquear muitos clientes legítimos (Precision). O uso de XGBoost combinado com técnicas de oversampling e análise de SHAP values provou ser uma abordagem robusta para este problema financeiro.
