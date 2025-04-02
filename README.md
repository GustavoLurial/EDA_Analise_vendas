# Análise Exploratória de Vendas
![image](https://github.com/user-attachments/assets/684bbd4f-3017-4612-89d0-6457c1b9591c)

Este projeto consiste na análise dos dados de vendas de chocolate disponibilizados no [Kaggle]([https://dados.gov.br/dados/conjuntos-dados/venda-de-medicamentos-controlados-e-antimicrobianos---medicamentos-industrializados](https://www.kaggle.com/datasets/atharvasoundankar/chocolate-sales)), com objetivo de entender a dinâmica das vendas.

## Etapas:
### **1 - Entendimento do negócio**
A análise a seguir traz insights sobre como as vendas de uma empresa especializada em vendas de chocolate estão acontecendo, tendo em vista a necessidade de entender padrões de vendas, funcionários mais capacitados, produtos com maior demanda e regiões que estão de destacando

Analisar e entender dados de vendas podem trazer insights importantes sobre quais decisões e ações tomar, baseado em um fato.

A EDA a seguir tem como objetivo aprimorar os meus conhecimentos.

### **2 - Entendimento dos dados**
Para realizar essa análise irei usar uma base de vendas de chocolates do kaggle: https://www.kaggle.com/datasets/atharvasoundankar/chocolate-sales

Columns & Description:
- Sales Person : Name of the salesperson responsible for the transaction
- Country : Sales region or store location where the transaction took place
- Product: Name of the chocolate product sold.
- Date: The transaction date of the chocolate sale.
- Amount: Total revenue generated from the sale.
- Box Shipped: Number of chocolate boxes shipped in the order.

### **3 - Importações e Pré-Processamentos**
Aqui realizei a limpeza dos dados, mudando para os tipos certos e substituindo caracteres especiais. 
Realizei também a criação de variáveis novas para as análises.

### **4 - Análise Exploratória de Dados (EDA)**
Realizei as análises dividindo em Análises Univariadas categóricas/numéricas e Análises Multivariadas categóricas/numéricas

### **5 - Insights e recomendações**

### Analises Estatisticas Univariadas:

- 1. Aumento da Receita
-- O histograma de "Amount" (Valor total das vendas) mostra uma distribuição assimétrica à direita, indicando que a maioria das vendas ocorre em faixas menores de faturamento, mas há outliers com valores altos.
Ação: Estratégias para incentivar compras maiores, como descontos progressivos ou pacotes promocionais, podem ajudar a aumentar o ticket médio.
-- O gráfico de "Amount per box" mostra que a maioria das caixas vendidas tem um valor unitário baixo, o que sugere que os preços podem estar comprimidos.
Ação: Explorar a possibilidade de lançar produtos premium ou pacotes de edição limitada para aumentar o valor médio por caixa.

- 2. Redução de Custos
-- O histograma de "Boxes Shipped" mostra que a maioria dos pedidos envolve um número relativamente baixo de caixas, mas há um longo cauda de pedidos grandes.
Ação: Avaliar os custos logísticos e ver se pedidos pequenos estão gerando ineficiências no transporte. Programas de "Pedido Mínimo para Frete Grátis" podem ajudar a reduzir a frequência de envios pequenos e aumentar a eficiência operacional.
-- A variação de "Amount per box" sugere que pode haver oportunidades de otimização na precificação ou embalagem.
Ação: Verificar se o custo de embalagem e distribuição está alinhado com a margem de lucro dos diferentes produtos.

- 3. Melhoria na Qualidade de Vida
-- Caso a empresa tenha clientes corporativos ou revendedores, os pedidos muito pequenos podem indicar dificuldades na gestão de estoque por parte dos clientes.
Ação: Oferecer soluções como assinaturas de chocolates para garantir um fluxo previsível de pedidos e reduzir a necessidade de pequenos reabastecimentos.
-- Se os produtos forem voltados para consumidores finais, o preço baixo por caixa pode indicar que clientes compram chocolates esporadicamente e em pequenas quantidades.
Ação: Criar programas de fidelidade para incentivar compras frequentes e aumentar o engajamento do consumidor.

- 1. Oportunidades para Aumento de Receita
-- O ticket médio por pedido é 5.652,31, mas há uma alta variação (desvio padrão: 4.102,44) e pedidos chegando a 22.050,00.
-- Ação: Criar estratégias para aumentar o ticket médio, como pacotes de produtos premium, descontos progressivos ou brindes para compras acima de um certo valor.
-- A mediana do "Amount per box" é 36,15, mas a média está em 105,72, o que sugere que poucos pedidos de alto valor distorcem a média. Além disso, o percentil 75% é 79,16, mostrando que 75% dos pedidos têm um valor por caixa inferior a esse.
-- Ação: Trabalhar na precificação, possivelmente segmentando produtos para diferentes públicos e destacando itens de maior valor agregado.

- 2. Redução de Custos
-- A mediana de caixas enviadas por pedido é 135, mas há pedidos pequenos (mínimo de 1 caixa) e muito grandes (máximo de 709 caixas).
-- Ação: Avaliar se pedidos pequenos estão gerando custos logísticos desproporcionais. Criar incentivos para compras em maior volume pode ajudar a reduzir o número de pedidos pequenos e otimizar a logística.
-- O Amount per box tem uma variação extremamente alta (desvio padrão de 278,66, com pedidos indo de 0,01 até 4.291,00).
-- Ação: Pode ser interessante analisar se certos clientes ou canais de venda têm um valor muito abaixo da média, indicando necessidade de ajustes na política de precificação.

- 3. Melhorias na Qualidade de Vida
-- Se houver um número significativo de pedidos pequenos, pode indicar que os clientes têm dificuldades na gestão de estoque ou fluxo de caixa.
-- Ação: Criar um programa de assinatura ou recompra automática pode facilitar a vida dos clientes e garantir um fluxo de pedidos mais previsível.
-- A grande dispersão no Amount per box sugere que pode haver diferenças significativas nos tamanhos das embalagens ou produtos vendidos.
-- Ação: Analisar se os produtos mais baratos são acessíveis para clientes de baixa renda e se há formas de melhorar a acessibilidade a chocolates premium.

### Análise multidimensional:
- **1 Foco nos produtos de maior receita**

O produto "Smooth Silky Salty" lidera as vendas em receita, seguido de "50% Dark Bites" e "White Choc".

Estratégias como campanhas promocionais e aumento da distribuição podem maximizar a lucratividade desses produtos.

- **2 Expansão dos produtos premium**

Produtos como "99% Dark & Pure" e "85% Dark Bars" aparecem no topo, indicando que há demanda por chocolates com alto teor de cacau.

Explorar variações desses produtos ou criar novos sabores pode ser uma boa estratégia.

- **3 Revisão dos produtos com menor receita**

O último colocado, "70% Dark Bites", tem uma receita significativamente menor.

Precisamos entender se o problema está na precificação, demanda ou falta de marketing.

- **4 Produtos com alto volume de vendas, mas baixa margem**

Se algum dos produtos bem vendidos tem baixo valor agregado, pode ser interessante reajustar preços ou otimizar custos de produção.

- **5 Oportunidade de cross-sell**

Combinar produtos mais vendidos com outros complementares em promoções pode incentivar compras maiores.

Exemplo: Se "Smooth Silky Salty" vende bem, podemos oferecer pacotes com "Peanut Butter Cubes".

- Podemos notar que o vendedor que teve a maior frequência de venda não foi o que mais gerou receita, indicando que não devemos olhar apenas pela quantidade de itens vendidos, mas sim quais foram os itens vendidos
- Como estratégia podemos entender quais foram os produtos que o Ches vendeu e replica-los para o Kelci
- Podemos também identificar quais foram os produtos que Wilone vendeu e entender se na região onde ele se encontra a procura pelos produtos mais caros é muito baixa
- Outro ponto é entender os vendedores não estão sobrecarregados
- Caso venhamos a desligar algum funcionario, devemos cruzar as informações com a quantidade de produtos vendidos e a receita gerada
- O vendedor Wilone possui a menor quantidade de receita vendida e a menor quantidade de produtos vendidos, entender se isso é causado pela região que ele está alocado
- Podemos observar que quase metade dos vendedores estão abaixo da média
- Podemos observar que ambos os gráficos seguem a mesma tendência durante o tempo
- Outro ponto que podemos observar é que o mês que mais teve venda não foi necessariamente o mês que mais lucrativo. Podemos observar que Janeiro foi o mês que gerou a maior receita, enquanto Junho foi o mês com o maior número de itens vendidos.
- Cabe estudar mais afundo o que houve nesses meses
