# Client credit analysis
Este projeto tem por objetivo verificar se um determinado cliente está apto a receber um empréstimo utilizando o algoritmo de classificação SVM. As principais etapas deste trabalho foram:

* **1 - Limpeza dos dados:** Os dados são carregados e verificados nesta etapa, que neste projeto precisou renomear as colunas, excluir valores não existentes e erros na base de dados original, como outliers de clientes com 144 anos de idade, por exemplo;
* **2 - Feature Engineering:** Posteriormente os dados são agrupados para facilitar a análise, além da criação de novas colunas que permitem verificar a relação entre variáveis;
* **3 - Análise exploratória:** Nessa etapa é realizada a análise da base de dados, com a análise univariada, bivariada e multivariada, onde são encontrados vários insights;
* **4 - Filtragem das variáveis:** A filtragem é feita de forma que consiga-se separar as colunas que são inúteis, das numéricas e das categóricas, para seguir para a próxima etapa;
* **5 - Pré-processamento dos dados:** Nesta etapa os dados são divididos em treino e teste e são feitos alguns ajustes na base. O encoding é realizado nas variáveis categóricas através do método Ordinal Encoding e Label Encoding. Quanto à escala dos dados numéricos, após testar o modelo algumas vezes, decidi por usar o StandardScaler pois aumentava a velocidade do modelo, sendo que o modelo sem qualquer ajuste demora 78 minutos para concluir e o ajustado apenas 9 minutos;
* **6 - Treinamento do modelo:** Nesta etapa o modelo é treinado. Para esse projeto foi optado por usar-se o SVM;
* **7 - Avaliação do modelo:** Por fim, o modelo é avaliado nos dados de treino e de teste. Neste projeto, o accuracy score dos dados de treino foi aproximadamente 0,831 e o de teste foi de aproximadamente 0,835, o que aponta que o modelo está bem ajustado e não sofre de overfitting.
