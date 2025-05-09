<h1 align="center"> 📊 Business Case - Dashboard de Logística</h1>

<p align="center">
  <img src="https://github.com/user-attachments/assets/0c74de87-d8fd-4f44-bbe2-f16bce5e1c66" alt="imagem" width="1100"/>
</p>

## 📃 Contexto
A área de logística de uma empresa automotiva fictícia busca otimizar a eficiência operacional e melhorar a satisfação dos clientes através de uma gestão mais precisa das suas operações de transporte. Eles desejam, especialmente, avaliar os atrasos nas entregas e que fatores estão relacionados a esses atrasos, para que possam operar nesses problemas e assim melhorar seus resultados.

***

<br>

## 🎯 Objetivos
O objetivo da análise é identificar fatores relacionados ao atraso nas entregas e propor soluções que diminuam as taxas de atraso, melhorando assim a qualidade dos serviços da empresa e consequentemente aumentando a satisfação dos clientes.

***

<br>

## 🧱 Estrutura do Projeto
### 🗄 Banco de dados
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

***

<br>

### 🔎 Análise Exploratória

#### 📌 1. Indique o total de viagens e a porcentagem dentro e fora do prazo**  
No período de janeiro/2022 a agosto/2023 tivemos um total de 8.362 viagens. Desse total:

* 5.830 foram dentro do prazo (69,72%)
* 2.432 foram com atraso (29,08%)

--

#### 📌 2. Apresente o total de viagens por transportadora**  
| Transportadora | Total de Viagens | % do Total |
|----------------|------------------|------------|
| Log Elite             | 5.400 | 64,58% |
| RodaFirme Transportes | 1.238 | 14,80% |
| Cargas Bahia          | 1.157 | 13,84% |
| ExpressCargo          | 567   |  6,78% |

--

#### 📌 3. Apresente o total de viagens por tipo de veículo**  
| Veículo | Total de Viagens | % do Total |
|----------------|------------------|------------|
| Truck   | 4.994 | 59,72% |
| VUC     | 1.643 | 19,65% |
| Carreta | 1.359 | 16,25% |
| Toco    |   366 |  4,38% |

--

#### 📌 4. Qual o valor total de frete, por ano avaliado?**  
O valor total de frete para 2022 inteiro foi de R$22,92 milhões. Como 2023 vai até agosto em nossa análise, vamos considerar esse mesmo período para os dois anos:
* Janeiro/2022 a Agosto/2022: R$15,59 milhões
* Janeiro/2023 a Agosto/2023: R$17,18 milhões

Agosto de 2022 contou com um valor de frete 10,20% maior que o mesmo período do ano passado.

--

#### 📌 5. Quais estados mais contaram com entregas?**  
Os estados de São Paulo, Minas Gerais, Paraná, Rio Grande do Sul e Santa Catarina foram os principais destinos das entregas. No geral, as regiões Sul e Sudeste detém nossa maior clientela.

***

<br>

### 📍 Respondendo às perguntas de negócio

#### 📌 1. Indique a taxa de atraso e as médias de valor de frete e peso de carga, por tipo de veículo.**  
Carreta e VUC contam com as maiores taxas de atraso, 30,68% e 29,28%, respectivamente.
| Veículo | Taxa Atraso | Média Valor Frete | Média Peso Carga (kg) |
|---------|-------------|-------------------|-----------------|
| Truck   | 28,69% | R$5,32 mil | 6,56 mil  kg |
| VUC     | 29,28% | R$844,88   | 1,11 mil  kg |
| Carreta | 30,68% | R$8,26 mil | 12,99 mil kg |
| Toco    | 27,60% | R$2,50 mil | 3,30 mil  kg |

#### 📌 2. Há relação com o peso de carga e o atraso?**  
Não é possível relacionar peso e taxa de atraso, uma vez que, conforme tabela vista anteriormente, Carreta tem maior peso médio de carga e VUC tem menor peso médio, no entanto, ambos têm taxa de atraso muito semelhante. O fator atraso pode estar relacionado ao desempenho dos próprios veículos com a distância do transporte.

#### 📌 3. Que regiões tiveram maior atraso nas entregas?**  
Os estados de Alagoas, Maranhão e Piauí contaram com maior taxa de atraso, 33% em ambos. Além disso, outros dois estados da região também possuem valor semelhante: Ceará (32%) e Paraíba (31%). Logo, podemos considerar a região Nordeste como aquela com maior taxa de atraso.

#### 📌 4. Que regiões têm maior custo médio de frete? Qual a margem de atraso para essas regiões?**  
Selecionando o Top 3: Minas Gerais, Piauí e Rio de Janeiro têm maior custo de frete. Na tabela a relação Custo frete x Taxa atraso:
| Estado | Custo Médio Frete | Taxa Atraso |
|--------|-------------------|-------------|
| MG  | R$6,74 mil | 29% |
| PI  | R$4,76 mil | 33% |
| RJ  | R$4,72 mil | 30% |

#### 📌 5. Que transportadora mais realizou viagens? Qual o desempenho delas em relação ao atraso nas entregas?**  
| Transportadora | Total Viagens | Taxa Atraso |
|----------------|---------------|-------------|
| Cargas Bahia          | 1,16 mil | 30,08% |
| ExpressCargo          | 567      |     0% |
| Log Elite             | 5,40 mil | 31,28% |
| RodaFirme Transportes | 1,22 mil | 31,91% |

***

<br>

### 📈 Recomendações Estratégicas
De acordo com a análise, podemos considerar alguns pontos:
* Descartar o fator peso de carga como principal influenciador dos atrasos no transporte;
* No geral, a região Nordeste conta com maior taxa de atraso. Considerando que a maior parte dos transportes para essa região vieram de Campinas/SP, podemos considerar fatores externos para esse atraso: distância do transporte, qualidade das estradas para essas regiões;
* As transportadores têm desempenho semelhante no que diz respeito aos atrasos.

De acordo com esses pontos e análise em geral, podemos tomar algumas das seguintes decisões:
* Buscar otimizar o transporte, verificando a viabilidade de utilizar as transportadores de Salvador para atender especialmente o Nordeste (transportes saídos de Salvador para as outras cidades do Nordeste têm menor taxa de atraso quando comparados a Campinas e Manaus);
* Aumentar o prazo contratado para as regiões cuja margem de atraso é maior, especialmente considerando que esses atrasos podem estar ligados a fatores externos (qualidade da estrada, distância);
* Dar preferência a veículos do tipo Carreta e Truck, que contaram com melhor desempenho na relação atraso x peso de carga.

