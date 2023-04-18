# sales_prediction
Este projeto estuda a empresa fictícia Rossmann, que demanda do seu time de dados uma previsão das vendas de suas lojas para as próximas 6 semanas.

* **1** Limpezas e adaptações básicas nos dados;
* **2** São realizados ajustes para uma melhor exploração e utilização dos dados; 
* **3** Filtragem de variáveis indesejadas;
* **4** É realizado o Rescaling, para diminuir o viés dos modelos sobre as variáveis de maior abrangência; Encoding para transformar as variáveis categóricas em numéricas, compatibilizando assim o dataset com os algoritmos; e transformação das variáveis, particularmente os dias e meses, para que o algoritmo os entenda como fenômenos cíclicos;
* **5** São selecionadas as variáveis que possuem maior correlação com a variável resposta utilizando o algoritmo Boruta. No projeto está incluido apenas o resultado da aplicação desse algoritmo;
* **6** Seleciona-se o algoritmo xgboost para produzir o modelo final que irá para produção. O modelo é então refinado para maior precisão. Para não ocupar muita memória no bot do telegram, o n_estimators do modelo em produção foi reduzido para 500, apenas a título de demonstração. Porém, o modelo mais otimizado possui n_estimators=2500;
* **7** É realizada a interpretação do erro do modelo, para verificar sua usabilidade;
* **8** Por fim, é feito o deploy do modelo para produção.

## Consulta dos resultados de forma automatizada:

Para facilitar a consulta das previsões para todos os stakeholders, foi criado um bot no telegram, como produto final deste projeto.
É só testar! Entre no link abaixo e digite um número de 100 a 999 (cada número corresponde ao código de uma das lojas) e aguarde um minuto, logo o bot responderá a previsão de vendas da respectiva loja. Caso a loja que você requisitar não exista, o bot também avisará!

https://t.me/rossmann1848_bot