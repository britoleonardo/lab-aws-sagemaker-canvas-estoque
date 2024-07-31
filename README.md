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
    ![image](https://github.com/britoleonardo/lab-aws-sagemaker-canvas-estoque/blob/master/Dataset.png)
    
    #### Em _Select a column to predict_, selecionei a coluna ESTOQUE, a qual quero uma predição dos dados.
    
    ###### Para fins de validação e curácia dos dados utilizei a coluna PRECO, utilizando a forma de predição Standart que leva em média 2hs para maior tempoi de aprendizdo,
    segui com a análise através da média entre a os valores dos produtos obtidos no dataset.

    ![image](https://github.com/britoleonardo/lab-aws-sagemaker-canvas-estoque/blob/master/Dataset.png)

    #### Em Configure Model, foi selecionado a coluna ID_PRODUTOS para identificar os itens da coluna ESTOQUE. Enquanto a coluna DIA será o período em que ocorreu as váriações dos dados.
    Feito a previsão de até 1 dia, junto com a utilização de Feriados no Brasil.
    ![image](https://github.com/britoleonardo/lab-aws-sagemaker-canvas-estoque/blob/master/Dataset.png)

    #### No Data Visualizer conseguimos analisar os resultados obtidos de forma mais visual.
    ![image](https://github.com/britoleonardo/lab-aws-sagemaker-canvas-estoque/blob/master/Dataset.png)
    
### 3. CONCLUSÃO

   #### No Data Visualizer conseguimos analisar os resultados obtidos de forma mais visual.
  ![image](https://github.com/britoleonardo/lab-aws-sagemaker-canvas-estoque/blob/master/Dataset.png)


### Tecnologias utilizadas

[![ChatGPT](https://img.shields.io/badge/ChatGPT-74aa9c?style=for-the-badge&logo=openai&logoColor=white)](https://chat.openai.com/)
[![AWS](https://img.shields.io/badge/Amazon_AWS-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)](https://aws.amazon.com/pt/free/?)
