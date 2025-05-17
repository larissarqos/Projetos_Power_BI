

<h1 align="center"> 📊 Business Case - Análise de Vendas </h1>

<p align="center">
  <img src="https://github.com/user-attachments/assets/4857c915-c3ea-4c16-b664-110d5f3dceb1" alt="hr" width="1100"/>
</p>

<br>

## 📃 Contexto  
O setor comercial de uma rede fictícia de lojas de roupas deseja avaliar o desempenho de suas filiais ao longo do ano de 2024. Com uma **meta mensal de R$7.000,00 por loja**, a empresa busca entender se os objetivos foram alcançados, identificar quais unidades e produtos geraram maior retorno, além de obter uma visão consolidada sobre seu faturamento anual.

***

<br>

## 🛠️ Ferramentas e Métodos Utilizados
- Microsoft Excel (fórmulas, tabelas dinâmicas, gráficos, slicers)
- Business Intelligence
  
***

<br>

## 🎯 Objetivos  
Para atender à demanda da empresa, realizamos uma análise exploratória das vendas de 2024, com foco nas seguintes questões-chave:

- Qual foi o faturamento de 2024?   
- Quais lojas mais se destacaram em vendas?  
- Quais foram os produtos mais vendidos?  
- As lojas atingiram a meta mensal estabelecida de R$7.000,00?

Com base nessas perguntas, conseguimos avaliar o desempenho por loja, produto e mês — oferecendo à empresa uma visão clara sobre os pontos fortes e oportunidades de melhoria.

***

<br>

## 🧱 Estrutura do Projeto  

### 🗄 Banco de dados  

| Coluna           | Descrição                                              |
|------------------|--------------------------------------------------------|
| Loja             | Nome da filial                                         |
| Data             | Data da venda                                          |
| Produto          | Produto vendido                                        |
| Valor_Unitario   | Valor unitário do produto                              |
| Quantidade       | Quantidade vendida                                     |
| Valor_Total      | Valor total da venda (Quantidade × Valor Unitário)     |

***

<br>

### 📍 Respondendo às perguntas de negócio

#### 📌 1. Qual foi o faturamento de 2024?  
O faturamento total do ano foi de **R$461.743,30**. As lojas do **Leblon** e de **Ipanema** lideraram as vendas, responsáveis por **28%** e **21,8%** do total, respectivamente.

| Loja     | Faturamento      | Participação no total  |
|----------|------------------|------------------------|
| Leblon   | R$129.020,00     | 28%                    |
| Ipanema  | R$100.448,64     | 21,8%                  |
| Botafogo | R$91.200,00      | 19,8%                  |
| Barra    | R$73.385,08      | 15,9%                  |
| Tijuca   | R$67.689,58      | 14,6%                  |
| **Total**| **R$461.743,30** | **100%**               |

--

#### 📌 2. Quais lojas mais se destacaram em vendas?  
Em 2024, foram registradas **759 vendas**, totalizando **2.308 itens**. As filiais do **Leblon** e de **Ipanema** lideraram tanto em número de vendas quanto em faturamento.

--

#### 📌 3. Quais foram os produtos mais vendidos?  
As vendas foram bem distribuídas entre os produtos. Porém, em termos de faturamento, os destaques foram **Camisa Linho**, **Oxford** e **Joa**, que juntas representaram mais de **70% do faturamento**.

| Produto         | Nº de Vendas | Quantidade | Faturamento Anual | % do Total  |
|-----------------|--------------|------------|-------------------|-------------|
| Camisa Oxford   | 158          | 480        | R$100.464,00      | 21,75%      |
| Camiseta Navy   | 157          | 479        | R$80.136,70       | 17,36%      |
| Camiseta Joa    | 151          | 480        | R$97.104,00       | 21,03%      |
| Camiseta Pima   | 149          | 423        | R$50.506,20       | 10,94%      |
| Camisa Linho    | 144          | 446        | R$133.532,40      | 28,92%      |
| **Total**       | **759**      | **2.308**  | **R$461.743,30**  | **100%**    |

--

#### 📌 4. As lojas atingiram a meta mensal estabelecida de R$7.000,00? **  
Com base no faturamento médio mensal por loja (faturamento total ÷ 12), apenas **3 das 5 filiais** alcançaram ou superaram a meta: **Leblon, Ipanema e Botafogo**.

**Resumo por loja:**

- **Leblon** – R$10.388,30/mês: Melhor desempenho do ano. Abaixo da meta apenas em setembro, com crescimento contínuo a partir de outubro.

