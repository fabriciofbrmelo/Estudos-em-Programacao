# Python

## Curso em Vídeo com Gustavo Guanabara
- Comandos que estou aprendendo com os vídeos de Gustavo Guanabara

## Módulo 1

### Prazer te conhecer
```
nome = input('Digite seu nome: ')
print('É um prazer te conhecer, {}!'.format(nome))
```

### Soma
```
n1 = int(input('Digite um valor: '))
n2 = int(input('Digite um valor: '))
s = n1 + n2
print('A soma entre', n1, 'e', n2, 'vale', s)
ou
print('A soma entre {} e {} vale {}'.format(n1, n2, s))
```

### Média
```
n1 = float(input('Digite sua primeira nota: '))
n2 = float(input('Digite sua segunda nota: '))
m = (n1+n2)/2
print('A média entre {:.1f} e {:.1f} é {:.2f}'.format(n1, n2, m))
```

### Verificar com var.is
```
a = input('Digite algo: ')
print('O tipo primitivo desse valor é: ', type(a))
print('Só tem espaços? ', a.isspace())
print('É um número? ', a.isnumeric())
print('É alfabético? ', a.isalpha())
print('É alfanumérico? ', a.isalnum())
print('Está em maiúsculas? ', a.isupper())
print('Está em minúsculas? ', a.islower())
print('Está capitalizada? ', a.istitle())
```

### Operadores Aritméticos
```
1 = int(input('Um valor: '))
n2 = int(input('Outro valor: '))
s = n1 + n2
m = n1 * n2
d = n1 / n2
di = n1 // n2
e = n1 ** n2
print('A soma é {}, \n o produto é {} e a \n divisão é {:.3f}'.format(s, m, d), end= '>>>')
print('Divisão inteira {} e potência {}'.format(di, e))
```

### Antecessor e Sucessor
```
n = float(input('Digite um número: '))
print('Analisando o valor {}, seu antecessor é {} e o seu sucessor é {}'.format(n, (n-1), (n+1)))
```

### Dobro e Raiz
```
n = int(input('Digite um número: '))
print('O dobro de {} vale {}.'.format(n, (n*2)))
print('O triplo de {} vale {}. \nA raiz quadrada de {} é {:.2f}'.format(n, (n*3), n, pow(n, (1/2))))
```

### Sistema Métrico
```
medida = float(input('Digite uma distância em metros: '))
km = medida / 1000
hm = medida / 100
dam = medida / 10
dm = medida * 10
cm = medida * 100
mm = medida * 1000
print('A medida de {}m corresponde a \n{}km, \n{}hm, \n{}dam, \n{}dm, \n{}cm, \n{}mm'.format(medida, km, hm, dam, dm, cm, mm))
```

### Tabuada
```
num = int(input('Digite um número para ver sua tabuada: '))
print('-'*12)
print('{} x {:2} = {}'.format(num, 1, num*1))
print('{} x {:2} = {}'.format(num, 2, num*2))
print('{} x {:2} = {}'.format(num, 3, num*3))
print('{} x {:2} = {}'.format(num, 4, num*4))
print('{} x {:2} = {}'.format(num, 5, num*5))
print('{} x {:2} = {}'.format(num, 6, num*6))
print('{} x {:2} = {}'.format(num, 7, num*7))
print('{} x {:2} = {}'.format(num, 8, num*8))
print('{} x {:2} = {}'.format(num, 9, num*9))
print('{} x {:2} = {}'.format(num, 10, num*10))
print('_'*12)
```

### Conversor
```
real = float(input('Quanto dinheiro você tem na carteira? R$ '))
dolar = real / 3.27
euro = real / 5.25
print('Com R${:.2f} você pode comprar US${:.2f} ou £${:.2f}'.format(real, dolar, euro       ))
```

### Largura Parede
```
larg = float(input('Largura da parede: '))
alt = float(input('Altura da parede: '))
area = larg * alt
print('Sua parede tem a dimensão de {:.1f}x{:.1f} e sua área é de {:.1f}m2'.format(larg, alt, area))
tinta = area / 2
print('Para pintar essa parede você precisará de {}l de tinta'.format(tinta))
```

### Desconto
```
preco = float(input('Qual o preço do produto? R$ '))
novo = preco - (preco * 5 / 100)
print('O produto que custava R$ {:.2f}, na promoção com desconto de 5% vai custar R$ {:.2f}'.format(preco, novo))
```

