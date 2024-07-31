# 📊 Previsão de Estoque Inteligente na AWS com [SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)

## 🎯 Bootcamp Nexa - Machine Learning para Iniciantes na AWS - DIO.me)

## 📰 RESUMO

O projeto final do bootcamp é utilizar um dataset e utilizar o Sagemakers Canva para  PREVER o estoque inteligente baseando-se em Machine Learning.

![image](https://github.com/britoleonardo/lab-aws-sagemaker-canvas-estoque/blob/master/Imagem%203.png)

###### Este repositório foi realizado através de um bootcamp oferecido pelo DIO.me, o objetivo alcançado foi a utilização do Sagemakers Canva na AWS para criação de um modelo de estoque intelingente e análise dos Dados Obtidos, este projeto retrata uma forma de validação dos estudos oferecidos pela plataforma. 

## 🚀 Passo a Passo

### 1. DATASET

-   O Dataset foi gerado através do Chat-GPT, disponibilizado na pasta 'datasets', as instruções dadas foram:
    ![image](https://github.com/britoleonardo/lab-aws-sagemaker-canvas-estoque/blob/master/Dataset.png)

### 2. SAGEMAKER

-   Para o objetivo do projeto foi selecionado o Predective Analysis como meu Problem type, sendo ele direcionado a predizer o estoque com base no histórico do arquivo CSV.
    ![image](https://github.com/britoleonardo/lab-aws-sagemaker-canvas-estoque/blob/master/modelo%20de%20previs%C3%A3o.png)
    
    #### Em _Select a column to predict_, selecionei a coluna ESTOQUE, a qual quero uma predição dos dados.
    
    ###### Para fins de validação e Estresse da plataforma utilizei dados da coluna PRECO no primeiro upload, utilizando a forma de predição Standart que leva em média 2hs para maior tempo de aprendizdo, poréam na versão 1, a porcentagem de erro era significativa. Então refiz a Análise, retirando a coluna PRECO, segui com a análise através da mediana dos preços e com Quick build.

    ![image]([Imagem 6](https://github.com/britoleonardo/lab-aws-sagemaker-canvas-estoque/blob/master/Imagem%205.png))

    #### Em Configure Model, foi selecionado a coluna ID_PRODUTOS para identificar os itens da coluna ESTOQUE. Enquanto a coluna DIA será o período em que ocorreu as váriações dos dados.
    Feito a previsão de até 4 dias, junto com a utilização de Feriados no Brasil.
    ![image]([https://github.com/britoleonardo/lab-aws-sagemaker-canvas-estoque/blob/master/Dataset.png](https://github.com/britoleonardo/lab-aws-sagemaker-canvas-estoque/blob/master/Imagem%204.png))

    #### No Data Visualizer conseguimos analisar os resultados obtidos de forma mais visual.
    ![image]([https://github.com/britoleonardo/lab-aws-sagemaker-canvas-estoque/blob/master/Dataset.png](https://github.com/britoleonardo/lab-aws-sagemaker-canvas-estoque/blob/master/Imagem%208.png))

    #### Ao Analisar a variação da quantidade de produtos, bem como a Mediana dos preços durante o período avaliado, entende-se que há uma forte indicação de erro de alimentação no documento, o que pode levar a uma Análise infiel a realidade, como solicitado ao Chat-GPT, a coluna ESTOQUE deveria descrecer levemente, então o resultado da previsão individual dos produtos sempre levaria ao mesmo resultado, ou seja, um estoque zerado, como indicado abaixo pelos Produtos de ID 13 e 9.

    ![image]([[https://github.com/britoleonardo/lab-aws-sagemaker-canvas-estoque/blob/master/Dataset.png](https://github.com/britoleonardo/lab-aws-sagemaker-canvas-estoque/blob/master/Imagem%208.png)](https://github.com/britoleonardo/lab-aws-sagemaker-canvas-estoque/blob/master/Imagem%207%20estoque%20item%2013.png))
    ![image]([[https://github.com/britoleonardo/lab-aws-sagemaker-canvas-estoque/blob/master/Dataset.png](https://github.com/britoleonardo/lab-aws-sagemaker-canvas-estoque/blob/master/Imagem%208.png)](https://github.com/britoleonardo/lab-aws-sagemaker-canvas-estoque/blob/master/Imagem%207%20estoque%20item%209.png))
    
    
### 3. CONCLUSÃO

   #### Como ja feito alguns testes durante a realização do curso, houve um limite na predição em Batch, por isso a Análise foi individual.
  ![image]([https://github.com/britoleonardo/lab-aws-sagemaker-canvas-estoque/blob/master/Dataset.png](https://github.com/britoleonardo/lab-aws-sagemaker-canvas-estoque/blob/master/imagem%202.png))

  #### Porém, podemos chegar a algumas conclusões. Há um aumento significativo de erro quando o foi arquivo analisado, no ambiente teste isso é "Aceitável", porém na análise produtiva de uma empresa isso pode ser um fator determinante para a vida útil da empresa e empregabilidade dos funcionários, Caso isso ocorra em um ambiente real pode-se indicar manipulação dos dados ou má gestão por parte dos colaboradores, tornando a predição ineficaz e trazendo percas significaticas a empresa.

  #### Durante vários testes na plataforma podemos verificar uma projeção sigficativa dos resultados levando em conta os dados P10 e P90, que indicam a projeção em um ambiente favorável e em um ambiente desfavorável respectivamente, assim  conseguimos manipular os dados e a estratégia a ser tomada para prevenir riscos e diminuir gastos desnecessários colaborando com a boa gestão e saúde financeira da empresa.


### Tecnologias utilizadas

[![ChatGPT](https://img.shields.io/badge/ChatGPT-74aa9c?style=for-the-badge&logo=openai&logoColor=white)](https://chat.openai.com/)
[![AWS](https://img.shields.io/badge/Amazon_AWS-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)](https://aws.amazon.com/pt/free/?)
