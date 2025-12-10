 # Como aumentar o ticket médio de um supermercado de acordo com os dados?        
# 1️⃣Definição do Problema         
Esse projeto é baseado em um supermercado varejista, o proprósito inicial é descobrir como aumentar o ticket médio de um supermercado mas também responder às 7 perguntas que nos foram propostas.  
                            
As perguntas foram:                                                              
   
    
                                                  
                                    
-Qual o perfil de cliente que mais compra determinado produto?                   
              
-Qual é a categoria que mais vende produtos?              
   
-Qual é a sazonalidade das vendas?    
        
-Quais produtos têm maior margem de lucro?   
 
-Qual o perfil dos clientes que mais compram?

-Quais clientes compram produtos de maior valor?
 
-Qual é a frequência de compras dos clientes? 


**Nesse momento temos que verificar as 7 perguntas usando a ordem ao nosso favor, como a resposta de uma pergunta depende da outra, é importante saber por onde começar.**

# 2️⃣Limpeza e Preparação dos Dados

Como estava a base de dados:
 
![{82087AEB-DFFA-476A-BD04-EE4F512E067B}](https://github.com/user-attachments/assets/8f4bbc0a-8ae2-4aee-9fa7-ff023eca602a)

Depois da limpeza e preparação:


![{BB24346E-0689-4D25-9883-5D395D344633}](https://github.com/user-attachments/assets/5e8bdce6-f553-4176-b51a-bbf65f1b6e55)


Retirei informações que não respondiam nenhuma pergunta nem o problema principal e traduzi toda a base de dados

(muitas pessoas não entendem a importância e acabam descartando uma simples limpeza e preparação, porém isso ajuda muito)
# 3️⃣Análise Exploratória de Dados (EDA)

Nesse momento nós entramos de cabeça no negócio (independente do que seja), aqui entendemos cada ponto e o que cada dado está dizendo

**Vamos responder nossa primeira pergunta: Qual é a cada categoria que mais vende produtos?**

Usando python, eu pedi pra ele contar quantas vezes cada categoria aparece, somar por categoria e fazer um gráfico. 

Simples assim.

![{78FEA79C-4314-4BBA-A4DF-559D48886843}](https://github.com/user-attachments/assets/0c6e1890-b5c7-4e7d-ad4f-54f4197650eb)



Olhando o resultado aparentemente são os Acessórios de Moda, porém como a nossa base de dados divide por cliente, provavelmente este dado está errado devido a possibilidade de um cliente comprar 10 produtos de uma mesma categoria e ter o mesmo peso de um cliente que comprou apenas um.

**Para respondermos a resposta de forma correta, temos que somar a quantidade vendida por categoria.** 

![{71528EDA-6EAE-49E4-836B-E5A3424BFBB8}](https://github.com/user-attachments/assets/17fd66a0-bd09-41b1-811a-538cb18f4235)


É um erro comum que podemos cometer se pularmos a etapa de entender a base de dados, como os dados se comunicam, como eles funcionam...


**Segunda pergunta: Qual o perfil dos clientes (por exemplo, tipo, sexo, localização) que mais compram?**


Para responder essa pergunta temos que agrupar as diferentes combinações que existem dos clientes, e logo depois disso verificar quais compram mais em valor total.


![{5DAD0510-4FF2-4711-9305-97D664F0E31F}](https://github.com/user-attachments/assets/695e3681-59d3-4687-8b72-cf523c6f2859)


**Terceira pergunta: Quais clientes compram produtos de maior valor?**
Para responder essa pergunta temos que verificar a média do valor dos produtos, que no caso é R$ 55,67 e verificar quais estão acima da média para depois verificar qual o perfil dos clientes que mais compram esses produtos.
![{0BE91E4B-A3ED-4A9F-90E1-017690A0A4B7}](https://github.com/user-attachments/assets/bbec97d3-f876-4da2-8c9a-1d9050d0aede)

**Quarta pergunta: Qual é a sazonalidade das vendas? (Produtos que vendem mais em determinadas épocas do ano)**
Para responder temos que separar por categoria e por mês, depois disso vamos verificar se tem categorias que vendem mais em determinados meses.
![{84AF68E7-91DF-4769-B9FC-984D5D8898FC}](https://github.com/user-attachments/assets/2766a4ce-4e06-4aa1-94e0-7fbd44c42e8c)

**Quinta pergunta: Quais produtos têm maior margem de lucro?**

Essa pergunta não tem como responder com a base de dados que foi fornecida, nesse caso a ideia seria marcar uma reunião com o responsável do estabelecimento e informá-lo que o percentual do lucro deve ser informado para cada categoria.

**Sexta pergunta: Qual o perfil de cliente que mais compra determinado produto?**
Para responder essa pergunta vamos agrupar os tipos de cliente por categorias de produtos

![{574620C3-5D4D-4051-B5DB-62FAE4FA97D2}](https://github.com/user-attachments/assets/c390f37a-6304-4459-bca5-c54471f28ffe)

**Sétima pergunta: Qual é a frequência de compras dos clientes?**
![{28216602-DB35-4BAF-B5A3-0F14399369E8}](https://github.com/user-attachments/assets/4701d72c-10ed-4e0f-a167-f9b3e328d1d7)

# 3️⃣ Análise dos Insight e Resolução do Problema
O principal desafio a ser solucionado é o aumento do ticket médio. Esse é um problema específico para cada cliente e envolve até mesmo aspectos científicos, pois exige a previsão dos comportamentos e decisões do consumidor. Ao antecipar esses passos, podemos influenciá-lo estrategicamente para aumentar seus gastos de forma natural e planejada.

# Como aumentar o ticket médio?

- Organizando estrategicamente a prateleira de acordo com a frequência que os produtos saem

- Promoção de combinações estratégicas

- Organizar a prateleira com produtos mais caros com uma pequena diferença de preço

entre outros.

### Organizando estrategicamente a prateleira de acordo com a frequência que os produtos saem
De acordo com o gráfico de frequência de compras, podemos observar que quatro categorias de produtos se destacam em janeiro. Uma sugestão seria colocá-las no mesmo corredor ou até mesmo na mesma prateleira.

Esses pequenos detalhes podem influenciar diretamente o comportamento de compra e contribuir para o aumento do ticket médio dos clientes.

O próximo passo seria realizar testes para verificar se essa estratégia realmente aumenta o ticket médio. Caso contrário, novas análises seriam feitas para buscar outras soluções.

### Promoção dessas combinações
Outro ponto a ser considerado é a promoção dessas combinações. Com a organização das prateleiras de acordo com a frequência de compras, seria importante analisar quais produtos dessas categorias têm maior saída. A partir disso, poderiam ser feitas promoções direcionadas para esses produtos, testando se o aumento nas vendas contribui para um aumento ainda maior no ticket médio.

### Organizar a prateleira com produtos mais caros com uma diferença de preço reduzida
Uma estratégia interessante seria aumentar o preço dos produtos de valor médio, de forma a reduzir a diferença entre esses e os produtos de maior valor. Ao fazer isso, os clientes perceberiam que a diferença de preço entre um produto de valor médio e um de maior qualidade e preço é pequena. Esse cenário pode levá-los a optar pelo produto de maior valor, já que a diferença financeira não é tão significativa. Dessa forma, o mercado aproveita para aumentar o ticket médio, incentivando os consumidores a escolherem opções de maior valor por um custo marginalmente maior.

# 4️⃣ Avaliação e Interpretação dos Resultados
Nessa etapa, as soluções previstas seriam analisadas para verificar se atingiram o resultado esperado pelo dono do mercado. Como se trata de um projeto de estudo e não de uma implementação prática, infelizmente não será possível seguir adiante. No entanto, o objetivo principal foi alcançado: a prática do pensamento crítico, bem como o desenvolvimento de habilidades na linguagem Python e suas bibliotecas. Esse exercício contribuiu significativamente para o aprendizado e aprimoramento de habilidades analíticas e técnicas.

### Percebe como é importante utilizar dados para embasar decisões?
Se gostou desse projeto que fiz, e gostaria de tirar uma dúvida ou algum conselho/feedback. Me mande mensagem em uma das minhas redes:

Email: eduardafaculdade0306@gmail.com

Linkedin: https://www.linkedin.com/in/eduarda-diniz-24a275272/




**Base de dados foi retirada do site Kaggle, link: https://www.kaggle.com/datasets/hosammhmdali/supermarket-sales**

      
  
 

 

