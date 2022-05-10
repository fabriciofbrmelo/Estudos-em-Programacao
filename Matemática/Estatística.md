# Estatística

|Elementar|Básico|Intermediário|Avançado|
|-|-|-|-|
|Estatística Descritiva|Dados Observáveis|Modelo de Probabilidade - Sigmas Álgebras|Teoria da Medida|
|Dados Concretos|Modelo de Probabilidade Reduzido|Variáveis Aleatórias - Funções Mensuráveis|Problema da Medida|
|Tabelas e Gráficos Simples|Variáveis Aleatórias|Convergências: Probabilidade, Distribuição Quase Certa|Teorema da Extensão de Carathéodory|
|Medidas de Resumo: Média, Mediana, Desvio Padrão, Variância, Primeiro e Terceiro Quartil|Probabilidades Condicionais|Desigualdades de Markov, Tchebycheff, Kolongorov e Bernstein|Teorema da Extensão de Kolmogorov|
||Independência|Teorema do Limite Central|Derivada de Radon-Nikodyn|
||Esperanças Matemáticas|Análise Multivariada|Teoremas do Limite Central|
||Teorema do Limite Central|Modelos Lineares Generalizados|Sequências Marginais|
||Intervalos de Confiança|Modelos Não-Lineares|Desigualdades|
||Testes para Média e Proporção|Modelos Mistos|Convergência|
||Modelos Lineares|Modelos Aditivos Generalizados|Espaços Abstratos e Métricas Não-Triviais|
|||Séries Temporais|Modelos Estatísticos - Famílias de Probabilidade|
||||Estimadores - Estatísticas Suficientes, Completas e Ancilares|


## Medidas de Tendência Central
- [x] Média Aritmética Simples
- [x] Média Geométrica
- [x] Média Harmônica
- [x] Moda
- [x] Mediana
- [x] Desvio Médio
- [x] Variância
- [x] Desvio Padrão

## Probabilidade
- [x] Probabilidade Complementar
- [x] Análise Combinatória
- Permutação
- Permutação com Repetição
- Combinação
- Combinação com Repetição
- Arranjo

## Conjuntos Numéricos
- [x] Conjunto das Partes
- [x] Complementar
- [x] Intervalos do conjunto
- Conjunto Fechado
- Conjunto Aberto
- [x] Intersecção e União
- [x] Diferença e Complementar de Conjunto
- [x] Operações com Intervalos

## Tipos de Dados
- [x] Qualitativos
- [x] Quantitativos
- [x] Modelos
- [x] Diferença de Média e Mediana
- [x] Gráficos
- [x] Frequência

## Quantis, Quartis e Percentis
- [x] Quantis
- [x] Quartis
- [x] Percentis
- [x] Medidas de Dispersão
- [x] Boxplot
- [x] Dados Agrupados e Não-Agrupados

# Curso Univesp

#### **Probabilidade** --> estudo da aleatoriedade e incerteza; método para quantificação das chances.

### Fenômeno Determinístico / Probabilístico
1. Determinístico: o resultado é sempre o mesmo (a CHUVA sempre CAI)
2. Probabilístico: o resultado é incerto / variável

> Probabilidade: medida da informação sobre a ocorrência de um evento
>
> Estatística: baseia-se no estudo dos fenômenos probabilísticos

|Fenômenos Aleatórios|Experimento Aleatório|
|-|-|
|Diferentes Resultados|Possíveis Resultados são conhecidos (**PROBABILIDADE**)|
|Mesmo em condições iguais, o resultado é imprevisível|Resultado final é desconhecido até o final|
|- Lançamento de Moedas - Dados - Carta de Baralho - Vida útil de um PC|Pode ser repetido sob as mesmas condições|
||Quando for repetido um grande número de vezes e houver regularidade, é possível estruturar um modelo matemático probabilístico|

```
P = lim m/n
n --> ∞

m = sucessos
n = n.º de experimentos
```

## Espaço Amostral (S)

Conjunto --> Coleção definida de objetos ou itens
Espaço Amostral --> é o CONJUNTO de todos os possíveis resultados desse experimento

|Espaço Amostral do Lançamento de uma MOEDA|Espaço amostral do Lançamento de DUAS MOEDAS|Espaço Amostral do Lançamento de um DADO|
|-|-|-|
|Cara(C)|Cara(C) - Cara(C)|1, 2|
|Coroa(K)|Cara(C) - Coroa(K)|3, 4|
||Coroa(K) - Cara(C)|5, 6|
||Coroa(K) - Coroa(K)||
|S = {C, K}|S = {(C, C), (C, K), (K, C), (K, K)}|S = {1, 2, 3, 4, 5, 6}|

## Evento Aleatório (E)

- Qualquer subconjunto de um ESPAÇO AMOSTRAL (S)
- Resultado possível em experimentos aleatórios e que não é previsível

||Lançamento de Moeda|Lançamento de Dado|Lançamento de Duas Moedas|
|-|-|-|-|
|Espaço Amostral|S = {C, K}|S = {1, 2, 3, 4, 5, 6}|S = {(C, K), (C, C), (K, C), (K, K)}|
|Evento Aleatório|E = C|E = 3|E = (K, K)|
|Probabilidade de E|P(E) = 1/2|P(E) = 1/6|P(E) = 1/4|

