# Análise de Filmes - PProductions

****

## 🔍 Sobre o Projeto

O objetivo deste projeto é analisar o comportamento de filmes, tanto no que diz respeito a avaliação de clientes quanto no que diz respeito ao faturamento obtido.

O projeto foi desenvolvido em Jupyter Notebook. Todo o trabalho foi elaborado a partir de uma base de dados em csv com diversas informações de filmes lançados ao longo dos anos.

## 🗃️ Etapas do Projeto

Para o desenvolvimento do projeto foram importadas e utilizadas várias bibliotecas, como pandas, numpy, scikit-learn, matplotlib, seaborn e optuna.

Foi elaborada a fase de Preparação de Dados, em que foram tratados os Missing Values e valores duplicados.

Em seguida, variáveis foram transformadas para o prosseguimento das análises. Houve mudança de tipo de variável e remoção de palavras em colunas numéricas.

Após esses tratamentos, foi realizada a Análise Exploratória de Dados. Calculei o Índice de Correlação entre variáveis quantitativas e o nível de associação entre variáveis qualitativas e variáveis binárias, que foram criadas, utilizando o IV (Information Value). Com base nesses cálculos, realizei uma série de análises do comportamento das variáveis e dos relacionamentos entre elas.

Com a EDA finalizada, desenvolvi 6 modelos para avaliar qual teria o melhor poder de predição da nota IMDB.
Os 6 modelos desenvolvidos foram: Regressão Logística, Árvore de Decisão, Bagging de Regressão Logística, Random Forest, AdaBoost e Gradient Boosting.

Foram calculadas métricas de desempenho dos modelos. A principal medida utilizada para avaliação dos modelos foi o AUROC.
Os 2 modelos que apresentaram as melhores performances foram o AdaBoost e o Gradient Boosting.

Uma vez analisados todos os modelos, realizei a Tunagem dos Hiperparâmetros dos 2 melhores modelos avaliados.

Após a Tunagem, o modelo que apresentou a melhor performance foi o Gradient Boosting, apresentando um AUROC superior a 88% na base de teste e entregando uma boa capacidade de generalização.
