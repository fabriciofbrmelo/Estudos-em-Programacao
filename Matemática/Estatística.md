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

# Curso Unesp

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