```
Probabilidade de um Evento Aleatório (E)
0 =< P(E) =< 1
0% =< P(E) =< 100%
```

## Evento Complementar

```
A = Evento Aleatório
A' = Evento Complementar = Caso A não aconteça
```
![EVENTO COMPLEMENTAR](https://user-images.githubusercontent.com/87718178/166807248-0996e712-193b-457c-9aad-e4a9dc24d28d.jpg)

## Evento Equiprovável

```
Cada ponto tem a mesma probabilidade
P(1) = P(2) = P(3)
```

## Evento Mutuamente Excludente

```
Se acontecer A, não acontece B
Se acontecer B, não acontece A
```
![evento mutuamente excludente](https://user-images.githubusercontent.com/87718178/166808040-12859b40-68e2-4cd9-803e-f7f3242c3623.jpg)

## Operações entre Eventos

### União (ou) - A U B

```
Pelo menos um dos eventos
A ou B ou AMBOS
```
![união](https://user-images.githubusercontent.com/87718178/166809902-b95ba6ff-57c7-49df-9092-d5a85a611b09.jpg)


### Intersecção (e) - A ∩ B

```
Pontos que pertencem simultaneamente a A e B
Só se A e B ocorrer
```
![intersecção](https://user-images.githubusercontent.com/87718178/166809924-c234c14b-09ef-4e06-bb28-7a55dcc4a2c8.jpg)

## Axiomas de Probabilidade

```
Em um Evento Mutuamente Excludente P (A ∩ B) = 0 é impossível ter Intersecção
Se Ø é o Conjunto Vazio, então P(Ø) = 0
```
![evento mutuamente excludente](https://user-images.githubusercontent.com/87718178/166810151-e23f89fb-0804-4ca5-a862-b1d5abb8bf4b.jpg)

```
Teorema do Evento Complementar
Se A' é o complemento do Evento A, então P(A')= 1 - P(A)
```
![EVENTO COMPLEMENTAR](https://user-images.githubusercontent.com/87718178/166807248-0996e712-193b-457c-9aad-e4a9dc24d28d.jpg)

```
Teorema da Soma
P (A U B) = P(A) + P(B) - P(A ∩ B)
```
![união](https://user-images.githubusercontent.com/87718178/166809902-b95ba6ff-57c7-49df-9092-d5a85a611b09.jpg)

```
Se A e B são mutuamente exlucdentes
P (A U B) = P(A) + P(B)
```
![evento mutuamente excludente](https://user-images.githubusercontent.com/87718178/166808040-12859b40-68e2-4cd9-803e-f7f3242c3623.jpg)

```
P(A U B U C) = P(A) + P(B) + P(C) - P(A ∩ B) - P(A ∩ C) - P(B ∩ C) + P(A ∩ B ∩ C)
```
![3](https://user-images.githubusercontent.com/87718178/166813247-4145d922-fb93-428b-9a29-8d61b3ad1c5b.jpg)

## Exercício - Cartas de Baralho

|Espaço Amostral(S)||
|-|-|
|Espadas ♠|A 2 3 4 5 6 7 8 9 10 J Q K|
|Paus ♣|A 2 3 4 5 6 7 8 9 10 J Q K|
|Copas ♥|A 2 3 4 5 6 7 8 9 10 J Q K|
|Ouro ♦|A 2 3 4 5 6 7 8 9 10 J Q K|
```
Cartas de Baralho: 52
a) Chance de Copas?
b) Chance de Figura?
c) Chande de Figura de Copas?
d) Chance de Figura ou Copas?
```
```
a) Chance de Copas
P(A)= M/N = 13/52 = 1/4
```
```
b) Chance de ser Figura
P(B)= M/N = 12/52 = 3/13
```
```
c) Chance de ser Figura de Copas (intersecção)
P(C)= M/N = 3/52
```
|Espaço Amostral(S)|Intersecção|
|-|-|
|Espadas ♠||
|Paus ♣||
|Copas ♥|J Q K|
|Ouro ♦||

```
d) Chance de ser Figura ou Copas (união)
P(D)= M/N = (9 + 3 + 10) / 52 = 22/52
ou
P(A U B) = P(A) + P(B) - P(A ∩ B)
P(A U B) = 13 + 12 - 3
P(A U B) = 22
```
|Espaço Amostral(S)||
|-|-|
|Espadas ♠|J Q K|
|Paus ♣|J Q K|
|Copas ♥|A 2 3 4 5 6 7 8 9 10 J Q K|
|Ouro ♦|J Q K|

> J Q K aparece duas vezes, uma vez como figura outra como copas, por isso exclui a intersecção

## Exercício - Quatro Moedas

|Espaço Amostral (S)|16 possibilidades||||
|:-:|:-:|:-:|:-:|:-:|
|O CARAS|1 CARA|2 CARAS|3 CARAS|4 CARAS|
|KKKK|CKKK|CCKK|CCCK|CCCC|
||KCKK|CKCK|CCKC||
||KKCK|CKKC|CKCC||
||KKKC|KKCC|KCCC||
|||KCKC|||
|||KCCK|||
|1 possibilidade|2 pssibilidades|6 possibilidades|4 possibilidades|1 possibilidade|

```
a) obter n.º par de caras P(A)
b) obter exatamente 3 caras P(B)
c) obter ao menos 2 caras consecutivas P(C)
d) obter 3 caras ou n.º par de caras P(B U A)
e) obter exatamente 3 caras e ao menos 2 caras consecutivas P(B ∩ C)
f) não ocorrer o evento "n.º par de caras e ao menos 2 caras consecutivas" P(B ∩ C')
```
```
a) Obter Número PAR de CARAS
0 caras --> 1 possibilidade
2 caras --> 6 possibilidades
4 caras --> 1 possibilidade

P(A) = M/N
P(A) = 8/16 = 1/2 = 0,5 = 50%
```
```
b) Obter EXATAMENTE 3 CARAS
3 caras --> 4 possibilidades

P(B) = M/N
P(B) = 4/16 = 1/4 = 0,25 = 25%
```
```
c) Obter ao menos 2 CARAS CONSECUTIVAS
2 caras --> 3 em 6
3 caras --> 4 em 4
4 caras --> 1 em 1

P(C) = M/N
P(C) = 8/16 = 1/2 = 0,5 = 50%
```
```
d) Obter 3 CARAS ou n.º PAR de CARAS P(B U A)
P(A U B) = P(A) + P(B) - P(A ∩ B)
P(A U B) = 4/16 + 8/16 - 0
P(A U B) = 12/16 = 3/4 = 0,75 = 75%

P(A ∩ B) = 0, pois não existe intersecção
```
```
e) Obter EXATAMENTE 3 caras e ao menos 2 CARAS CONSECUTIVAS P(B ∩ C)
P(B) = Exatamente 3 caras = 1/4
P(C) = Ao menos 2 caras consecutivas

P(B ∩ C) = M/N = 4/16 = 1/4
```
![e](https://user-images.githubusercontent.com/87718178/166970196-884653c9-5abf-426d-b27c-0fbcee9d434e.jpg)
```
f) Não ocorrer o evento "n.º par de caras e ao menos 2 caras consecutivas" P(B ∩ C')
P(B ∩ C') = 1 - P(B ∩ C)
P(B ∩ C') = 1 - 1/4
P(B ∩ C') = (4 - 1)/4 = 3/4

P = M/N = 12/16 = 3/4
```

## Exercício - Telespectadores de uma Operadora

```
Prédio - 50 habitantes
Canal A: 15 pessoas assistem
Canal B: 10 pessoas assistem
Canal C: 8 pessoas assistem
Canal A e B: 6 pessoas assistem
Canal A e C: 4 pessoas assistem
Canal B e C: 3 pessoas assitem
Canal A, B, C: 1 pessoa assiste
```
![VENN](https://user-images.githubusercontent.com/87718178/166978561-6dda6049-bb47-44c6-9b29-622ac4ea2cec.jpg)
```
Prédio - 50 habitantes
6 + 5 + 2 + 1 + 3 + 2 + 2 = 21
21 pessoas assistem algum canal (21/50)
29 não assistem nada

P(canal) = 21/50 = 0,42 = 42%
P(só 1 canal) = (6 + 2 + 2) / 50 = 10/50 = 1/5 = 0,20 = 20%
```

## Contagem, Combinação e Arranjo

|Evento 1|1 Moeda|2 Resultados Possíveis|
|-|-|-|
|Evento 2|1 Dado|6 Resultados Possíveis|

|2 Eventos em Conjunto: 2x6 = 12 Possibilidades|
|-|
|Evento 1 - m possibilidades|
|Evento 2 - n possibilidades|
|Ambos = m.n possibilidades|

|K,1|K,2|K,3|K,4|K,5|K,6|
|-|-|-|-|-|-|
|C,1|C,2|C,3|C,4|C,5|C,6|

### Problemas Complexos: Combinação ou Arranjo

### Combinação

```
**ORDEM NÃO FAZ DIFERENÇA**

Cn,p = n! / p!(n-p)!

n --> número de elementos do conjunto amostral
p --> número de elementos escolhidos
c --> número de combinações possíveis
```
```
Quantas comissões de 3 pessoas dá para formar com 10 pessoas?

n --> 10 elementos
p --> 3 escolhidos

Cn,p = n! / p!(n-p)!
C10,3 = 10! / 3!(10-3)!
C10,3 = 120
```

### Arranjo

```
**ORDEM FAZ DIFERENÇA**

Ar,p = r! / (r-p)!

r --> número de elementos do conjunto amostral
p --> número de elementos escolhidos
a --> número de arranjos possíveis
```
```
Quantas chapas de 10 pessoas, sendo que precisa ter um Presidente, um Tesoureiro e um Secretário?

r --> 10 elementos
p --> 3 escolhidos

Ar,p = r! / (r-p)!
A10,3 = 10! / (10-3)!
A10,3 = 720
```
