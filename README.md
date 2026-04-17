# 🛡️ Insurance Risk Classification - Naive Bayes
Este projeto implementa um modelo de Machine Learning para prever e classificar o nível de danos/acidentes (Accident) em apólices de seguros, utilizando uma base de dados com 20.000 registos e 27 atributos variados.

O objetivo é automatizar a triagem de perfis de clientes e prever a severidade de potenciais sinistros com base em dados demográficos, comportamento de condução e características do veículo.

## 📊 Sobre o Dataset
O conjunto de dados insurance.csv contém informações detalhadas, incluindo:

* Perfil do Condutor: Idade (Age), Estatuto Socioeconómico (SocioEcon), Aversão ao Risco (RiskAversion) e Histórico de Condução (DrivHist).

* Veículo: Ano (VehicleYear), Modelo (MakeModel), Quilometragem (Mileage) e itens de segurança como Airbags e Antilock.

* Variável Alvo (Accident): Classificada em quatro níveis: None, Mild, Moderate e Severe.

## 🛠️ Tecnologias e Ferramentas
``` Linguagem: Python.

Principais Bibliotecas:

Pandas & NumPy: Manipulação e limpeza de dados.

Scikit-learn: Implementação do modelo e métricas.

Yellowbrick: Visualização de performance (Confusion Matrix).
```
## ⚙️ Fluxo de Desenvolvimento
Exploração de Dados: Carregamento do dataframe e verificação de valores nulos (nenhum valor ausente encontrado).

Pré-processamento: * Remoção de colunas irrelevantes (Unnamed: 0).

Transformação de variáveis categóricas em numéricas utilizando LabelEncoder.

Treino do Modelo: Divisão dos dados em 70% para treino e 30% para teste, utilizando o algoritmo Gaussian Naive Bayes (GaussianNB).

Avaliação: Análise detalhada através de métricas de classificação.

## 📈 Resultados Obtidos
O modelo apresentou uma performance sólida, destacando-se na identificação de casos sem acidentes:

* Acurácia Geral: 86%.

* Precisão (Média Ponderada): 92%.

* Recall (Média Ponderada): 86%.

* F1-Score (Média Ponderada): 83%.

## Performance por Classe (Exemplos):
* Classe 'None': Precisão de 98% e Recall de 100%.

* Classe 'Moderate': Recall elevado de 91%.
