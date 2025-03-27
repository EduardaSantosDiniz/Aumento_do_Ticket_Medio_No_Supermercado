# Como aumentr o ticket médio de um supermercado de acordo com os dados?
# 1️⃣Definição do Problema
Esse projeto é baseado em um supermercado varejista, o próposito inicial é descobrir como aumentar o ticket médio de um supermercado mas também responder 7 perguntas que nos foi proposto.
  
As perguntas foram:     
  
-Qual o perfil de cliente que mais compra determinado produto?

-Qual é a cada categoria que mais vende produtos?
 
-Qual é a sazonalidade das vendas? (Produtos que vendem mais em determinadas épocas do ano)

-Quais produtos têm maior margem de lucro?

-Qual o perfil dos clientes (por exemplo, idade, sexo, localização) que mais compram?NAO RESPODIDO

-Quais clientes compram produtos de maior valor?

-Qual é a frequência de compras dos clientes?


**Nesse momento temos que verificar as 7 perguntas usando a ordem ao nosso favor, como a resposta de uma pergunta depende da outra, é importante saber por onde começar.**

# 2️⃣Limpeza e Preparação dos Dados

Como estava a base de dados:

![{82087AEB-DFFA-476A-BD04-EE4F512E067B}](https://github.com/user-attachments/assets/8f4bbc0a-8ae2-4aee-9fa7-ff023eca602a)

Depois da limpeza e preparação:


![{BB24346E-0689-4D25-9883-5D395D344633}](https://github.com/user-attachments/assets/5e8bdce6-f553-4176-b51a-bbf65f1b6e55)


Retirei informações que não respondiam nenhuma pergunta nem o problema principal e traduzi toda a base de dados

(muitas pessoas não entendem o motivo e acabam descartando uma simples limpeza e preparação porém isso ajuda muito na hora de entender os dados)
# 3️⃣Análise Exploratória de Dados (EDA)

Nesse momento nós entramos de cabeça no negócio (independente do que seja), aqui entendemos cada ponto e oque cada dado está falando.

**Vamos responder nossa primeira pergunta: Qual é a cada categoria que mais vende produtos?**

Usando python, eu pedi pra ele contar quantas vezes cada categoria aparece, somar por categoria e fazer um gráfico. 

Simples assim...

![{78FEA79C-4314-4BBA-A4DF-559D48886843}](https://github.com/user-attachments/assets/0c6e1890-b5c7-4e7d-ad4f-54f4197650eb)



Olhando o resultado aparentemente é o Acessórios de moda, porém como a nossa base de dados divide por cliente, provavelmente este dado está errado devido a possibilidade de um cliente comprar 10 produtos de uma mesma categoria e ter o mesmo peso de um cliente que comprou apenas um.

**Para respondermos a resposta de forma correta, temos que somar a quantidade vendida por categoria.**

![{71528EDA-6EAE-49E4-836B-E5A3424BFBB8}](https://github.com/user-attachments/assets/17fd66a0-bd09-41b1-811a-538cb18f4235)


É um erro bobo que podemos cometer se pularmos a etapa de entender a base de dados, como os dados se comunicam, como eles funcionam...


**Segunda pergunta: Qual o perfil dos clientes (por exemplo, tipo, sexo, localização) que mais compram?**


Para responder essa pergunta temos que agrupar as diferentes combinações que existem dos clientes, e logo depois disso verificar qual compram mais em valor total de compra.


![{5DAD0510-4FF2-4711-9305-97D664F0E31F}](https://github.com/user-attachments/assets/695e3681-59d3-4687-8b72-cf523c6f2859)















 Base de dados foi retirada do site Kaggle, link: https://www.kaggle.com/datasets/hosammhmdali/supermarket-sales

      
  
 

 

