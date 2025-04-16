<h1 align="center">Business Case - Dashboard de Logística</h1>

## Contexto
A área de logística de uma empresa automotiva fictícia busca otimizar a eficiência operacional e melhorar a satisfação dos clientes através de uma gestão mais precisa das suas operações de transporte. Eles desejam, especialmente, avaliar os atrasos nas entregas e que fatores estão relacionados a esses atrasos, para que possam operar nesses problemas e assim melhorar seus resultados e atendimento aos seus clientes.

## Objetivos
O objetivo da análise é identificar fatores relacionados ao atraso nas entregas e propor soluções que diminuam as taxas de atraso, melhorando assim a qualidade dos serviços da empresa e consequentemente aumentando a satisfação dos clientes.

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

**1. Indique o total de viagens e a porcentagem dentro e fora do prazo**  
aaaaa

**2. Apresente o total de viagens por tipo de veículo**  
aaaa

**3. Apresente o total de viagens por transportadora**  
aaaaaaa

**4. Qual o valor total de frete, por ano avaliado?**  
aaaa

**5. Quais regiões mais contaram com entregas?**  
aaaa

<br>

### 3. Respondendo às perguntas de negócio

**1. Indique o total de viagens, valor de frete e peso de carga, por tipo de veículo.**  
aaa

**2. Que tipo de veículo mais atrasou entregas?**  
aaa

**3. Há relação com a carga e o atraso?**  
aaa

**4. Que regiões tiveram maior atraso nas entregas?**  
aaa

**5. Que regiões têm maior custo de frete? Qual a margem de atraso?**  
aaa

**6. Que períodos do ano contaram com maior valor de frete?**  
aaa

**7. Que transportadora mais realizou viagens? Qual o desempenho delas em relação ao atraso nas entregas? utilizar KPI**  
aaa


<br>

### 4. Sugestões
De maneira geral, a taxa de churn dos serviços é altíssima, quase 40%. O ideal é que esteja mais próxima de 0 possível, sendo 5% um valor aceitável. Se temos 40% como taxa de churn, estamos 8x acima do cenário ideal e isso é preocupante. O foco das sugestões será a redução dos cancelamentos, segue alguns pontos que podemos considerar para melhorar nossa retenção:

* **Primeiro, foco:** Devemos focar em assinaturas do tipo anual e campanhas do tipo Recorrente. Um programa de membros pode ajudar a unir essas duas opções, ofertando produtos diferenciados e exclusivos para os clientes que optarem por essa opção. No geral, aumentar o contato com o cliente, melhorar o atendimento e estar atento às preferências de acordo com seu perfil, são ações que podem melhorar a confiança e fidelidade desses clientes, aumentanddo nossa retenção.

* **Programas de Fidelização:** Com uma taxa de churn de quase 40%, devemos desenvolver programas de fidelização para nossos clientes. Oferecer descontos e ofertas em meses comemorativos (vai criar no cliente a expectativa de receber uma nova promoção nas próximas datas comemorativas); incentivar a assinatura para pacotes família ou assinatura compartilhada (aumentando a fidelização do cliente) e inserir também programas de recomendação, concedendo descontos ou mensalidade grátis para cada indicação bem sucedida, são medidas que podem fazer nossos clientes ficarem mais tempo.

* **Avaliar a campanha Promocional:**  Quase 1/3 dos clientes vieram através da campanha promocional e mais de 70% deles cancelaram. Devemos analisar que programas de fidelização foram aplicadas para manter esses clientes e, se foram aplicadas, qual o motivo de seu fracasso. A retenção foi baixíssima para essa campanha, apesar da alta captação de clientes. Devemos nos perguntar: o público alvo da campanha tinha real interesse no que foi ofertado? Houveram muitas reclamações dos que vieram por essa campanha? O que foi feito para manter esse clientes? Essas perguntas podem nos guiar a otimizar uma próxima campanha promocional (que teve boa captação) e aumentar a retenção de clientes através dela.
