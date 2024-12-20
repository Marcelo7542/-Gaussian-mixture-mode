English Description Below


Detecção de Anomalias e Modelos de Mistura Gaussiana

Descrição do Projeto

Neste repositório, desenvolvi duas análises principais relacionadas à detecção de anomalias e modelagem de dados utilizando modelos baseados em distribuições gaussianas.

O trabalho inclui uma exploração detalhada de Gaussian Mixture Models (GMM), abordagens robustas para remoção de anomalias, 
e a aplicação de métodos para identificar padrões em datasets tanto sintéticos quanto reais.

Os dois arquivos principais são:

Anomaly Detection

Gaussian Mixture Model

Anomaly Detection:

Neste arquivo, concentrei meus esforços em detecção de anomalias em dados bidimensionais, aplicando técnicas que incluem:

Modelos de Mistura Gaussiana (GMM):

Treinei modelos GMM para identificar clusters nos dados e determinar anomalias com base na densidade dos pontos.

Pontos com densidade abaixo de um limiar percentil foram marcados como anomalias.

Remoção de Anomalias Manual:

Após identificar os outliers, limpei os dados e treinei novamente o GMM para observar o impacto na modelagem.

Elliptic Envelope:

Explorei um método robusto para detecção de outliers baseado em distribuições elípticas, removendo outliers de forma automática.

Bayesian Gaussian Mixture:

Apliquei um modelo Bayesiano para determinar automaticamente o número ideal de componentes gaussianos nos dados.

Visualizações em gráficos 2D demonstram as fronteiras dos clusters, os pesos das componentes gaussianas e os outliers detectados.


Gaussian Mixture Model (GMM)

O Gaussian Mixture Model (GMM) é um modelo probabilístico que assume que os dados são provenientes de uma mistura de várias distribuições gaussianas. 

Ele é amplamente utilizado para tarefas como clustering e detecção de anomalias, pois permite a modelagem de dados com diferentes formas e distribuições.

Criação de Dados Sintéticos

Utilizei o make_blobs para gerar dados sintéticos com três centros de clusters e adicionei ruído aos dados.

Treinamento do Modelo GMM

Ajustei o modelo GMM com o GaussianMixture do Scikit-learn, utilizando os dados gerados.

Visualização dos Clusters e Fronteiras de Decisão

Visualizei as fronteiras de decisão e os centroides dos clusters identificados, além de plotar as previsões de associação de cada ponto aos clusters.

Análise dos Parâmetros do Modelo

Exibi os pesos das componentes, as médias e covariâncias das distribuições gaussianas, e verifiquei a convergência do modelo.

Detecção de Anomalias

Identifiquei os outliers com base na densidade de probabilidade dos pontos.

Avaliação do Modelo

Comparei diferentes tipos de covariância (full, tied, diag, spherical) para observar a influência na modelagem dos dados.

Visualizações

Criei gráficos 2D para mostrar as fronteiras de decisão, pesos e centros das distribuições gaussianas, além da detecção de outliers.





Anomaly Detection and Gaussian Mixture Models

Project Description

In this repository, I developed two main analyses related to anomaly detection and data modeling using models based on Gaussian distributions.

The work includes a detailed exploration of Gaussian Mixture Models (GMM), robust approaches for anomaly removal, 
and the application of methods to identify patterns in both synthetic and real datasets.

The two main files are:

Anomaly Detection

Gaussian Mixture Model

Anomaly Detection:

In this file, I focused on anomaly detection in two-dimensional data, applying techniques that include:

Gaussian Mixture Models (GMM):

I trained GMM models to identify clusters in the data and determine anomalies based on the density of points. 

Points with density below a percentile threshold were marked as anomalies.

Manual Anomaly Removal:


After identifying the outliers, I cleaned the data and retrained the GMM to observe the impact on the modeling.

Elliptic Envelope:

I explored a robust method for outlier detection based on elliptical distributions, automatically removing outliers.

Bayesian Gaussian Mixture:

I applied a Bayesian model to automatically determine the optimal number of Gaussian components in the data.

2D visualizations demonstrate the cluster boundaries, the weights of the Gaussian components, and the detected outliers.

Gaussian Mixture Model (GMM)

The Gaussian Mixture Model (GMM) is a probabilistic model that assumes the data comes from a mixture of several Gaussian distributions. 
It is widely used for tasks such as clustering and anomaly detection, as it allows for modeling data with different shapes and distributions.

Synthetic Data Creation:

I used make_blobs to generate synthetic data with three cluster centers and added noise to the data.

Training the GMM Model:

I adjusted the GMM model with the GaussianMixture from Scikit-learn using the generated data.

Cluster and Decision Boundaries Visualization:

I visualized the decision boundaries and the centroids of the identified clusters, in addition to plotting the association predictions of each point to the clusters.

Model Parameter Analysis:

I displayed the weights of the components, the means, and the covariances of the Gaussian distributions, and checked the model's convergence.

Anomaly Detection:

I identified the outliers based on the density of the points.

Model Evaluation:

I compared different types of covariance (full, tied, diag, spherical) to observe the impact on data modeling.

Visualizations:

I created 2D plots to show the decision boundaries, the weights, and centers of the Gaussian distributions, in addition to the outlier detection.

