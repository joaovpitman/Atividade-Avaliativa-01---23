# Análise de Dados Históricos de Ações (PETR4)

Este projeto realiza uma análise financeira detalhada de ativos da B3 (Bolsa de Valores do Brasil), com foco inicial na Petrobrás (PETR4.SA). O objetivo é fornecer um script de referência que demonstre todas as etapas de coleta, processamento e visualização de dados do mercado financeiro.

## 🚀 Objetivo
O projeto visa automatizar a análise de desempenho de ações no período de **janeiro de 2023 a maio de 2026**. Além da Petrobrás, a estrutura está preparada para analisar empresas como:
* Vale S.A. (VALE3.SA)
* Ambev S.A. (ABEV3.SA)
* Itaú Unibanco (ITUB4.SA)
* Banco do Brasil (BBAS3.SA)

## 🛠️ Funcionalidades
O código executa as seguintes tarefas para cada empresa selecionada:
1. **Download de Dados:** Extração de dados históricos via biblioteca `yfinance`.
2. **Processamento de Dados:** Exibição de preços de abertura, fechamento, máximas, mínimas e volume.
3. **Análise Estatística:**
    * Cálculo da média anual do preço de fechamento.
    * Cálculo do desvio-padrão anual para medir a volatilidade.
4. **Indicadores de Desempenho:** Cálculo do retorno semestral percentual entre períodos consecutivos.
5. **Visualização:** Geração de gráficos para acompanhamento das tendências.

## 📊 Exemplo de Resultados (PETR4)
Com base na análise realizada, o script gera métricas como:
* **Médias Anuais:** Acompanhamento da valorização (ex: R$ 19.25 em 2023 para R$ 40.98 em 2026).
* **Retornos Semestrais:** Identificação de variações significativas, como o crescimento de +50.63% entre 2025_S2 e 2026_S1.

## 📦 Requisitos
Para rodar este notebook, você precisará das seguintes bibliotecas Python:
* `pandas`
* `yfinance`
* `matplotlib`
* `numpy`

## ✒️ Autor
* **Seu Nome** - [Seu Link do GitHub]
