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
No período de janeiro/2022 a agosto/2023 tivemos um total de 8.362 viagens. Desse total:

* 5.830 foram dentro do prazo (69,72%)
* 2.432 foram com atraso (29,08%)

**2. Apresente o total de viagens por transportadora**  
| Transportadora | Total de Viagens | % do Total |
|----------------|------------------|------------|
| Log Elite             | 5.400 | 64,58% |
| RodaFirme Transportes | 1.238 | 14,80% |
| Cargas Bahia          | 1.157 | 13,84% |
| ExpressCargo          | 567   |  6,78% |

**3. Apresente o total de viagens por tipo de veículo**  
| Veículo | Total de Viagens | % do Total |
|----------------|------------------|------------|
| Truck   | 4.994 | 59,72% |
| VUC     | 1.643 | 19,65% |
| Carreta | 1.359 | 16,25% |
| Toco    |   366 |  4,38% |

**4. Qual o valor total de frete, por ano avaliado?**  
O valor total de frete para 2022 inteiro foi de R$22,92 milhões. Como 2023 vai até agosto em nossa análise, vamos considerar esse mesmo período para os dois anos:
* Janeiro/2022 a Agosto/2022: R$15,59 milhões
* Janeiro/2023 a Agosto/2023: R$17,18 milhões

Agosto de 2022 contou com um valor de frete 10,20% maior que o mesmo período do ano passado.

**5. Quais estados mais contaram com entregas?**  
Os estados de São Paulo, Minas Gerais, Paraná, Rio Grande do Sul e Santa Catarina foram os principais destinos das entregas. No geral, as regiões Sul e Sudeste detém nossa maior clientela.

<br>

### 3. Respondendo às perguntas de negócio

**1. Indique o total de viagens, valor de frete e peso de carga, por tipo de veículo.**  
aaa

**2. Que tipo de veículo mais atrasou entregas?**  
aaa

**3. Há relação com o peso de carga e o atraso?**  
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