### Salário
```
sal = float(input('Qual o salário do funcionário? R$ '))
novo = sal + (sal * 15 / 100)
print('O salário do funcionário era R$ {:.2f} e com aumento de 15% ele passará a receber R$ {:.2f}'.format(sal, novo))
```

### Temperatura
```
celsius = float(input('Qual a temperatura em graus celsius? ºC: ' ))
farenheit = ((9 * celsius) / 5) + 32
print('A temperatura de {}ºC corresponde a {}ºF!'.format(celsius, farenheit))
```

### Aluguel
```
dias = int(input('Quandos dias alugados? '))
km = float(input('Quantos km rodados? '))
pago = dias * 60 + (km * 0.15)
print('O total a pagar é de R${:.2f}'.format(pago))
```

### Quebrando um número
```
from math import trunc
num = float(input('Digite um número: '))
print('O valor digitado foi {} e a sua porção inteira é {}'.format(num, trunc(num)))
```

```
num = float(input('Digite um valor: '))
print('O valor digitado foi {} e a sua porção inteira é {}'.format(num, int(num)))
```

```
num = float(input('Digite um valor: '))
print('O valor digitado foi de {} e a sua porção inteira é {}'.format(num, (num // 1)))
```

### Hipotenusa
```
b = float(input('Comprimento do cateto oposto: '))
c = float(input('Comprimento do cateto adjacente: '))
a = (b ** 2 + c ** 2) ** (1/2)
print('A hipotenusa é {:.2f}'.format(a))
```

```
import math
b = float(input('Comprimento do cateto oposto: '))
c = float(input('Comprimento do cateto adjacente: '))
a = math.hypot(b, c)
print('A hipotenusa é {:.2f}'.format(a))
```

```
from math import hypot
b = float(input('Comprimento do cateto oposto: '))
c = float(input('Comprimento do cateto adjacente: '))
a = hypot(b, c)
print('A hipotenusa é {:.2f}'.format(a))
```

### Seno, cosseno e tangente
```
import math
an = float(input('Digite o ângulo que você deseja: '))
seno = math.sin(math.radians(an))
cosseno = math.cos(math.radians(an))
tangente = math.tan(math.radians(an))
print('O ângulo de {:.2f} tem \n o seno de {:.2f}, \n o cosseno de {:.2f} \n e a tangente de {:.2f}'.format(an, seno, cosseno, tangente))
```

```
from math import radians, sin, cos, tan
an = float(input('Digite o ângulo que você deseja: '))
seno = sin(radians(an))
cosseno = cos(radians(an))
tangente = tan(radians(an))
print('O ângulo de {:.2f} tem \n o seno de {:.2f}, \n o cosseno de {:.2f} \n e a tangente de {:.2f}'.format(an, seno, cosseno, tangente))
```

### Bháskara
```
a = float(input('Entre com o valor de a: '))
b = float(input('Entre com o valor de b: '))
c = float(input('Entre com o valor de c: '))

delta = (b ** 2) - 4 * a * c

print('\n**********************\n')

if a == 0:
    print('O valor de', a ,'deve ser diferente de 0')
elif delta < 0:
    print('Sem raízes reais')
else:
    x1 = (-b + delta ** (1/2)) / (2 * a)
    x2 = (-b - delta ** (1/2)) / (2 * a)

    print('x1: {}, x2: {}'.format(x1, x2))
```

### Fatiamento

```
frase = 'Curso em Video Python'
print(frase[9])
```
> Escreve a letra que está no numero 9

```
print(frase[9:13])
```
> Escreve as letras que estão de 9 até 12

```
print(frase[9:21:2])
```
> Escreve as letras de 9 a 20 pulando 2

```
print(frase[:5])
```
> Escreve do começo 0 até 5

```
print(frase[15:])
```
> Escreve do numero 15 até o final

```
print(frase[9::3])
```
> Escreve do numero 9 até o final pulando 3, quando pula 3 mostra o terceiro

### Análise

```
print(len(frase))
```
> quantos caracteres tem frase

```
print(frase.count('o'))
```
> quantas vezes aparece o O

```
print(frase.count('o', 0, 13))
```
> quantas vezes aparece o do 0 a 12

```
print(frase.find('deo'))
```
> onde começa deo

```
print(frase.find('Android'))
```
> vai retornar -1, pois não existe

```
print('Curso' in frase)
```
> vai retornar true ou false

### Transformação

```
frase.replace('Python', 'Android')
frase.upper()
frase.lower()
frase.capitalize()
frase.title()
frase.strip()
frase.rstrip()
frase.lstrip()
```

### Divisão

