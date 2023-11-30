# Análise Exploratória de Dados da Olist

<img src="reports/logo1.png">

# 1. Descrição
- Neste projeto, realizarei uma análise exploratória de dados de um e-commerce brasileiro, a Olist. Algumas perguntas de negócio serão formuladas e respondidas através de técnicas de coleta, limpeza, exploração e visualização de dados.
- Este é um conjunto de dados público de comércio eletrônico brasileiro de pedidos feitos na Olist Store. O conjunto de dados contém informações de 100 mil pedidos de 2016 a 2018 feitos em vários marketplaces no Brasil. Suas características permitem visualizar um pedido a partir de várias dimensões: desde o status do pedido, preço, desempenho de pagamento e frete até a localização do cliente, atributos do produto e, finalmente, análises escritas pelos clientes. Também foi lançado um conjunto de dados de geolocalização que relaciona os códigos postais brasileiros a coordenadas de latitude/longitude.
- Este conjunto de dados foi generosamente fornecido pela Olist, a maior loja de departamentos nos marketplaces brasileiros. A Olist conecta pequenas empresas de todo o Brasil a canais sem complicações e com um único contrato. Esses comerciantes podem vender seus produtos através da Olist Store e enviá-los diretamente para os clientes usando os parceiros logísticos da Olist. Saiba mais em seu site: www.olist.com
- Após um cliente comprar o produto da Olist Store, um vendedor é notificado para atender ao pedido. Assim que o cliente recebe o produto, ou a data de entrega estimada expira, o cliente recebe uma pesquisa de satisfação por e-mail, onde pode atribuir uma nota para a experiência de compra e escrever alguns comentários.
- Abaixo, tem-se o schema do banco de dados, utilizado para unir datasets e obter os dados necessários para responder as perguntas de negócio.

<img src="reports/schemaOlist.png">

# 2. Tecnologias utilizadas
Python (Pandas, Numpy, Matplotlib, Seaborn), Jupyter Notebook, Git e Github (versionamento de código), Anaconda (terminal e ambiente virtual) e VSCode (ambiente de desenvolvimento).

# 3. Perguntas de negócio 
As seguintes perguntas de negócio foram formuladas por mim e respondidas, com o objetivo de descrever aspectos sobre os pedidos, clientes, vendedores, itens comprados, entre outros fatores, a fim de possibilitar futuras tomadas de decisão informadas para a empresa.

1. Qual o preço médio dos produtos comprados?
2. Qual o valor médio pago por pedido?
3. Em quantas parcelas, em média, os pedidos são parcelados?
4. Quais estados vendem mais? (número de pedidos e valor médio pago por pedido)
5. Quais cidades vendem mais?
6. Quais as categorias de item mais vendidas?
7. Quais as categorias de item mais vendidas por região?
9. Qual o número médio de itens por pedido?
10. Onde estão localizados os clientes?
11. Onde estão localizados os vendedores?
12. Qual o número médio de parcelas no pagamento, por região?
13. Como se dá a evolução mensal das vendas ao longo do tempo?
14. Como se dá a evolução das vendas ao longo do dia? Em quais horários são feitos mais pedidos?
15. Como se dá a evolução das vendas ao longo da semana? Em quais dias da semana são feitos mais pedidos?
16. Qual o valor médio do frete pago por pedido?
17. Em quais regiões se paga um maior frete e um menor frete, em média? E quanto aos estados?
18. Qual o review score médio dos pedidos?
19. Quais regiões do país apresentam um maior review score nos seus pedidos, e um menor? E quanto aos estados?
20. Qual o número médio de dias para se entregar um pedido?
21. Quais regiões do país apresentam o maior tempo médio de entrega, e o menor? E quanto aos estados?
22. Existe alguma correlação entre o valor pago em um pedido e o número de parcelas escolhido para o pagamento?

# 4. Planejamento da solução
O seguinte passo a passo foi seguido, baseado no framework CRISP-DM

1. Coleta de dados.
2. Entendimento do contexto negócio.
3. Entendimento dos dados.
4. Limpeza dos dados.
5. Análise exploratória de dados.
6. Conclusão.

# Principais insights de negócio

1. Estados das regiões sul e sudeste concentram os maiores números de pedidos, clientes e vendedores. Em especial, o estado de São Paulo e a sua capital apresentam valores maiores que todos os outros. Enquanto isso, estados das regiões norte e nordeste apresentam os menores indicadores.

<img src="reports/pedidos_por_estado.png">

<img src="reports/pedidos_por_cidade.png">

<img src="reports/clientes_por_estado.png">

<img src="reports/vendedores_por_estado.png">

2. Entre os itens mais vendidos, estão produtos para a casa e móveis, produtos de cama, mesa e banho, e produtos para beleza e saúde.

<img src="reports/itens_mais_vendidos.png">

3. Clientes das regiões norte e nordeste tendem a dividir o pagamento em um maior número de parcelas por pedido (em média), enquanto clientes das regiões sul e sudeste apresentam um menor número. Isso faz sentido, uma vez que tais regiões possuem os piores indicadores de renda do país.

<img src="reports/parcelas_por_estado.png">

4. De forma geral, as vendas cresceram ao longo dos dois anos, atingindo seu ápice em novembro de 2017, provavelmente por conta da black friday.

