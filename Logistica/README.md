Business Case - Dashboard de Logística

Contexto
A área de logística de uma empresa automotiva fictícia busca otimizar a eficiência operacional e melhorar a satisfação dos clientes através de uma gestão mais precisa das suas operações de transporte. O time realiza reuniões mensais com as transportadoras contratadas e precisa de uma visão detalhada das operações, que permita a análise de rotas, desempenho de transporte e otimização de recursos.

Dicionário da base de dados

Coluna
Descrição
Load
Código da carga
Transportadora
Nome da transportadora responsável
Origem-Cidade
Cidade de origem
Origem-UF
Estado de origem
Destino
Cidade e Estado de destino
Peso Bruto (kg)
Peso bruto da carga em kg
Cubagem (m³)
Cubagem da carga, em m³
Data de Coleta
Data da coleta do produto
Data de Entrega
Data de entrega do produto
Prazo Realizado (dias)
Diferença entre a data de entrega e a data de coleta, em dias
Prazo Contratado (dias)
Prazo contratado para realização da entrega, em dias


Segue descrição das colunas da base de dados. As agrupei de acordo com aquilo que se relacionam, ficando em 4 grupos: Características dos clientes; Tipo de gasto; Tipo de compra; Compra por campanha.

Características dos clientes - Agrupa as colunas relacionadas a características pessoais dos clientes: ID, Ano Nascimento, Idade, Faixa Etária, Escolaridade, Estado Civil, Salário Anual, Filhos em Casa, Adolescentes em Casa, Data Cadastro, Dias Desde Última Compra e País;

Tipo de gasto - Agrupa as colunas que contêm os valores gastos com as categorias dos produtos da empresa: Gasto com Eletrônicos, Gasto com Brinquedos, Gasto com Móveis, Gasto com Utilidades, Gasto com Alimentos, Gasto com Vestuário;

Tipo de compra - Agrupa as colunas relacionadas ao número de compras em cada canal da empresa: Número de Compras com Desconto, Número de Compras na Web, Número de Compras via Catálogo, Número de Compras na Loja, Número de Compras na Web;

Compra por campanha - Inclui as colunas que indicam se houve ou não compras nas campanhas de marketing, sendo 0 para não e 1 para sim: Compra na Campanha 1, Compra na Campanha 2, Compra na Campanha 3, Compra na Campanha 4,Compra na Campanha 5, Compra na Campanha 1, Total Compras Campanhas (para identificar, de forma geral, quem comprou em 1, 2 ou mais das campanhas de marketing);

Outros: As colunas Adolescentes em Casa, Data Cadastro, Dias desde Última Compra, Número Visitas WebSite Mês, e Comprou não foram utilizadas nesta análise.

Objetivos da análise
O objetivo da análise é identificar possíveis problemas de desempenho no setor e sugerir soluções aplicáveis para estes. Para isso, nossa análise buscará responder às seguinte perguntas:
Nossas entregas têm sido realizadas dentro do prazo?
O valor do frete tem apresentado grande variação? 
Qual o desempenho dos nossos tipos de veículo?
Como está a eficiência do transporte?

Indicadores Chave de Desempenho (KPIs) e Métricas
On Time Delivery (OTD): Percentual de entregas realizadas dentro do prazo contratado (quantidade de entregas no prazo / total entregas);
Quantidade de Viagens: Total de Viagens realizadas por tipo de veículo, categorizando entre VUC, Toco, Truck e Carreta;
Evolução do Frete: Análise temporal do valor do frete;
Peso e Cubagem Transportada: Medição do peso e cubagem total das cargas transportadas;
Desempenho por Região: Performance regional com base nas entregas dentro e fora do prazo.

Perguntas e respostas (análise descritiva)
1. Nossas entregas têm sido realizadas dentro do prazo?
Considerando 100% como todas as entregas dentro do prazo, nosso transporte conta com uma taxa de 68,80% de sucesso. Não há grande variação deste valor por estado, todos contam com uma taxa de atraso entre 28% e 35%.

imagem 1. Gráfico de barras - Status de entrega

Dada a meta estabelecida de 80% para taxa de entregas dentro do prazo, estamos 11,20% abaixo dela.

imagem 2. Indicador - Ontime Delivery (OTD)

     


     2. O valor do frete tem apresentado grande variação?
Contamos com uma queda significativa no valor do frete de janeiro de 2022 para fevereiro do mesmo ano (diferença aproximada de R$1,7 milhões). Houve aumento expressivo em janeiro de 2023, fazendo o valor total do frete ficar acima da faixa dos R$2,0 Mi (embora tenha havido queda em março de 2023, R$1,85 Mi).
   	
imagem 3. Gráfico de linha - Valor do frete ao longo do tempo

Impacto frete vendas

     3. Qual o desempenho dos nossos tipos de veículos?
     4. Como está o desempenho das nossas transportadoras?
     

Sugestões para melhora de performance (análise prescritiva)
 
Nossas entregas têm sido realizadas dentro do prazo?
O valor do frete tem apresentado grande variação? 
Qual o desempenho dos nossos tipos de veículo?
Como está a eficiência do transporte?



Performance de Transporte(OTD): Medir o percentual de entregas dentro do prazo para melhorar a pontualidade e a satisfação do cliente;
Mapa: Visualizar o valor do frete de acordo com a localidade de destino;
Viagens por Tipo de Veículo: Analisar a distribuição das viagens por tipo de veículo (caminhão) para otimizar o uso da frota;
Evolução do Valor do Frete: Monitorar a variação do custo do frete ao longo do tempo, para ajustar estratégias de precificação;
Total de Viagens, Peso e Cubagem: Avaliar a eficiência do transporte analisando o total de viagens, peso e cubagem transportada.

