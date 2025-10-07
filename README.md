Análise Preditiva de Energia e Estabilidade de Redes
📝 Descrição
Este projeto consiste em uma coleção de análises de machine learning focadas no setor de energia. Utilizando um Jupyter Notebook, foram explorados quatro datasets distintos para resolver problemas de regressão e classificação. Os objetivos variam desde a previsão de consumo de energia e potência gerada por fontes renováveis até a classificação da estabilidade de redes elétricas inteligentes e níveis de radiação solar.

📖 Índice
Análises Realizadas

Tecnologias Utilizadas

Como Executar o Projeto

Estrutura do Projeto

Resultados e Conclusões

Fontes dos Dados

🚀 Análises Realizadas
O notebook está dividido nas seguintes análises principais:

Predição de Consumo de Energia de Eletrodomésticos (Regressão):

Objetivo: Prever o consumo de energia de eletrodomésticos com base em dados ambientais (temperatura, umidade) de uma residência.

Modelos: Regressão Linear, Árvore de Regressão, Random Forest Regressor.

Métricas: R², Raiz do Erro Quadrático Médio (RMSE) e Erro Absoluto Médio (MAE).

Classificação da Estabilidade de Redes Inteligentes (Classificação):

Objetivo: Classificar a estabilidade de uma rede elétrica inteligente como 'estável' ou 'instável'.

Modelos: Árvore de Decisão, K-Nearest Neighbors (KNN), Regressão Logística.

Métricas: Acurácia, F1-Score e Matriz de Confusão.

Classificação de Níveis de Radiação Solar (Classificação):

Objetivo: Classificar os períodos do dia em 'Alta Radiação' ou 'Baixa Radiação' com base na mediana da radiação.

Modelos: Árvore de Decisão, Random Forest Classifier, Support Vector Machine (SVM).

Métricas: Acurácia e Matriz de Confusão.

Predição de Potência de Turbinas Eólicas (Regressão):

Objetivo: Prever a potência ativa (em kW) gerada por uma turbina eólica, com base na velocidade do vento, direção e potência teórica.

Modelos: Regressão Linear, Árvore de Regressão, Random Forest Regressor.

Métricas: R² e Raiz do Erro Quadrático Médio (RMSE).

🛠️ Tecnologias Utilizadas
As seguintes ferramentas e bibliotecas foram utilizadas neste projeto:

Python 3

Pandas: para manipulação e análise de dados.

NumPy: para operações numéricas.

Matplotlib e Seaborn: para visualização de dados.

Scikit-learn: para implementação dos modelos de machine learning, pré-processamento e avaliação.

Jupyter Notebook: como ambiente de desenvolvimento.

⚙️ Como Executar o Projeto
Para replicar as análises, siga os passos abaixo:

Clone este repositório:

Bash

git clone https://[URL-DO-SEU-REPOSITORIO].git
cd [NOME-DO-DIRETORIO]
Crie um ambiente virtual (recomendado):

Bash

python -m venv venv
source venv/bin/activate  # No Windows, use `venv\Scripts\activate`
Instale as dependências:
Crie um arquivo requirements.txt com o seguinte conteúdo:

Plaintext

pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter
E instale-o com o pip:

Bash

pip install -r requirements.txt
Faça o download dos datasets:
Certifique-se de que os seguintes arquivos CSV estejam na pasta /content/ (ou ajuste os caminhos no notebook):

energydata_complete.csv

smart_grid_stability_augmented.csv

SolarPrediction.csv

Wind_Turbine_Scada_Dataset.csv

Inicie o Jupyter Notebook:

Bash

jupyter notebook
Abra o arquivo CP2_SEM2SERS.ipynb e execute as células.

📂 Estrutura do Projeto
O projeto está contido em um único Jupyter Notebook (CP2_SEM2SERS.ipynb), que é dividido em seções claras para cada uma das quatro análises.

Cada seção segue uma estrutura semelhante:

Carregamento e Pré-processamento dos Dados: Leitura do arquivo CSV e preparação inicial dos dados.

Divisão dos Dados: Separação em conjuntos de treino e teste.

Treinamento e Avaliação: Instanciação, treinamento e avaliação de múltiplos modelos de machine learning.

Comparação e Conclusão: Análise comparativa dos resultados para determinar o melhor modelo para o problema.

📊 Resultados e Conclusões
1. Predição de Consumo de Energia
O modelo Random Forest Regressor apresentou o melhor desempenho, com o maior R² e o menor RMSE.

Conclusão: Relações não-lineares entre as variáveis ambientais e o consumo de energia são mais bem capturadas por modelos baseados em árvores de decisão.

2. Estabilidade de Redes Inteligentes
O modelo Árvore de Decisão foi o mais confiável para detectar instabilidade.

Conclusão: O critério de escolha foi o menor número de Falsos Negativos, crucial para evitar falhas na detecção de instabilidade da rede.

3. Classificação de Radiação Solar
O Random Forest Classifier alcançou a maior acurácia.

Conclusão: Tanto o Random Forest quanto o SVM mostraram excelente desempenho, com poucas classificações incorretas, sendo adequados para a tarefa.

4. Predição de Potência Eólica
O Random Forest Regressor novamente se destacou, com o maior R² e o menor RMSE.

Conclusão: A capacidade do modelo de lidar com interações complexas entre as variáveis (velocidade do vento, direção) o torna ideal para prever a geração de energia eólica.

💾 Fontes dos Dados
Consumo de Energia: Appliances energy prediction Data Set

Estabilidade da Rede: Smart Grid Stability Augmented

Radiação Solar: Solar Power Generation Data

Geração Eólica: Wind Turbine Scada Dataset
