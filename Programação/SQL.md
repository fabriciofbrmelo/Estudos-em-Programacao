# SQL

### Para que serve e o que é o SQL?
1. Banco de Dados Relacional
2. Registros --> Tabelas --> Arquivos
3. Arquivos Sequenciais

- Disco (disquete) --> tabelas, índices, numerações = armazenamento indexado (Arquivo de Acesso Direto)

### Como armazenar dados de forma mais segura e eficiente?
- Surge o COBOL (linguagem antiga da programação)
- Surge o Banco de Dados

## Banco de Dados:
1. Base de Dados
2. Sistema Gerenciador de Banco de Dados (SGDB)
3. Linguagem de Exploração
4. Programas Adicionais

IBM criou o PC
- criou dados hierárquicos (Modelo Hierárquico)
- Modelo em Rede
- Modelo Relacional --> MySQL

Structured English Query Language (SEQUEL) --> Structured Query Language (SQL)
- Linguagem de Consulta, dar comandos aos dados e ele te volta uma query.

Vários SQL --> Padronização do SQL
1. Bancos de Dados: Oracle, IBM, SQL Server
2. Bancos de Dados Gratuitos: MySQL, MariaDB

## Para usar o MySQL precisa de um WAMP Server (Windows, Apache, MySQL, PHP)

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

## SQL

1. DDL (Data Definition Language) --> create database, create table, alter table, drop table
2. DML (Data Manipulation Language) --> insert into, update, delete, truncate, select
3. DQL (Data Query Language) --> seletc (pode ser DML ou DQL)

- Manipular registros --> manipular linhas/tuplas

## SELECT

1. Obtendo dados das tabelas --> SELECT

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

2. Combinando testes:
- select * from cursos
- where carga > 35 and totaulas < 30;

- select * from cursos
- where carga > 35 or totaulas < 30;

3. Operador Like

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

4. Distinguindo

- select nacionalidade from gafanhotos
- select distinct nacionalidade from gafanhotos --> agrupa as nacionalidades iguais

5. Agregação

- select count(*) from cursos; --> Conta quantos cursos tem na tabela;
- select count(*) from cursos where carga > 40; --> Conta quantos cursos com carga maior que 40;
- select * from cursos order by carga; --> mostra os cursos ordenados por carga
- select max(carga) from cursos; --> qual a maior carga
- select max(totaulas) from cursos where ano ='2016'; --> dentre os cursos de 2016, qual o maximo de aulas?
- select nome, max(totaulas) from cursos where ano ='2016'; ---> qual o curso de 2016 com o maximo de aulas?
- select min(totaulas) from cursos where ano ='2016'; --> dentre os cursos de 2016, qual o mínimo de aulas?
- select nome, min(totaulas) from cursos where ano ='2016'; ---> qual o curso de 2016 com o mínimo de aulas?
- select sum(totaulas) from cursos where ano ='2016'; --> somar a carga horária de todos os cursos
- select avg(totaulas) from cursos where ano ='2016'; --> média carga horária de todos os cursos

6. Distinguindo e Agregando
i. Distinguindo --> SELECT DISTINCT from cursos order by carga;
- seleciona todos os cursos com cargas horárias iguais e coloca na coluna os cursos de carga 10, 20, 40, 60 --> não fala quantos cursos tem 40 horas, fala só a carga horária
ii. Agrupando --> para saber quantos cursos tem 20, 40, 60
- SELECT carga from cursos group by carga;

- SELECT carga, COUNT(nome) from cursos group by carga;

- select totaulas, count(*) from cursos group by totaulas order by totaulas;

- select ano, count(*) from cursos group by ano having count(ano) >= 5 order by count(*);

--> where é diferente de having, having só usa na hora de agrupar

### Exercícios

1. Uma lista com a profissão dos gafanhotos e seu quantitativo
- select * from gafanhotos;

- select profissao from gafanhotos group by profissao;

- select profissao, count(*) from gafanhotos group by profissao;

2. Quantos gafanhotos homens e mulheres nasceram após 01/jan/2005
- select * from gafanhotos;

- select * from gafanhotos where sexo = 'M';
- select * from gafanhotos where sexo = 'F';

- select sexo from gafanhotos group by sexo;

- select sexo, count(*) from gafanhotos group by sexo;

- select sexo, count(nome) from gafanhotos group by sexo;

- select sexo, count(nome) from gafanhotos group by sexo order by sexo;

- select sexo, count(*) from gafanhotos where nascimento > '2005-01-01' group by sexo;

3. Lista com gafanhotos que nasceram fora do BRASIL, mostrando o país de origem e o total de pessoas nascidas lá. Só nos interessam os países que tiveram mais de 3 gafanhotos com essa nacionalidade
- select nacionalidade,count(*)from gafanhotos  where nacionalidade <> 'brasil' group by nacionalidade having count(nacionalidade ) >'3';

4. uma lista agrupada pela altura dos gafanhotos ,mostrando quantas pessoas  pesam mais de 100kg e que estao acima da media da altura de todos os gafanhotos
- select altura, count(*) from gafanhotos where peso > '100' group by altura having altura > (select avg(altura) from gafanhotos);

## DER - DIAGRAMA ENTIDADE RELACIONAMENTO

Conectar a tabela gafanhotos com a tabela cursos --> um gafanhoto pode fazer um curso
cardinalidade --> 1 gafanhoto assiste n cursos ou 1 curso é assistido por n gafanhotos

muitos-para-muitos --> vários gafanhotos assistem vários cursos
um-para-um --> uma pessoa casa com uma outra pessoa
um-para-muitos --> um funcionário cuida de n pessoas ou n pessoas são cuidadas por 1 funcionário

chava primária e chave estrangeira
--> a chave estrangeira é a chave primária que veio de outro lugar