- **Ipanema** – R$8.370,72/mês: Crescimento a partir de março. Consistente no restante do ano, sempre próxima ou acima da meta.

- **Botafogo** – R$7.600,00/mês: Regular ao longo do ano, exceto em julho.

- **Barra** – R$6.115,42/mês: Acima da meta apenas em julho, novembro e dezembro. Desempenho fraco em setembro.

- **Tijuca** – R$5.610,17/mês: Atingiu ou superou a meta em apenas 5 meses. Início e fim do ano com queda nas vendas.

***

<br>

### 📈 Recomendações Estratégicas
Com base na análise dos dados e padrões identificados, algumas ações podem ser adotadas:

#### 🟦 Ações por loja
- **Campanhas promocionais focadas nas lojas com menor desempenho:** Promoções sazonais, descontos progressivos e ações em datas comemorativas podem ajudar a impulsionar vendas, principalmente no primeiro trimestre.
  
#### 🟦 Ações por produto
- **Aproveitar o potencial dos produtos mais lucrativos:** Campanhas de marketing direcionadas para os best-sellers (como Camisa Linho e Oxford) podem alavancar ainda mais o faturamento.

***

<br>

### 🚀 Impacto Esperado
A adoção das estratégias sugeridas pode gerar impactos positivos tanto no aumento de faturamento quanto na eficiência operacional da rede de lojas. Com base nos dados de 2024, os seguintes resultados são projetados:

#### 🟩 Aumento no faturamento das lojas de pior desempenho (Barra e Tijuca)
- **Projeção:** Se as lojas Barra e Tijuca alcançarem o faturamento médio de Ipanema e Botafogo (aproximadamente R$8.000/mês), o ganho potencial anual para cada uma das lojas é de ~ R$96.000. O faturamento total anual subiria de R$461,743 para  ~R$508.800, um **aumento percentual de ~11,4%**. 
- **Impacto:** Redução da disparidade entre filiais e maior previsibilidade de receita.
  
#### 🧮 Cálculo da projeção:
Média mensal de Ipanema e Botafogo: (R$8.370 + R$7.600) / 2 = R$7.985, arredondado para R$8.000
Projeção anual para Barra e Tijuca: R$8.000 * 12 = R$96.000 (cada)

* Novo faturamento anual estimado:

  Leblon: R$10.400 * 12 = R$124.800
  
  Ipanema: R$8.400 * 12 = R$100.800
  
  Botafogo: R$7.600 * 12 = R$91.200
  
  Barra: R$8.000 * 12 = R$96.000  
  
  Tijuca: R$8.000 * 12 = R$96.000
  
  Total: ~R$508.800

--

#### 🟩 Aumento de 10% nas vendas dos produtos mais lucrativos (Camisa Linho, Oxford e Joa)
- **Projeção:** Um aumento de apenas 10% nas vendas dos três produtos mais lucrativos pode gerar um acréscimo de aproximadamente R$32.800 ao faturamento anual, um **aumento percentual de ~ 7,1%**.
- **Impacto:** Elevação direta da receita sem necessidade de ampliar a cartela de produtos.
  
#### 🧮 Cálculo da projeção:

* **Camisa Linho:**
  Vendas atuais: 144 unidades + 10% = 158 unidades
  
  Valor médio por unidade: R$133.530 / 144 = ~ R$927,30
  
  Novo faturamento: 158 * R$927,30 ~ R$146.513



* **Camisa Oxford:**
  
  Vendas atuais: 158 unidades + 10% = 174 unidades
  
  Valor médio por unidade: R$100.460,00 ÷ 158= ~ R$636
  
  Novo faturamento: 174 * R$636 ~ R$110.664


* **Camiseta Joa:**
  
  Vendas atuais: 151 unidades + 10% = 166 unidades
  
  Valor médio por unidade: R$97.100 / 151 = ~ R$643,00
  
  Novo faturamento: 166 * R$643,00 ~ R$106.738

* **Total:**
  
  Novo total dos 3 produtos: R$146.513 + R$110.664 + R$106.738 = R$363.915  
  
  Faturamento atual dos 3 produtos: R$331.100  
  
  Acréscimo estimado: R$363.915 − R$331.100 = ~ R$32.815  

  Aumento percentual no faturamento total: (R$32.815 / R$461.743) * 100 = ~7,1%

***

<br>

*Este projeto foi desenvolvido como parte do meu portfólio em análise de dados. Sinta-se à vontade para explorar os dados, sugerir melhorias ou entrar em contato!*
