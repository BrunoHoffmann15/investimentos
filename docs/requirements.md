# Requisitos

1. Cadastro manual de títulos de renda fixa.

Como um usuário,
Eu quero adicionar manualmente os títulos de investimento de renda fixa que possuo,
Para que eu possa ter um controle personalizado e detalhado dos meus investimentos.

Critérios de aceitação:
- O sistema deve permitir o cadastro de informações como nome do título, valor investido, data de compra, taxa de juros, vencimento, etc.
- O sistema deve possibilitar adicionar uma tabela de imposto de renda para eu pagar.
  - A tabela de imposto será dada com base na tabela regressiva de imposto de renda.
- O sistema deve validar se todos os campos obrigatórios estão preenchidos antes de salvar.
- O sistema deve mostrar uma mensagem de confirmação quando o título for adicionado com sucesso.

2. Visualização de títulos de renda fixa.

Como um usuário,
Eu quero visualizar uma lista de todos os meus títulos de investimento,
Para que eu possa ver facilmente o status dos meus investimentos.

Critérios de aceitação:
- O sistema deve exibir uma tabela/lista com todos os títulos cadastrados.
- O sistema deve permitir ordenar e filtrar os títulos por diferentes critérios, como data de compra, valor, vencimento, etc.
- O sistema deve me mostrar o quanto eu receberia se resgatasse o dinheiro agora.
  - Considerando as taxas que precisam ser aplicadas e fazendo os cálculos do valor.
  - Considerando o valor de juros até o momento.

3. Importação de arquivo .csv de dados de renda fixa

Como um usuário,
Eu quero importar um arquivo .csv contendo os dados dos meus investimentos,
Para que eu possa adicionar vários títulos de uma vez sem precisar cadastrá-los manualmente.

Critérios de aceitação:
- O sistema deve aceitar arquivos no formato .csv.
- O sistema deve validar o conteúdo do arquivo, garantindo que todas as colunas necessárias estejam presentes e preenchidas.
- O sistema deve exibir uma pré-visualização dos dados antes de importá-los definitivamente.
- O sistema deve mostrar uma mensagem de erro caso o arquivo esteja em formato incorreto ou com dados inválidos.
- Os dados devem seguir o formato:
  - Indexação;
  - Taxa de Juros (Se tiver);
  - Nome do título;
  - Data Vencimento;
  - Data de Regaste;
  - Data da Compra;
  - Tabela de Taxação;
  - Típo de título;

4. Cadastro manual de investimentos em renda variável

Como um usuário,
Eu quero adicionar manualmente ações e outros investimentos de renda variável,
Para que eu possa gerenciar todos os meus ativos no sistema.

Critérios de aceitação:
- O sistema deve permitir o cadastro de informações como nome da ação ou fundo, quantidade de ativos, preço de compra, data de compra, e corretagem.
- O sistema deve verificar se o título já foi comprado anteriormente.
- O sistema deve validar se todos os campos obrigatórios estão preenchidos antes de salvar.
- O sistema deve calcular automaticamente o valor investido com base na quantidade de ativos e no preço de compra.
- Deve haver suporte para diferentes tipos de ativos, como ações, FIIs, ETFs, entre outros.

5. Cadastro de Teses de investimentos em renda variável

Como um usuário,
Eu quero poder adicionar uma tese de investimentos nos meus títulos de renda variável,
Para que eu possa acompanhar se meu título está ou não na hora de compras ou vender.

Critérios de aceitação:
- O sistema deve me permitir adicionar tese pode seguir diferentes estratégias;
  - Método do P/L (Preço/Lucro)
  - Método de Fluxo de Caixa Descontado (DCF)
  - Método do P/VPA (Preço/Valor Patrimonial por Ação)
  - Dividend Discount Model (DDM)
  - Análise de Múltiplos (Comparação com empresas semelhantes)
- O sistema deve manter um status da minha última tese.
- O sistema deve permitir adicionar campos como:
  - Data da Tese;
  - Preço Justo;
  - Preço Teto;
  - Hipóteses;

6. Atualização automática de preços de ações

Como um usuário,
Eu quero que o sistema atualize automaticamente os preços das minhas ações e fundos imobiliários,
Para que eu tenha sempre o valor atualizado dos meus investimentos.

Critérios de aceitação:
- O sistema deve integrar-se com uma API de mercado financeiro (como Alpha Vantage ou Yahoo Finance) para obter os preços mais recentes.
- O sistema deve exibir o valor atual de cada ativo e o valor total da carteira com base nos preços de mercado.
- O sistema deve atualizar os preços de acordo com um intervalo de tempo configurável (ex.: a cada 5 minutos ou ao abrir o dashboard).

7. Visualização e acompanhamento de carteira

Como um usuário,
Eu quero visualizar o desempenho da minha carteira de investimentos em renda variável ao longo do tempo,
Para que eu possa acompanhar o crescimento ou queda dos meus ativos.

Critérios de aceitação:
- O sistema deve exibir gráficos com o histórico de desempenho da carteira, incluindo valor investido, valor atual e variação percentual.
- O usuário deve poder filtrar os gráficos por período (últimos 7 dias, 30 dias, 1 ano, etc.).
- O sistema deve exibir informações sobre dividendos recebidos (caso aplicável).

8. Cadastro de Títulos de renda variável

Como um usuário,
Eu quero poder cadastrar manualmente um título de renda variável,
Para que eu possa reaproveitar ele na hora de cadastrar meus títulos comprados ou vendidos.

Critérios de Aceite:
- O sistema deve permitir eu adicionar um título indicando: ticker, data de criação, ramo de atuação, país de origem, sub-ramo de atuação.
- O sistema deve permitir eu adicionar uma tese de investimento para ticker.
  - A partir disso consigo associar a tese ao ticker.