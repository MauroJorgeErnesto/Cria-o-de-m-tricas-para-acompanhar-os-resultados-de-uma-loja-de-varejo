Contexto
Uma loja de varejo busca criar métricas para acompanhar seus resultados a partir de bases de dados de vendas e clientes. A missão é realizar o tratamento e a união dessas bases para gerar análises e métricas que auxiliem na tomada de decisões estratégicas.

Objetivos
Departamentos mais vendidos: Identificar quais departamentos possuem maior volume de vendas.
Média de preço com frete por departamento: Calcular a média dos preços considerando o frete, agrupados por departamentos.
Quantidade de vendas por mês: Determinar o número de vendas exclusivas realizadas em cada mês.
Média de renda por canal de venda: Avaliar a renda média dos clientes por tipo de canal de venda.
Média de idade por bandeira: Analisar a média de idade dos clientes associados a cada bandeira de pagamento.

Premissas de Negócio
Ausência de Estado: Para compras sem a informação de estado, deve-se preencher com "MS".
Validação de preços: O preço do produto não pode ser maior que o preço com frete.

Passos Realizados no Projeto

Tratamento de Dados:
Substituição de valores nulos na coluna estado com "MS".
Exclusão de registros onde o preço do produto era maior que o preço com frete para garantir a consistência dos dados.

Criação de Métricas:
Departamentos mais vendidos: Contagem de compras exclusivas por departamento.
Média de preço com frete por departamento: Cálculo da média de Preço_com_frete por departamento.

Quantidade de vendas por mês:
Conversão da coluna Data para o tipo datetime.
Extração do mês da data para agrupamento.
Contagem do número de compras únicas por mês.
Média de renda por canal de venda: Cálculo da renda média dos clientes, agrupada por idcanalvenda.
Média de idade por bandeira: Cálculo da idade média dos clientes, agrupada por bandeira.

Visualizações:
Gráficos foram criados para facilitar a análise dos dados:
Gráfico de barras mostrando a média de preço com frete por departamento.
Gráfico de linha representando a quantidade de vendas por data.
Gráfico de barras exibindo a idade média por bandeira de pagamento.
Gráfico de barras mostrando a renda média por canal de venda.

Ferramentas e Tecnologias Utilizadas:

Bibliotecas:
pandas para manipulação de dados.
matplotlib e plotly para criação de visualizações.
Visualização Interativa: Gráficos criados com plotly para análise exploratória.

Resultados
Este projeto resultou em um conjunto de métricas acionáveis que ajudam a empresa a identificar tendências de vendas, avaliar o desempenho de canais e bandeiras, e melhorar suas estratégias de precificação e marketing.

Observações
Os dados utilizados são fictícios e têm como objetivo a demonstração de métodos e ferramentas analíticas. Caso precise de mais informações ou queira incluir análises adicionais, sinta-se à vontade para contribuir!
