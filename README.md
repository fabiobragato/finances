# finances
The use of S3 of AWS and other tecniques to extract data from financial statements of brazillian companies, stock prices and other things that's useful in finances.

Work did in the conclusion of accountant course of Faculdade de Economia, Administração e Contabilidade de Ribeirão Preto, Universidade de São Paulo.

Active funcions:

---------------------- Commands ------------------------ 

---------------------- Reports from AWS ----------------------

buscar_relatorio(conta, ano, trimestre): 
- Purpose: find data from financial statements of brazillian financial conglomerates. 
- First Parameter: required report (ativo, passivo, DRE) - (Assets, Liabilities or Income Statement). 
- Second Parameter: year, ex: 2020. 
- Third Parameter: quarter, ex: 1. 

buscar_relatorios(conta, ano_inicial, trimestre_inicial, ano_final, trimestre_final): 
- Purpose: find data from financial statements of brazillian financial conglomerates at the given interval. 
- First Parameter: required report (ativo, passivo, DRE) - (Assets, Liabilities or Income Statement). 
- Second Parameter: initial year, ex: 2019. 
- Third Parameter: quarter, ex: 1. 
- Forth Parameter: final year, ex: 2020. 
- Fifth Parameter: quarter, ex: 2. 

ultimo_relatorio_disponivel(conta): 
- Purpose: bring the last available report. 
- Parâmetro (conta): required report (ativo, passivo, DRE) - (Assets, Liabilities or Income Statement).

---------------------- Reports via Web Scraping ----------------------

buscar_balancetes(safra_inicial, safra_final): 
- Purpose: find data of balance sheet from financial institutions disclosed by Bacen. 
- First Parameter: initial harvest, ex: 202001. 
- Second Parameter: final harvest, ex: 202004. 

---------------------- Reports from Yahoo Finance ----------------------

dados_acoes_yahoo(tickers, data_inicial, data_final, tipo): 
- Purpose: historic from stock prices. 
- First Parameter stock code. ex: MGLU3.SA. 
- Second Parameter: initial date in the format "yyyy-mm-dd", ex: "2020-01-01". 
- Third Parameter: final date in the format "yyyy-mm-dd", ex: "2020-02-10". 
- Forth Parameter: type of report ("G", "F", "C", "H", "L", "O" ou "V"), which: 
        G: Geral
        F: Adjusted Close Prices
        C: Close Prices
        H: High Prices 
        L: Minimun Prices
        O: Open Prices 
        V: Negociation Volumn

plotar_grafico_fechamentos(tickers, data_inicial, data_final): 
- Purpose: plota o gráfico de fechamento das ações selecionadas na base 100. 
- First Parameter stock code. ex: MGLU3.SA. 
- Second Parameter: initial date in the format "yyyy-mm-dd", ex: "2020-01-01". 
- Third Parameter: final date in the format "yyyy-mm-dd", ex: "2020-02-10". 

retornos_simples(tickers, data_inicial, data_final): 
- Purpose: traz em formato de tabela os retornos simples das ações selecionadas. 
- First Parameter stock code. ex: MGLU3.SA. 
- Second Parameter: initial date in the format "yyyy-mm-dd", ex: "2020-01-01". 
- Third Parameter: final date in the format "yyyy-mm-dd", ex: "2020-02-10". 

retornos_log(tickers, data_inicial, data_final): 
- Purpose: bring in a table format the simple returns of selected stocks. 
- First Parameter stock code. ex: MGLU3.SA. 
- Second Parameter: initial date in the format "yyyy-mm-dd", ex: "2020-01-01". 
- Third Parameter: final date in the format "yyyy-mm-dd", ex: "2020-02-10". 

---------------------- Help ------------------------

ajuda(): 
- Purpose: show all commands and how to work with them. 

periodos_disponiveis(): 
- Purpose: show all available AWS reports. 

---------------------- Contact ------------------------ 

For more information, questions or suggestions please contact: 
- fabio_bragato@hotmail.com 
- fabio.bragato.carmo@usp.br
