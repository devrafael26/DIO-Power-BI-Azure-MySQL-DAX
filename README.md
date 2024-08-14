# Desafios realizados ao longo do Bootcamp Sysvision - Data Analytics com Power BI - DIO

#### - Conectando o Power BI a um Banco de dados MySQL na Azure, tratar o dados, fazer algumas mesclas, agrupar e posteriormente construir um pequeno relatório de RH.
#### - Modelagem Dimensional Star Schema
#### - Criação de tabelas Dimensão e Fato através de uma tabela origem. Utilização de DAX para criar tabelas e colunas.
#####   d_Calendario = CALENDAR(MIN(f_Vendas[Date]), MAX(f_Vendas[Date])) --> para criar a tabela d_Calendario
#####   Day = WEEKDAY('d_Calendario'[Date]) --> para criar a coluna Day
#####   Day of Week = FORMAT('d_Calendario'[Date], "DDDD") --> para criar a coluna Day of Week
#####   Month = MONTH('d_Calendario'[Date]) --> para criar a coluna Month
#####   Year = YEAR('d_Calendario'[Date]) --> para criar a coluna Year

#####   A relação entre as tabelas f_Vendas e d_Calendario, foi feito através das colunas Date de cada tabela envolvida. Ajustou-se o formato da data para o tipo "Short Date" em ambas as tabelas.
#####   As colunas Day, Day of Week, Month e Year, foram criadas como colunas adicionais da tabela d_Calendário, para serem utilizadas em visualizações e análises.
