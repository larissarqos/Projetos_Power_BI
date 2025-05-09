<h1 align="center"> 📊 Business Case - Assinaturas de Streaming</h1>

<p align="center">
  <img src="https://github.com/user-attachments/assets/aeb43c96-67f1-4208-b867-1bf1a376b9de" alt="analise_vendas" width="1100"/>
</p>

## 📃 Contexto
Analisaremos a taxa de churn de diferentes serviços de streaming (dados fictícios): Amazon, Disney, Globoplay, HBO, Netflix e Telecine. Aplicaremos a Análise de Cohort para entender essas taxas considerando os fatores: campanha (promocional, reativação ou recorrente) e tipo de assinatura (mensal ou anual). 

***

<br>

## 🛠️ Ferramentas e Métodos Utilizados
- Power BI (DAX, Power Query, gráficos)
- Integração com Excel
- Business Intelligence
  
***

<br>
## 🎯 Objetivos
O objetivo da análise é identificar as taxas de churn e retenção dos serviços de assinatura considerando os fatores campanha e tipo de assinatura. Através da análise, vamos identificar os principais influenciadores da taxa de churn e o que pode ser feito para aumentar nossa taxa de retenção. Começaremos com uma análise exploratória dos dados e então responderemos a uma série de perguntas de negócio.

***

<br>

##  🧱 Estrutura do Projeto
### 🗄 Banco de dados
Abaixo o dicionário dos dados:

| Coluna | Descrição |
|--------|-----------|
| signature_id | ID da assinatura |
| product | Nome do produto |
| signature | Tipo de assinatura (annual, monthly) |
| campaign | Tipo de campanha (promotional, reactivation, recurring)|
| signup_date_time | Data de assinatura |
| cancel_date_time | Data de cancelamento |

***

<br>

### 🔎 Análise Exploratória

#### 📌 1. Qual o período avaliado?**  
As datas de assinatura de fevereiro de 2022 a abril de 2023

--

#### 📌 2. Qual o total de assinaturas?**  
Há um total de 69.993 assinaturas

-- 

#### 📌 3. Qual o total de assinaturas ativas e canceladas?**  
Do total, 43.203 assinaturas estão ativas (61,72%) e 26.790 estão canceladas (38,28%)

***

<br>

### 📍 Respondendo às perguntas de negócio

#### 📌 1. Que produto é o mais assinado?**  
HBO (17.508 assinaturas), Netflix (15.405 assinaturas) e Amazon (14.337 assinatuas) lideram o TOP 3, respondendo a quase 70% do total de assinaturas.

--
   
#### 📌 2. Quais as taxas de retenção e churn, por produto?**  
Conforme tabela abaixo, podemos notar que não há grande variação nas taxas de retenção e churn, de acordo com o produto. Todos apresentam taxas similares.

| Produto   | Total Assinaturas | Taxa de Retenção | Taxa de Churn |
|-----------|-------------------|------------------|---------------|
| Amazon    | 14.337 | 61,44% | 38,56% |
| Disney    | 8.095  | 61,33% | 38,67% |
| Globoplay | 8.551  | 61,90% | 38,10% |
| HBO       | 17.508 | 62,09% | 37,91% |
| Netflix   | 15.405 | 61,46% | 38,54% |
| Telecine  | 6.097  | 62,29% | 37,71% | 

--

#### 📌 3. Quais as taxas de churn e retenção, por campanha?**  
Comparando o total de assinaturas das campanhas Promocional e Reativação, cuja quantidade de assinaturas é similar, nota-se o quão alta é a taxa de churn da campanha promocional (73,01%), quase o dobro de Reativação.

| Campanha  | Total Assinaturas | Taxa de Retenção | Taxa de Churn |
|-----------|-------------------|------------------|---------------|
| Promocional | 19.093 | 26,99% | 73,01% |
| Reativação  | 21.133 | 60,67% | 39,33% |
| Recorrente  | 29.767 | 84,80% | 15,25% |

--

#### 📌 4. Que tipo assinatura teve menor taxa de churn: anual ou mensal?**  
As assinaturas anuais, mesmo em maior número (aprox. 7 mil assinaturas a mais) que as mensais, possuem menor taxa de cancelamento (32,44%), enquanto as assinaturas por mês contam churn de 45,44%.

| Tipo Assinatura  | Total Assinaturas | Taxa de Retenção | Taxa de Churn |
|------------------|-------------------|------------------|---------------|
| Anual   | 38.576 | 67,56% | 32,44% |
| Mensal  | 31.417 | 54,56% | 45,44% |

--

#### 📌 5. Que períodos do ano contaram com maior taxa de churn?**  
As assinaturas dos meses de julho/2022 e janeiro/2023, de forma geral, contaram com uma maior taxa de cancelamentos.

--

#### 📌 6. Indique o produto, campanha, e tipo de assinatura com os melhores resultados**
   
* **Produto:** Os produtos contaram com um desempenho similar em quesitos de churn e retenção. Se avaliarmos por total de assinaturas, HBO, Netflix e Amazon tiveram melhor desempenho
* **Campanha:** As camapanhas de reativação tiveram menor taxa de churn, 15,25%
* **Tipo de Assinatura:** As assinaturas anuais contaram com menor taxa de cancelamento, 32,44%

***

<br>

### 📈 Recomendações Estratégicas
De maneira geral, a taxa de churn dos serviços é altíssima, quase 40%. O foco das recomendações será a redução dos cancelamentos . 
**Cenário ideal:** Mais próxima de 0 possível, 5% é um valor aceitável.

#### 🟦 Incentivar as assinaturas cujas campanha e período contaram com maior retenção
-**Aumento das assinaturas do tipo anual e recorrente:**  Um programa de membros pode ajudar a unir essas duas opções, ofertando vantagens e conteúdos exclusivos para os clientes optarem por esse serviço.

#### 🟦 Aumentar a fidelização
- **Melhorar ou criar campanhas de fidelização:**
  Lançar descontos e promoções periódicos;
  Oferecer upgrades com benefícios exclusivos;
  Incentivar a assinatura de pacotes família / assinatura compartilhada;
  Personalizar recomendações de acordo com o perfil do cliente;
  Criar programas de indicação concedendo descontos / mensalidade grátis para cada indicação bem sucedida.
  
#### 🟦 Melhorar o atendimento ao cliente
- **Melhorar os canais de atendimento** No geral, aumentar o contato com o cliente, melhorar o atendimento e estar atento às preferências de acordo com seu perfil, são ações que podem melhorar a confiança e fidelidade desses clientes, aumentanddo nossa retenção.

#### 🟦 Otimizar a campanha Promocional
- **Identificar erros e acertos da campanha Promocional:** A campanha promocional contou com alta conversão (quase 1/3 dos clientes vieram através dela), mas baixíssima retenção (churn de mais de 70%). Algumas perguntas podem levar a melhor clareza e posterior otimização dessa campanha, que contou com alta captação:

  O público alvo da campanha tinha real interesse no que foi ofertado?

  Houveram muitas reclamações dos que vieram por essa campanha?

  Que programas de fidelização foram aplicados nos clientes que vieram através dessa campanha?

***

<br>

*Este projeto foi desenvolvido como parte do meu portfólio em análise de dados. Sinta-se à vontade para explorar os dados, sugerir melhorias ou entrar em contato!*
