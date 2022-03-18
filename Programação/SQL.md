# SQL

Banco de Dados Relacional

Registros --> Tabelas --> Arquivos

Arquivos Sequenciais

Disco (disquete) --> tabelas, índices, numerações = armazenamento indexado (Arquivo de Acesso Direto)

Como armazenar dados de forma mais segura e eficiente?
Surge o COBOL (linguagem antiga da programação)
Surge o Banco de Dados

Banco de Dados:
1. Base de Dados
2. Sistema Gerenciador de Banco de Dados (SGDB)
3. Linguagem de Exploração
4. Programas Adicionais

IBM criou o PC
- criou dados hierárquicos (Modelo Hierárquico)
- Modelo em Rede
- Modelo Relacional --> MySQL

Structured English Query Language (SEQUEL) --> Structured Query Language (SQL)
Linguagem de Consulta, dar comandos aos dados e ele te volta uma query.

Vários SQL --> Padronização do SQL
Bancos de Dados: Oracle, IBM, SQL Server
Bancos de Dados Gratuitos: MySQL, MariaDB

Para usar o MySQL precisa de um WAMP Server (Windows, Apache, MySQL, PHP)

Banco de Dados --> Tabelas --> Registros

Tipos Primitivos --> Tipos de dados para serem cadastrados em tabelas

I. Numérico
1. Inteiro
- TinyInt
- SmallInt
- Int
- MediumInt
- BigInt
2. Real
- Decimal
- Float
- Double
- Real
3. Lógico
- Bit
- Boolean

II. Data/Tempo
- Date
- DateTime
- TimeStamp
- Time
- Year

III. Literal
1. Caractere
- Char
- VarChar
2. Texto
- TinyText
- Text
- MediumText
- LongText
3. Binário
- TinyBlob
- Blob
- MediumBlob
- LongBlob
4. Coleção
- Enum
- Set

IV. Espacial
- Geometry
- Point
- Polygon
- MultiPolygon

DDL (Data Definition Language) --> create database, create table, alter table, drop table

DML (Data Manipulation Language) --> insert into, update, delete, truncate, select

DQL (Data Query Language) --> seletc (pode ser DML ou DQL)

- Manipular registros --> manipular linhas/tuplas

Obtendo dados das tabelas --> SELECT

select * from tabela --> * = todas as colunas
order by coluna asc; --> ascendente
order by coluna desc; --> descendente


select (coluna, coluna, coluna) from tabela --> (coloquei em parenteses para o comando não ser executado, no sql não precisa)
select nome, descricao, ano from cursos

where ano (<=) '2015'

order by ano, nome;
- (<) menor
- (<=) menor igual
- (>) maior
- (>=) maior igual
- (!=) diferente
- (<>) diferente

select (coluna, coluna, coluna) from tabela
- select nome, ano from cursos
- where ano between '2014' and '2016'

select nome, descricao, ano from cursos
- where ano in (2014, 2016, 2018)
- order by ano

Combinando testes:
- select * from cursos
- where carga > 35 and totaulas < 30;

- select * from cursos
- where carga > 35 or totaulas < 30;

Operador Like

- select * from cursos
- where nome like 'P%'; --> todos que começam com P (p minúsculo/maíusculo, não faz diferença)
- where nome like '%P'; --> todos que terminam com P
- where nome like '%p%'; --> qualquer nome que tenha a letra p, não importa a posição
- where nome not like '%p%'; --> p em lugar nenhum
- where nome like 'PH%P' --> qualquer um que começa com ph e termina com p
- where nome like 'PH$P_' --> underline significa um único caractere
- where nome like 'p_p%'; --> começa com p, tem um caractere, de novo um p, qualquer coisa após

- select * from gafanhotos
- where nome like '%silva%'; --> qualquer pessoas que tenha o nome silva em qualquer lugar (só que aqui pega até silvana, por exemplo)
- where nome like '%_silva%' --> underline serve como espaço, então quem tem silvana não entra

Distinguindo

select nacionalidade from gafanhotos
select distinct nacionalidade from gafanhotos --> agrupa as nacionalidades iguais

Agregação
