# Dashboard Financeiro Corporativo

Este repositório apresenta um dashboard desenvolvido no Power BI para análise de movimentações financeiras por centro de custo e setor. O objetivo é facilitar a visualização e interpretação dos dados financeiros, permitindo a identificação de padrões, controle de despesas e suporte à tomada de decisões estratégicas.

<h3>Demonstração</h3>

<p>
  <img src="./assets/Dashboard Financeiro.gif" alt="Demonstração do Dashboard" width="800"/>
</p>


## Visão Geral do Projeto

O projeto realiza a consolidação e tratamento de diversas planilhas de relatórios financeiros, agrupando e relacionando as informações por setor, tipo de despesa e período.

### Fontes de Dados Utilizadas

- **Setores.xlsx**  
  Contém o mapeamento entre centro de custo e setor da empresa.

  | Centro de Custo | Setor            |
  |------------------|------------------|
  | 100901           | Logística        |
  | 100902           | Recursos Humanos |
  | 100903           | Comercial        |
  | 100904           | Compras          |
  | 100905           | Marketing        |

- **Extratos (pasta)**  
  Arquivos no formato `Relatório CC XXXXX Pn.xlsx`, com colunas como:
  - Data
  - Conta contábil
  - Tipo de movimentação
  - Classificação da despesa
  - Documento fiscal
  - Centro de custo
  - Status do pagamento
  - Valor
  - Saldo

## Recursos do Dashboard

- Total de despesas por setor e centro de custo
- Classificação das despesas por tipo
- Análise temporal das movimentações
- Indicadores de valores totais e saldos acumulados
- Segmentações dinâmicas por data, status, setor e tipo de despesa

## Tecnologias Utilizadas

- Power BI Desktop
- Power Query (ETL)
- DAX (Data Analysis Expressions)
- Gráficos nativos: linhas, barras, matriz, cartões

## Estrutura de Tratamento de Dados

A consolidação dos relatórios de diferentes centros de custo é feita automaticamente no Power BI através de parâmetros e funções personalizadas no Power Query, o que permite atualizar o modelo apenas adicionando novos arquivos à pasta `Extratos`.

## Demonstração

O dashboard financeiro foi desenvolvido para oferecer uma visão consolidada das receitas, despesas e saldos por centro de custo. Ele permite ao usuário acompanhar com clareza a saúde financeira de diferentes setores da organização.

Na parte superior do painel, são exibidos **indicadores-chave** como:

- Total de receitas
- Total de despesas
- Saldo consolidado
- Comparativo entre valor orçado e realizado (quando aplicável)

O painel conta também com:

- **Gráfico de barras** com as despesas agrupadas por categoria (ex: administrativas, serviços, impostos)
- **Gráfico de linha** ou de colunas com a evolução mensal dos gastos e receitas
- **Tabela dinâmica** com detalhamento por centro de custo, permitindo visualizar valores e categorias por setor
- **Segmentações interativas** que filtram os dados por período, tipo de movimentação, status e centro de custo

Todos os elementos do dashboard são interativos: ao clicar em um centro de custo específico, por exemplo, o painel inteiro é filtrado para exibir apenas os dados daquele setor.


<p>
  <img src="./assets/Dashboard Financeiro.gif" alt="Demonstração do Dashboard" width="500"/>
</p>