```
frase.split()
```
> divide uma string de 21 caracteres em varias de 0 a 5 caracteres
> curso em video tem 21 caracteres de 0 a 21
> curso fica com 0 a 4, em 0 a 1, video 0 a 4
> curso é classificado como 0, em como 1, video como 2'''

```
frase = 'Curso em Vídeo Python'
dividido = frase.split()
print(dividido[2][3])
```
> Curso em Vídeo se torna ['Curso', 'em', 'vídeo', 'Python']
> 
> dividido[2] seleciona o 3º termo da lista que começa com 0
> 
> dividido[2][3] seleciona a quarta letra do terceiro termo

### Junção

```
'-'.join(frase)
```
> juntar as frases colocando tracinho

### Sorteio

```
from random import choice
n1 = str(input('Primeiro aluno: '))
n2 = str(input('Segundo aluno: '))
n3 = str(input('Terceiro aluno: '))
n4 = str(input('Quarto aluno: '))
lista = [n1, n2, n3, n4]
escolhido = choice(lista)
print('O aluno escolhido foi {}'.format(escolhido))
```

### Ordem de uma Lista

```
from random import shuffle
n1 = str(input('Primeiro aluno: '))
n2 = str(input('Segundo aluno: '))
n3 = str(input('Terceiro aluno: '))
n4 = str(input('Quarto aluno: '))
lista = [n1, n2, n3, n4]
shuffle(lista)
print('A ordem de apresentação será: ')
print(lista)
```

### Tocar música no Python

```
import pygame
pygame.init()
pygame.mixer.music.load('nomedamusica')
pygame.mixer.music.play()
pygame.event.wait()
```

### Analisando Texto

```
nome = str(input('Digite seu nome completo: ')).strip()
print('Analisando seu nome...')
print('Seu nome em maiúsculas é {}'.format(nome.upper()))
print('Seu nome em minúsculas é {}'.format(nome.lower()))
print('Seu nome tem ao todo {} letras'.format(len(nome) - nome.count(' ')))
# print('Seu primeiro nome tem {} letras'.format(nome.find(' ')))
separa = nome.split()
print('Seu primeiro nome é {} e ele tem {} letras'.format(separa[0], len(separa[0])))
```

### Separando digitos de um número

```
num = int(input('Digite um número: '))
n = str(num)
print('Analisando o número {}'.format(num))
print('Unidade: {}'.format(n[3]))
print('Dezena: {}'.format(n[2]))
print('Centena: {}'.format(n[1]))
print('Milhar: {}'.format(n[0]))
```
> Se digitar menos que 4 números não funciona

```
num = int(input('Digite um número: '))
u = num // 1 % 10
d = num // 10 % 10
c = num // 100 % 10
m = num // 1000 % 10
print('Analisando o número {}'.format(num))
print('Unidade: {}'.format(u))
print('Dezena: {}'.format(d))
print('Centena: {}'.format(c))
print('Milhar: {}'.format(m))
```
> Esse funciona independente do número ter 2 ou 4 algarismos

### Verificando as primeiras letras de um texto

```
cid = str(input('Em que cidade você nasceu? ')).strip()
print(cid[:5].upper() == 'CAÇU')
```

### Procurando uma string dentro de outra

```
nome = str(input('Qual seu nome completo? ')).strip()
print('Seu nome tem Silva? {}'.format('silva' in nome.lower()))
```

### Primeira e última ocorrência de uma string

```
frase = str(input('Digite uma frase: ')).strip().upper()
print('A letra A aparece {} vezes na frase'.format(frase.count('A')))
print('A primeira letra A apareceu na posição {}'.format(frase.find('A')+1))
print('A última letra A apareceu na posição {}'.format(frase.rfind('A')+1))
```

### Primeiro e último nome de uma pessoa

```
n = str(input('Qual seu nome completo? ')).strip()
nome = n.split()
print('Prazer em conhecê-lo {}!'.format(n))
print('Seu primeiro nome é {}'.format(nome[0]))
print('Seu último nome é {}'.format(nome[len(nome)-1]))
```

Condições

'''tempo = int(input('Quantos anos tem seu carro? '))
if tempo <= 3:
    print('Seu carro está novinho')
else:
    print('Seu carro está velhinho')
print('-FIM-')'''

'''print('carro novo' if tempo <= 3 else 'carro velho')'''

'''nome = str(input('Qual é o seu nome? '))
if nome == 'Gustavo':
    print('Que nome lindo você tem!')
else:
    print('Seu nome é uma merda!')
