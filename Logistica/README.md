<h1 align="center">Business Case - Dashboard de Logística</h1>

## Contexto
A área de logística de uma empresa automotiva fictícia busca otimizar a eficiência operacional e melhorar a satisfação dos clientes através de uma gestão mais precisa das suas operações de transporte. O time realiza reuniões mensais com as transportadoras contratadas e precisa de uma visão detalhada das operações, que permita a análise de rotas, desempenho de transporte e otimização de recursos.

## Objetivos
O objetivo da análise é identificar possíveis problemas de desempenho no setor e sugerir soluções aplicáveis para estes. Para isso, nossa análise buscará responder às seguinte perguntas:
Nossas entregas têm sido realizadas dentro do prazo?
O valor do frete tem apresentado grande variação? 
Qual o desempenho dos nossos tipos de veículo?
Como está a eficiência do transporte?


## Estrutura do Projeto
### 1. Banco de dados
Abaixo o dicionário dos dados:

| Coluna | Descrição |
|--------|-----------|
| Load                    | Código da carga |
| Transportadora          | Nome da transportadora responsável |
| Origem-Cidade           | Cidade de origem |
| Origem-UF               | Estado de origem |
| Destino                 | Cidade e Estado de destino |
| Peso Bruto (kg)         | Peso bruto da carga em kg |
| Cubagem (m³)            | Cubagem da carga, em m³ |
| Data de Coleta          | Data da coleta do produto |
| Data de Entrega         | Data de entrega do produto |
| Prazo Realizado (dias)  | Diferença entre a data de entrega e a data de coleta, em dias |
| Prazo Contratado (dias) | Prazo contratado para realização da entrega, em dias |

<br>

### 2. Análise Exploratória

**1. Qual o período avaliado?**  
As datas de assinatura de fevereiro de 2022 a abril de 2023

**2. Qual o total de assinaturas?**  
Há um total de 69.993 assinaturas

**3. Qual o total de assinaturas ativas e canceladas?**  
Do total, 43.203 assinaturas estão ativas (61,72%) e 26.790 estão canceladas (38,28%)

<br>

### 3. Respondendo às perguntas de negócio

**1. Que produto é o mais assinado?**  
HBO (17.508 assinaturas), Netflix (15.405 assinaturas) e Amazon (14.337 assinatuas) lideram o TOP 3, respondendo a quase 70% do total de assinaturas.
   
**2. Quais as taxas de retenção e churn, por produto?**  
Conforme tabela abaixo, podemos notar que não há grande variação nas taxas de retenção e churn, de acordo com o produto. Todos apresentam taxas similares.

| Produto   | Total Assinaturas | Taxa de Retenção | Taxa de Churn |
|-----------|-------------------|------------------|---------------|
| Amazon    | 14.337 | 61,44% | 38,56% |
| Disney    | 8.095  | 61,33% | 38,67% |
| Globoplay | 8.551  | 61,90% | 38,10% |
| HBO       | 17.508 | 62,09% | 37,91% |
| Netflix   | 15.405 | 61,46% | 38,54% |
| Telecine  | 6.097  | 62,29% | 37,71% | 

**3. Quais as taxas de churn e retenção, por campanha?**  
Comparando o total de assinaturas das campanhas Promocional e Reativação, cuja quantidade de assinaturas é similar, nota-se o quão alta é a taxa de churn da campanha promocional (73,01%), quase o dobro de Reativação.

| Campanha  | Total Assinaturas | Taxa de Retenção | Taxa de Churn |
|-----------|-------------------|------------------|---------------|
| Promocional | 19.093 | 26,99% | 73,01% |
| Reativação  | 21.133 | 60,67% | 39,33% |
| Recorrente  | 29.767 | 84,80% | 15,25% |

**4. Que tipo assinatura teve menor taxa de churn: anual ou mensal?**  
As assinaturas anuais, mesmo em maior número (aprox. 7 mil assinaturas a mais) que as mensais, possuem menor taxa de cancelamento (32,44%), enquanto as assinaturas por mês contam churn de 45,44%.

| Tipo Assinatura  | Total Assinaturas | Taxa de Retenção | Taxa de Churn |
|------------------|-------------------|------------------|---------------|
| Anual   | 38.576 | 67,56% | 32,44% |
| Mensal  | 31.417 | 54,56% | 45,44% |

**5. Que períodos do ano contaram com maior taxa de churn?**  
As assinaturas dos meses de julho/2022 e janeiro/2023, de forma geral, contaram com uma maior taxa de cancelamentos.

**6. Indique o produto, campanha, e tipo de assinatura com os melhores resultados**
   
* **Produto:** Os produtos contaram com um desempenho similar em quesitos de churn e retenção. Se avaliarmos por total de assinaturas, HBO, Netflix e Amazon tiveram melhor desempenho
* **Campanha:** As camapanhas de reativação tiveram menor taxa de churn, 15,25%
* **Tipo de Assinatura:** As assinaturas anuais contaram com menor taxa de cancelamento, 32,44%

<br>

### 4. Sugestões
De maneira geral, a taxa de churn dos serviços é altíssima, quase 40%. O ideal é que esteja mais próxima de 0 possível, sendo 5% um valor aceitável. Se temos 40% como taxa de churn, estamos 8x acima do cenário ideal e isso é preocupante. O foco das sugestões será a redução dos cancelamentos, segue alguns pontos que podemos considerar para melhorar nossa retenção:

* **Primeiro, foco:** Devemos focar em assinaturas do tipo anual e campanhas do tipo Recorrente. Um programa de membros pode ajudar a unir essas duas opções, ofertando produtos diferenciados e exclusivos para os clientes que optarem por essa opção. No geral, aumentar o contato com o cliente, melhorar o atendimento e estar atento às preferências de acordo com seu perfil, são ações que podem melhorar a confiança e fidelidade desses clientes, aumentanddo nossa retenção.

* **Programas de Fidelização:** Com uma taxa de churn de quase 40%, devemos desenvolver programas de fidelização para nossos clientes. Oferecer descontos e ofertas em meses comemorativos (vai criar no cliente a expectativa de receber uma nova promoção nas próximas datas comemorativas); incentivar a assinatura para pacotes família ou assinatura compartilhada (aumentando a fidelização do cliente) e inserir também programas de recomendação, concedendo descontos ou mensalidade grátis para cada indicação bem sucedida, são medidas que podem fazer nossos clientes ficarem mais tempo.

* **Avaliar a campanha Promocional:**  Quase 1/3 dos clientes vieram através da campanha promocional e mais de 70% deles cancelaram. Devemos analisar que programas de fidelização foram aplicadas para manter esses clientes e, se foram aplicadas, qual o motivo de seu fracasso. A retenção foi baixíssima para essa campanha, apesar da alta captação de clientes. Devemos nos perguntar: o público alvo da campanha tinha real interesse no que foi ofertado? Houveram muitas reclamações dos que vieram por essa campanha? O que foi feito para manter esse clientes? Essas perguntas podem nos guiar a otimizar uma próxima campanha promocional (que teve boa captação) e aumentar a retenção de clientes através dela.
