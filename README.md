# Dashboard de Vendas

📊 Dashboard de Vendas — Eletrônicos
<p align="left">
  <img src="https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" />
  <img src="https://img.shields.io/badge/DAX-0078D4?style=for-the-badge&logo=microsoft&logoColor=white" />
  <img src="https://img.shields.io/badge/Power%20Query-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white" />
  <img src="https://img.shields.io/badge/Status-Concluído-brightgreen?style=for-the-badge" />
</p>

Análise completa do desempenho comercial de uma empresa de eletrônicos, com foco em lucratividade, categorias de produtos, performance de vendedores e evolução de receita ao longo do tempo.

🔗 Acessar Dashboard ao Vivo: https://app.powerbi.com/view?r=eyJrIjoiYmJlNTZmZmMtZjE5OS00MTFmLTk0YzYtMzg2MDc2MmYwYjg3IiwidCI6IjdiNzZjYWM5LTBkYTQtNGNmZC1hZWY1LWEyNDgyNDI5NmYyMiJ9

🎯 Objetivo
Centralizar os principais indicadores de vendas de uma empresa do setor de eletrônicos em um único painel interativo, permitindo que gestores acompanhem o desempenho em tempo real, identifiquem as categorias mais lucrativas e tomem decisões baseadas em dados.

📌 Principais KPIs
IndicadorValor💰 Receita TotalR$ 114,59 milhões📈 Lucro TotalR$ 21,98 milhões🎯 Margem de Lucro19,18%🛒 Ticket MédioR$ 3.540,00🏆 Categoria LíderNotebooks🥇 Melhor VendedorDiego Santos📦 Produto Mais VendidoMonitor LG 27" 4K

📋 Visões e Análises do Painel
🏷️ Lucratividade por Categoria
Comparativo visual entre as categorias de produtos (Notebooks, Monitores, Smartphones, Acessórios, etc.), ordenadas por contribuição ao lucro total. Permite identificar rapidamente onde concentrar esforços comerciais.
📅 Evolução da Receita Mensal
Gráfico de linha com a evolução da receita mês a mês, facilitando a identificação de sazonalidades, picos de vendas e quedas de desempenho ao longo do ano.
👤 Ranking de Vendedores
Visão comparativa entre os vendedores da equipe, com destaque para o top performer e a distribuição de resultado entre os membros do time.
📦 Produtos em Destaque
Lista dos produtos mais vendidos em volume e receita, auxiliando decisões de estoque, mix de produtos e campanhas promocionais.
🔎 Filtros Interativos
O painel conta com filtros dinâmicos por ano e categoria, permitindo análises segmentadas e comparações entre períodos.

🧠 Metodologia
Coleta e Tratamento dos Dados

Dados importados e tratados via Power Query
Limpeza de inconsistências, padronização de nomes e categorias
Criação de tabela calendário para análises temporais

Modelagem

Modelo estrela (Star Schema) com tabela fato de vendas e dimensões de produto, vendedor, categoria e tempo
Relacionamentos otimizados para performance nas consultas DAX

Métricas DAX criadas
daxLucro Total = SUMX(Vendas, Vendas[Receita] - Vendas[Custo])

Margem de Lucro % = DIVIDE([Lucro Total], [Receita Total])

Ticket Médio = DIVIDE([Receita Total], COUNTROWS(Vendas))

Receita Total = SUM(Vendas[Receita])

💡 Principais Insights

Notebooks lideram em lucro absoluto, mas categorias como Monitores apresentam margens percentuais competitivas
O ticket médio de R$ 3,54 mil reflete um portfólio de produtos de médio-alto valor agregado
A receita apresenta variações mensais que indicam sazonalidade, especialmente em períodos como Black Friday e início de ano letivo
Diego Santos se destaca consistentemente como o melhor vendedor, sendo um benchmark interno para a equipe


🛠️ Ferramentas Utilizadas
FerramentaUsoPower BI DesktopConstrução do dashboard e visualizaçõesPower QueryETL e tratamento dos dadosDAXCriação de medidas e KPIs calculadosExcelBase de dados fonte
