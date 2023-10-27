# Clusterizacao_Kmeans_Wine
Agrupando em cluster tipos de vinhos, através da classificação das suas features.

## Descrição Projeto


**Conjunto de dados:** Base de dados com características de vinhos diversos .


**Arquivo:** dataset da iblioteca Sklearn


**Objetivo:** Aplicar machine learning com um modelo de clusterização e, analisar clusters obtidos, assim como métricas apresentadas pelo modelo.
Clusterização: A clusterização é uma técnica de análise de dados que tem como objetivo agrupar dados em conjuntos distintos com base em suas características. Podendo ser usada para identificar padrões em grandes conjuntos de dados, o que pode ser útil em áreas como marketing e estudos de mercado. É uma tarefa de aprendizado não supervisionado, o que significa que a classificação das informações é feita de forma automatizada, sem necessitar de etapas de treino e testes.

**IDE:** Colab


**Linguagem:** Python


**Principais bibliotecas utilizadas:**

• Pandas, para manipulação e tratamento dos dados; 

• Numpy, para realizar cálculos numéricos; 

• Sklearn, para aprendizado de machine learning;

• Matplotlib, para criação e visualização de gráficos;
• Seaborn, para criação e visualização de gráficos;
• Plotly, para criação e visualização de gráficos interativos.


**Modelo Utilizado:**

• K-Means, algoritmo iterativo que gera uma solução factível ao alocar um ponto ao cluster cujo “critério de agrupamento” é menor em relação ao centroide em questão.


**Métricas Aplicadas:**

• Silhouette Score:  avalia o desempenho do algoritmo de clustering, usando a distância intra-cluster média (a) e a distância média mais próxima do cluster (b) para cada amostra. O melhor valor é 1 e o pior valor é -1. Valores próximos de 0 indicam clusters sobrepostos. 


**Sequência de processos:**

1° Instalação bibliotecas;

2° Pré-processamento de conjuntos de dados;
Obs: Foi necessário colocar os dados na mesma escala (scale) e analisar valores outliers, filtrando os para que não impactassem negativamente na aplicação do algoritmo.

3° Aplicado teste com o algoritmo K-Means na base de dados para visualizar, quantos grupos (k) com características mais similares temos no dataset;
Obs: Nesse caso foi visto que podemos separar em 4 clusters.

4° Aplicar o método .fit do modelo de machine learning K-means, utilizando k=4;

5° Salvar centroides e labels sugeridos pelo modelo em variáveis;
*Centróides* são pontos que representam o centro de um cluster. Eles são calculados como a média aritmética de todos os pontos pertencentes ao cluster.

*Labels* são rótulos que indicam a qual cluster um objeto pertence, usados para identificar a qual grupo um objeto específico foi atribuído.

6° Criar DataFrame para visualizar centroides de cada grupo, com suas características;

7° Aplicar DataFrame criado em gráficos, para facilizar visualização e interpretação;

8° Aplicado métricas de silhouette, para verificar a qualidade do agrupamento alcançado.

**Resultado:** Foi possível visualizar os 4 clusters distintos dentro do dataset, porém, o resultado da métrica aplicada não foi muito boa, ficou em 24%, podendo ser melhorada.