print('Bom dia, {}'.format(nome))'''

n1 = float(input('Digite a primeira nota: '))
n2 = float(input('Digite a segunda nota: '))
m = (n1 + n2) / 2
print('A sua média foi {:.1f}'.format(m))
if m >= 6:
    print('Parabéns, você não é burro')
else:
    print('Vergonha da Profisson')
'''print('Parabens' if m >=6 else 'Estude mais')'''

Advinhação

from random import randint
from time import sleep
computador = randint(0, 5) #Faz o computador pensar
print('-=-' * 20)
print('Vou pensar em um número entre 0 e 5. Tente advinhar...')
print('-=-' * 20)
jogador = int(input('Em que número eu pensei? ')) #Jogador tenta advinhar
print('Processando...')
sleep(3)
if jogador == computador:
    print('Parabéns! Você conseguiu me vencer!')
else:
    print('Ganhei! Eu pensei no número {} e não no {}!'.format(computador, jogador))

Radar

velocidade = float(input('Qual é a velocidade do carro? '))
if velocidade > 80:
    print('Multado! Você excedeu o limite permitido que é de 80Km/h.')
    multa = (velocidade - 80) * 7
    print('Você deve pagar um multa de R${:.2f}!'.format(multa))
print('Tenha um bom dia! Dirija com segurança!')

Par ou ímpar

numero = int(input('Me diga um número qualquer: '))
resultado = numero % 2
if resultado == 0:
    print('O número {} é PAR'.format(numero))
else:
    print('O número {} é ÍMPAR'.format(numero))

distância

distancia = float(input('Qual é a distância da sua viagem? '))
print('Você está prestes a começar uma viagem de {} km'.format(distancia))
'''if distancia <= 200:
    preco = distancia * 0.50
else:
    preco = distancia * 0.45'''
preco = distancia * 0.50 if distancia <= 200 else distancia * 0.45
print('E o preço da sua passagem será de R${:.2f}'.format(preco))

ano bissexto

from datetime import date
ano = int(input('Que ano quer analisar? Coloque o para o ano atual: '))
if ano == 0:
    ano = date.today().year
if ano % 4 == 0 and ano % 100 != 0 or ano % 400 == 0:
    print('O ano {} é BISSEXTO'.format(ano))
else:
    print('O ano {} NÃO É BISSEXTO'.format(ano))

maior e menor

c = int(input('Digite o terceiro valor: '))
'''if a<b and a<c:
    menor = a
if b<c and b<a:
    menor = b
if c<b and c<a:
    menor = c'''
# Verificando quem é menor
menor = a
if b < a and b < c:
    menor = b
if c < a and c < b:
    menor = c
# Verificando quem é o maior
maior = a
if b > a and b > c:
    maior = b
if c > a and c > b:
    maior = c
print('O menor valor digitado foi {}'.format(menor))
print('O maior valor digitado foi {}'.format(maior))

salario

salario = float(input('Qual é o salário do funcionário? R$ '))
if salario <= 1250:
    novo = salario + (salario * 15 / 100)
else:
    novo = salario + (salario * 10 / 100)
print('Quem ganhava R$ {:.2f} passa a ganhar R$ {:.2f}'.format(salario, novo))

analisando triângulos

print('-=-' * 20)
print('Analisando Triângulos')
print('-=-' * 20)
r1 = float(input('Primeiro segmento: '))
r2 = float(input('Segundo segmento: '))
r3 = float(input('Terceiro segmento: '))
if r1 < r2 + r3 and r2 < r1 + r3 and r3 < r1 + r2:
    print('Os segmentos acima podem formar TRIÂNGULOS')
else:
    print('Os segmentos acima NÃO podem formar TRIÂNGULOS')

Cores no Terminal

'''
\033[style:text:back m
Style
0 - none
1 - bold
4 - underline
7 - negative

Text
30 - white
31 - red
32 - green
33 - yellow
34 - blue
35 - purple
36 - light blue
37 - grey

Back
40 - 47 (the same as 30 - 37)
'''
'''
print('\033[0:30:41mOlá, Mundo!\033[m') #só a frase
print('\033[4:33:44mOlá, Mundo!') # sem o \033 no final vai a linha toda
print('\033[1:35:43mOlá, Mundo!\033[m')
print('\033[30:42mOlá, Mundo!')
print('\033[mOlá, Mundo!')
print('\033[7:30mOlá, Mundo!')
'''

a = 3
b = 5
print('Os valores são \033[32m{}\033[m e \033[31m{}\033[m'.format(a, b))
