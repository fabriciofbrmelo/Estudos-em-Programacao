# Python

### Curso em Vídeo com Gustavo Guanabara
- Comandos que estou aprendendo com os vídeos de [Gustavo Guanabara](https://www.youtube.com/playlist?list=PLHz_AreHm4dlKP6QQCekuIPky1CiwmdI6)

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
```
preco = float(input('Qual o preço do produto? R$ '))
novo = preco * 0.95
print('O produto que custava R$ {:.2f}, na promoção com desconto de 5% vai custar R$ {:.2f}'.format(preco, novo))
```
> Se você quer aumentar 10% em um valor, multiplica o valor por 1.1, sendo 1.0 os 100% e 0.1 os 10% a mais, já se quiser diminuir é só multiplicar pelo valor diminuído, tipo multiplica por 0.9 para diminuir 10%, multipllica por 0.8 para diminuir 20%

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

## Módulo 2

## Condições

### if... else
```
tempo = int(input('Quantos anos tem seu carro? '))
if tempo <= 3:
    print('Seu carro está novinho')
else:
    print('Seu carro está velhinho')
print('-FIM-')
```

```
print('carro novo' if tempo <= 3 else 'carro velho')
```

```
nome = str(input('Qual é o seu nome? '))
if nome == 'Gustavo':
    print('Que nome lindo você tem!')
else:
    print('Seu nome é uma merda!')
print('Bom dia, {}'.format(nome))
```

```
n1 = float(input('Digite a primeira nota: '))
n2 = float(input('Digite a segunda nota: '))
m = (n1 + n2) / 2
print('A sua média foi {:.1f}'.format(m))
if m >= 6:
    print('Parabéns, você não é burro')
else:
    print('Vergonha da Profisson')
```

```
print('Parabens' if m >=6 else 'Estude mais')
```

### Advinhação
```
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
```

### Radar
```
velocidade = float(input('Qual é a velocidade do carro? '))
if velocidade > 80:
    print('Multado! Você excedeu o limite permitido que é de 80Km/h.')
    multa = (velocidade - 80) * 7
    print('Você deve pagar um multa de R${:.2f}!'.format(multa))
print('Tenha um bom dia! Dirija com segurança!')
```

### Par ou Ímpar
```
numero = int(input('Me diga um número qualquer: '))
resultado = numero % 2
if resultado == 0:
    print('O número {} é PAR'.format(numero))
else:
    print('O número {} é ÍMPAR'.format(numero))
```

### Distância
```
distancia = float(input('Qual é a distância da sua viagem? '))
print('Você está prestes a começar uma viagem de {} km'.format(distancia))
'''if distancia <= 200:
    preco = distancia * 0.50
else:
    preco = distancia * 0.45'''
preco = distancia * 0.50 if distancia <= 200 else distancia * 0.45
print('E o preço da sua passagem será de R${:.2f}'.format(preco))
```

### Biblioteca DateTime - Date
```
from datetime import date
today = date.today()
print(today)
print('day:', today.day)
print('month:', today.month)
print('year:', today.year)
```
> 2022-05-31
> 
> day: 31
> 
> month: 5
> 
> year: 2022
```
from datetime import date
print(today.strftime('%A %d %B %Y'))
```
> strftime para imprimir o dia da semana, o mês de maio em vez do número 5
> 
> Tuesday 31 May 2022
```
from datetime import date
print(today.strftime('%A, %dth of %B %Y'))
```
> Tuesday, 31th of May 2022
```
from datetime import date
next_year = today.replace(year = today.year + 1)
print(next_year)
```
> Para saber o próximo ano
> 
> 2023-05-31
```
from datetime import date
difference = abs(next_year - today)
print('only {} days untill next year'.format(difference.days))
```
> Para saber quantos dias faltam para o próximo ano
> 
> only 365 days untill next year
```
from datetime import date
NikolaTesla = date(1856, 7, 10)
print('Nikola Tesla was born on:', NikolaTesla)
```
> Você escolhe a data e sai no formato data
> 
> Nikola Tesla was born on: 1856-07-10
```
from datetime import date
NikolaTesla = date(1856, 7, 10)
NikolaTesla = date.fromisoformat('1856-07-10')
print('Nikola Tesla was born on:', NikolaTesla)
print(NikolaTesla.weekday())
```
> Saiu 3 porque Segunda é 0, Terça é 1, Quarta é 2, Quinta é 3, etc...
> 
> Nikola Tesla was born on: 1856-07-10
> 
> 3

### Biblioteca DateTime - DateTime (Horas)
```
from datetime import date, datetime
now = datetime.now()
print(now)
```
> Imprime data e hora com segundos
> 
> 2022-05-31 19:35:19.846711
```
from datetime import date, datetime
now = datetime.now()
print(now)
print("it's the {}th minute of the {}nd hour, of the {}th day of the {}nd month".format(now.minute, now.hour, now.day, now.month))
```
> 2022-05-31 18:55:22.431856
> 
> it's the 55th minute of the 18nd hour, of the 31th day of the 5nd month

### Biblioteca DateTime - DateTime (Horas com Time Zone)
#### Nuclear disaster in Chernobyl
```
from datetime import date, datetime
chernobyl = datetime.fromisoformat('1986-04-26 01:23:40:000+04:00')
print('the nuclear disaster in Chernobyl occured on: ', chernobyl)
```
> (ano-mês-dia hora:minuto:segundo:milissegundos timezone)
> 
> the nuclear disaster in Chernobyl occured on:  1986-04-26 01:23:40+04:00
```
from datetime import date, datetime
print(chernobyl.strftime('The Chernobyl accident occured on %A %B %dth, %Y at %X MSD(%Z)'))
```
> The Chernobyl accident occured on Saturday April 26th, 1986 at 01:23:40 MSD(UTC+04:00)
```
from datetime import date, datetime
print('MSD is actually:', chernobyl.tzinfo)
```
> MSD is actually: UTC+04:00

### Biblioteca DateTime - Time
```
from datetime import date, datetime, time
my_time = time(15, 33, 8)
print(my_time)
```
> 15:33:08
```
from datetime import date, datetime, time
my_time = time(15, 33, 8)
my_time = time.fromisoformat('15:33:08-07:00')
print(my_time)
```
> 15:33:08-07:00
```
from datetime import date, datetime, time
my_time = time(15, 33, 8)
my_time = time.fromisoformat('15:33:08-07:00')
print(my_time)
print(my_time.strftime('%I:%M %p'))
```
> 03:33 PM
```
from datetime import date, datetime, time
my_date = date(2022, 5, 22)
my_birthday = datetime.combine(my_date, my_time)
print(my_birthday)
```
> 2022-05-22 15:33:08-07:00

### Ano Bissexto
```
from datetime import date
ano = int(input('Que ano quer analisar? Coloque 0 para o ano atual: '))
if ano == 0:
    ano = date.today().year
if ano % 4 == 0 and ano % 100 != 0 or ano % 400 == 0:
    print('O ano {} é BISSEXTO'.format(ano))
else:
    print('O ano {} NÃO É BISSEXTO'.format(ano))
```

### Maior e Menor
```
a = int(input('Digite o primeiro valor: '))
b = int(input('Digite o segundo valor: '))
c = int(input('Digite o terceiro valor: '))
if a < b and a < c:
    menor = a
if b < c and b < a:
    menor = b
if c < b and c < a:
    menor = c
if a > b and a > c:
    maior = a
if b > c and b > a:
    maior = b
if c > b and c > a:
    maior = c
print('O menor valor digitador foi', menor)
print('O maior valor digitado foi', maior)
```

#### Maior e Menor - Simplificado
```
a = int(input('Digite o primeiro valor: '))
b = int(input('Digite o segundo valor: '))
c = int(input('Digite o terceiro valor: '))
menor = a
if b < a and b < c:
    menor = b
if c < a and c < b:
    menor = c
maior = a
if b > a and b > c:
    maior = b
if c > a and c > b:
    maior = c
print('O menor valor digitado foi {}'.format(menor))
print('O maior valor digitado foi {}'.format(maior))
```

### Salário
```
salario = float(input('Qual é o salário do funcionário? R$ '))
if salario <= 1250:
    novo = salario + (salario * 15 / 100)
else:
    novo = salario + (salario * 10 / 100)
print('Quem ganhava R$ {:.2f} passa a ganhar R$ {:.2f}'.format(salario, novo))
```

### Analisando Triângulos
```
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
```

## Cores no Terminal
> \033[style:text:back m
> 
> Style
> 
> 0 - none
> 
> 1 - bold
> 
> 4 - underline
> 
> 7 - negative

> Text
> 
> 30 - white
> 
> 31 - red
> 
> 32 - green
> 
> 33 - yellow
> 
> 34 - blue
> 
> 35 - purple
> 
> 36 - light blue
> 
> 37 - grey

> Back
> 
> 40 - 47 (the same as 30 - 37)

```
print('\033[0:30:41mOlá, Mundo!\033[m') #só a frase
print('\033[4:33:44mOlá, Mundo!') # sem o \033 no final vai a linha toda
print('\033[1:35:43mOlá, Mundo!\033[m')
print('\033[30:42mOlá, Mundo!')
print('\033[mOlá, Mundo!')
print('\033[7:30mOlá, Mundo!')
```

```
a = 3
b = 5
print('Os valores são \033[32m{}\033[m e \033[31m{}\033[m'.format(a, b))
```

```
nome = 'Guanabara'
print('Olá! Muito prazer em conhecê-lo, {}{}{}!'.format('\033[4;34m', nome, '\33[m'))
```

```
nome = 'Guanabara'
cores = {'limpa':'\033[m',
         'azul':'\033[34m',
         'amarelo':'\033[33m',
         'pretoebranco':'\033[7:30m'}
print('Olá! Muito prazer em te conhecer, {}{}{}!'.format(cores['amarelo'], nome, cores['limpa']))
```

## Condições Aninhadas

### Estruturas de Controle e Condições Aninhadas
```
nome = str(input('Qual é o seu nome? '))
if nome == 'Gustavo':
    print('Que nome bonito!')
elif nome == 'Pedro' or nome == 'Maria' or nome == 'Paulo':
    print('Seu nome é bem popular no Brasil!')
elif nome in 'Ana Cláudia Jéssica Juliana':
    print('Belo nome feminino')
else:
    print('Seu nome é bem normal!')
print('Tenha um bom dia {}'.format(nome))
```

### Empréstimo
```
valor = float(input('Qual o valor da casa? '))
salario = float(input('Qual o seu salário? '))
meses = int(input('Em quantos meses você quer financiar? '))
anos = float(meses / 12)
prestacao = valor / meses
print('Você quer financiar uma casa de R${:.2f} com o salário de R${:.2f} dividido em {} meses ou {:.1f} anos'.format(valor, salario, meses, anos))
if prestacao >= salario * 30 / 100:
    print('Seu empréstimo foi NEGADO')
else:
    print('Sua prestação será de R${:.2f} por {} meses'.format(prestacao, meses))
```
```
casa = float(input('Valor da casa: R$ '))
salario = float(input('Salário do comprador: R$ '))
anos = int(input('Quantos anos de financiamento? '))
prestacao = casa / (anos * 12)
minimo = salario * 30 / 100
print('Para pagar um casa de R${:.2f} em {} anos'.format(casa, anos), end='')
print(' e a prestação será de R${:.2f}'.format(prestacao))
if prestacao <= minimo:
    print('Empréstimo pode ser CONCEDIDO')
else:
    print('Empréstimo NEGADO')
```

### Binário
```
num = int(input('Digite um número inteiro: '))
print('''Escolha uma das bases para conversão:
[1] Converter para Binário
[2] Converter para Octal
[3] Converter para Hexadecimal''')
opcao = int(input('Sua opção: '))
if opcao == 1:
    print('{} convertido para BINÁRIO é igual a {}'.format(num, bin(num)[2:]))
elif opcao == 2:
    print('{} convertido para OCTAL é igual a {}'.format(num, oct(num)[2:]))
elif opcao == 3:
    print('{} convertido para HEXADECIMAL é igual a {}'.format(num, hex(num)[2:]))
else:
    print('OPÇÃO INVÁLIDA!!! Tente Novamente!!!')
```
> Coloca-se [2:0] para que se comece do 3º número, pois na hora que imprime binário vai ser 0b1101101010

### Maior ou Menor
```
num1 = int(input('Digite o primeiro número: '))
num2 = int(input('Digite o segundo número: '))
if num1 > num2:
    print('O número {} é maior que o número {}'.format(num1, num2))
elif num2 > num1:
    print('O número {} é maior que o número {}'.format(num2, num1))
else:
    print('Os dois valores são iguais!')
```

### Exército

```
from datetime import date
atual = date.today().year
nasc = int(input('Digite o ano do seu nascimento: '))
idade = atual - nasc
print('Quem nasceu em {} tem {} anos em {}.'.format(nasc, idade, atual))
print('''Você é Homem ou Mulher?
[M] Homem
[F] Mulher''')
opcao = str(input('Digite [M] para Homem ou [F] para Mulher: ').upper())
if opcao == 'M':
    if idade == 18:
        print('Você tem que se alistar IMEDIATAMENTE!')
    elif idade < 18:
        saldo = 18 - idade
        print('Ainda faltam {} anos para o alistamento'.format(saldo))
        ano = atual + saldo
        print('Seu alistamento será em {}.'.format(ano))
    elif idade > 18:
        saldo = idade - 18
        print('Você já deveria ter se alistado há {} anos.'.format(saldo))
        ano = atual - saldo
        print('Seu alistamento foi em {}.'.format(ano))
else:
    print('Você não precisa se alistar')
```

### Média
```
n1 = float(input('Digite a sua primeira nota: '))
n2 = float(input('Digite a sua segunda nota: '))
media = (n1 + n2) / 2
if media >= 7:
    print('Sua média é {:.1f} e você está APROVADO!'.format(media))
elif media >=5 and media <= 6.9:
    print('Sua média é {:.1f} e você está em RECUPERAÇÃO!'.format(media))
else:
    print('Sua média é {:.1f} e você está REPROVADO!'.format(media))
```

### Natação
```
print('-=-' * 10)
print('\033[1:31:40mConfederação Nacional de Natação\033[m')
print('-=-' * 10)
from datetime import date
ano = int(input('Em que ano você nasceu? '))
atual = date.today().year
idade = atual - ano
if idade <= 9:
    print('Você tem {} anos e está na categoria MIRIM'.format(idade))
elif 9 < idade <= 14:
    print('Você tem {} anos e está na categoria INFANTIL'.format(idade))
elif 14 < idade <= 19:
    print('Você tem {} anos e está na categoria JUNIOR'.format(idade))
elif 19 < idade <=20:
    print('Você tem {} anos e está na categoria SÊNIOR'.format(idade))
else:
    print('Você tem {} anos e está na categoria MASTER'.format(idade))
```

### Analisando triângulos
```
r1 = float(input('Primeiro segmento: '))
r2 = float(input('Segundo segmento: '))
r3 = float(input('Terceiro segmento: '))
if r1 < r2 + r3 and r2 < r1 + r3 and r3 < r1 + r2:
    print('Os segmentos PODEM FORMAR um triângulo ', end='')
    if r1 == r2 and r2 == r3:
        print('EQUILÁTERO!')
    elif r1 != r2 != r3 != r1:
        print('ESCALENO')
    else:
        print('ISÓSCELES')
else:
    print('Os segmentos NÃO PODEM FORMAR um triângulo!')
```

### IMC
```
peso = float(input('Qual o seu peso? (Kg) '))
altura = float(input('Qual a sua altura? (m) '))
imc = peso / (altura ** 2)
print('O IMC dessa pessoa é de {:.1f} '.format(imc), end='')
if imc < 18.5:
    print('e ela está ABAIXO DO PESO!')
elif 18.5 <= imc < 25:
    print('e ela está no PESO IDEAL!')
elif 25 <= imc < 30:
    print('e ela está com SOBREPESO!')
elif 30 <= imc < 40:
    print('e ela está com OBESIDADE!')
else:
    print('e ela está com OBESIDADE MÓRBIDA!')
```

### Pagamentos
```
print('{:=^40}'.format(' LOJAS GUANABARA '))
preco = float(input('Preço das compras: R$ '))
print('''FORMAS DE PAGAMENTO
[1] À VISTA (DINHEIRO/CHEQUE)
[2] À VISTA (CARTÃO)
[3] 2X NO CARTÃO
[4] 3X OU MAIS NO CARTÃO''')
opcao = int(input('Qual é a opção? '))
if opcao == 1:
    total = preco - (preco * 10 / 100)
elif opcao == 2:
    total = preco - (preco * 5 / 100)
elif opcao == 3:
    total = preco
    parcela = total/2
    print('Sua compra será parcelada em 2x de R${:.2f}'.format(parcela))
elif opcao == 4:
    total = preco + (preco * 20 / 100)
    totparc = int(input('Quantas parcelas? '))
    parcela = total / totparc
    print('Sua compra será parcelada em {}x de R${:.2f} COM JUROS'.format(totparc, parcela))
else:
    total = 0
    print('OPÇÃO INÁLIDA DE PAGAMENTO!!!')
print('Sua compra de R${:.2f} vai custar R${:.2f}'.format(preco, total))
```

### Rock, Paper, Scissors, Lizard, Spock
```
from random import randint
from time import sleep
itens = ('Rock', 'Paper', 'Scissors', 'Lizard', 'Spock')
computador = randint(0, 4)
print('=' * 50)
print('Welcome to ROCK, PAPER, SCISSORS, LIZARD, SPOCK')
print('=' * 50)
print('''Your options are:
[0] ROCK
[1] PAPER
[2] SCISSORS
[3] LIZARD
[4] SPOCK
''')
jogador = int(input('What is your move? '))
print('ROCK')
sleep(0.5)
print('PAPER')
sleep(0.5)
print('SCISSORS')
sleep(0.5)
print('LIZARD')
sleep(0.5)
print('SPOCK')
sleep(0.5)
print('-=' * 10)
print('Computer played {}'.format(itens[computador]))
print('You played {}'.format(itens[jogador]))
print('-=' * 10)
if computador == 0: # ROCK
    if jogador == 0: # ROCK
        print('TIE!')
    elif jogador == 1: # PAPER
        print('Paper covers Rock. Player wins! Congratulations!')
    elif jogador == 2: # SCISSORS
        print('Rock crushes Scissors. Computer wins! You lost!')
    elif jogador == 3: # LIZARD
        print('Rock crushes Lizard. Computer wins! You lost!')
    elif jogador == 4: # SPOCK
        print('Spock vaporizes Rock. Player wins! Congratulations!')
    else:
        print('Try Again!!!')
if computador == 1: # PAPER
    if jogador == 0: # ROCK
        print('Paper covers Rock. Computer wins! You lost!')
    elif jogador == 1: # PAPER
        print('TIE!')
    elif jogador == 2: # SCISSORS
        print('Scissors cuts Paper. Player wins! Congratulations!')
    elif jogador == 3: # LIZARD
        print('Lizard eats paper. Player wins! Congratulations!')
    elif jogador == 4: # SPOCK
        print('Paper disproves Spock. Computer wins! You lost!')
    else:
        print('Try Again!!!')
if computador == 2: # SCISSORS
    if jogador == 0: # ROCK
        print('Rock crushes scissors. Player wins! Congratulations!')
    elif jogador == 1: # PAPER
        print('Scissors cuts paper. Compute wins! You lost!')
    elif jogador == 2: # SCISSORS
        print('TIE!')
    elif jogador == 3: # LIZARD
        print('Scissors decapitates Lizard. Computer wins! You lost!')
    elif jogador == 4: # SPOCK
        print('Spock smashes scissors. Player wins! Congratulations!')
    else:
        print('Try Again!!!')
if computador == 3: # LIZARD
    if jogador == 0: # ROCK
        print('Rock crushes Lizard. Player wins! Congratulations!')
    elif jogador == 1: # PAPER
        print('Lizard eats paper. Computer wins! You lost!')
    elif jogador == 2: # SCISSORS
        print('Scissors decapitates Lizard. Player wins! Congratulations!')
    elif jogador == 3: # LIZARD
        print('TIE!')
    elif jogador == 4: # SPOCK
        print('Lizard poisons Spock. Computer wins! You lost!')
    else:
        print('Try Again!!!')
if computador == 4: # SPOCK
    if jogador == 0: # ROCK
        print('Spock vaporizes Rock. Computer wins! You lost!')
    elif jogador == 1: # PAPER
        print('Paper disproves Spock. Player wins! Congratulations!')
    elif jogador == 2: # SCISSORS
        print('Spock smashes Scissors. Computer wins! You lost!')
    elif jogador == 3: # LIZARD
        print('Lizard poisons Spock. Player wins! Congratulations!')
    elif jogador == 4: # SPOCK
        print('TIE!')
    else:
        print('Try Again!!!')
```

## Laços de Repetição (for)

### Contar de 0 a 6
```
for c in range(0, 6):
    print(c)
print('Fim')
```
> 0
> 
> 1
> 
> 2
> 
> 3
> 
> 4
> 
> 5
> 
> Fim

### Contar de 6 a 1 de trás para frente (último número não conta)
```
for c in range(6, 0, -1):
    print(c)
print('Fim')
```
> 6
> 
> 5
> 
> 4
> 
> 3
> 
> 2
> 
> 1
> 
> Fim

### Contar de 0 a 7 pulando de 2 em 2
```
for c in range(0, 8, 2):
    print(c)
print('Fim')
```
> 0
> 
> 2
> 
> 4
> 
> 6
> 
> Fim

### Escolhendo até onde você digitar
```
n = int(input('Digite um número: '))
for c in range(0, n):
    print(c)
print('Fim')
```
> Digite um número: 2
> 
> 0
> 
> 1
> 
> Fim

```
i = int(input('Início: '))
f = int(input('Fim: '))
p = int(input('Passo: '))
for c in range(i, f + 1, p):
    print(c)
print('Fim')
```
> Início: 1
> 
> Fim: 10
> 
> Passo: 1
> 
> 1
> 
> 2
> 
> 3
> 
> 4
> 
> 5
> 
> 6
> 
> 7
> 
> 8
> 
> 9
> 
> 10
> 
> Fim

```
s = 0
for c in range(0, 3):
    n = int(input('Digite um valor: '))
    s = s + n # s += n
print('O somatório de todos os valores foi {}'.format(s))
```
> Digite um valor: 2
> 
> Digite um valor: 3
> 
> Digite um valor: 4
> 
> O somatório de todos os valores foi 9

### Contagem regressiva
```
from time import sleep
for c in range(10, 0, -1):
    print(c)
    sleep(1)
print('Feliz Ano Novo!')
```

### Números Pares entre 1 e 50
```
for c in range(0, 50, 2):
    print('{} '.format(c), end='')
print('Fim')
```
> 0 2 4 6 8 10 12 14 16 18 20 22 24 26 28 30 32 34 36 38 40 42 44 46 48 Fim

```
for n in range(1, 51):
    if n % 2 == 0:
        print(n, end=' ')
print('Acabou!')
```
> 2 4 6 8 10 12 14 16 18 20 22 24 26 28 30 32 34 36 38 40 42 44 46 48 50 Acabou!

```
for n in range(1, 51):
    print('.', end='')
    if n % 2 == 0:
        print(n, end=' ')
print('Acabou!')
```
> ..2 ..4 ..6 ..8 ..10 ..12 ..14 ..16 ..18 ..20 ..22 ..24 ..26 ..28 ..30 ..32 ..34 ..36 ..38 ..40 ..42 ..44 ..46 ..48 ..50 Acabou!
> 
> Vai fazer um ponto para cada vez que roda o laço

```
for n in range(2, 51, 2):
    print('.', end='')
    print(n, end=' ')
print('Acabou!')
```
> .2 .4 .6 .8 .10 .12 .14 .16 .18 .20 .22 .24 .26 .28 .30 .32 .34 .36 .38 .40 .42 .44 .46 .48 .50 Acabou!
> 
> Repete um ponto só uma vez

### Soma de ímpares múltiplos de três de 1 a 500
```
soma = 0
cont = 0
for c in range(1, 501, 2):
    if c % 3 == 0:
        cont = cont + 1 # cont += 1
        soma = soma + c # soma += c
print('A soma de todos os {} valores múltiplos de três entre 1 e 500 é {}'.format(cont, soma))
```
> A soma de todos os 83 valores múltiplos de três entre 1 e 500 é 20667

### Tabuada 2.0
```
from time import sleep
num = int(input('Digite um número para ver sua tabuada: '))
for c in range(1, 11):
    print('{} x {:2} = {}'.format(num, c, num*c))
    sleep(1)
```

### Seis números inteiros e mostre a soma dos pares
```
soma = 0
cont = 0
for c in range(1, 7):
    num = int(input('Digite o {} valor: '.format(c)))
    if num % 2 == 0:
        soma += num
        cont += 1
print('Você informou {} números PARES e a soma foi {}'.format(cont, soma))
```
> Digite o 1º valor: 2
> 
> Digite o 2º valor: 3
> 
> Digite o 3º valor: 6
> 
> Digite o 4º valor: 9
> 
> Digite o 5º valor: 6
> 
> Digite o 6º valor: 5
> 
> Você informou 3 números PARES e a soma foi 14

### Progressão Aritmética
```
print('=' * 20)
print('10 TERMOS DE UMA PA')
print('=' * 20)
primeiro = int(input('Primeiro Termo: '))
razao = int(input('Razão: '))
decimo = primeiro + (10 - 1) * razao
for c in range(primeiro, decimo + razao, razao):
    print('{} '.format(c), end=' -> ')
print('ACABOU!')
```

### Números Primos
```
num = int(input('Digite um número: '))
for c in range(1, num + 1):
    print('{} '.format(c), end='')
```
> Digite um número: 5
> 
> 1 2 3 4 5

```
num = int(input('Digite um número: '))
for c in range(1, num + 1):
    if num % c == 0:
        print('\033[33m', end='')
    else:
        print('\033[31m', end='')
    print('{} '.format(c), end='')
```
> Digite um número: 5
> 
> 1 2 3 4 5 (1 e 5 saem pintados)

```
num = int(input('Digite um número: '))
tot = 0
for c in range(1, num + 1):
    if num % c == 0:
        print('\033[33m', end='')
        tot += 1
    else:
        print('\033[31m', end='')
    print('{} '.format(c), end='')
print('O número {} foi divisível {} vezes'.format(num, tot))
```
> Digite um número: 5
> 
> 1 2 3 4 5 O número 5 foi divisível 2 vezes

```
num = int(input('Digite um número: '))
tot = 0
for c in range(1, num + 1):
    if num % c == 0:
        print('\033[33m', end='')
        tot += 1
    else:
        print('\033[31m', end='')
    print('{} '.format(c), end='')
print('\n\033[mO número {} foi divisível {} vezes'.format(num, tot))
if tot == 2:
    print('E por isso ele é PRIMO!')
else:
    print('E por isso ele NÃO é PRINO')
```

### Palindromo
```
frase = str(input('Digite uma frase: ')).strip().upper()
palavras = frase.split()
print('Você digitou a frase {}'.format(palavras))
```
> Digite uma frase: Fabricio Freitas
> 
> Você digitou a frase ['FABRICIO', 'FREITAS']

```
frase = str(input('Digite uma frase: ')).strip().upper()
palavras = frase.split()
junto = ''.join(palavras)
print('Você digitou a frase {}'.format(junto))
```
> Digite uma frase: Fabrício Freitas
> 
> Você digitou a frase FABRÍCIOFREITAS

```
frase = str(input('Digite uma frase: ')).strip().upper()
palavras = frase.split()
junto = ''.join(palavras)
inverso = ''
for letra in range(len(junto) - 1, -1, -1):
    print(junto[letra])
```
> Digite uma frase: Fabricio
> 
> OICIRBAF

> len(junto) --> conta o número de letras de junto
> 
> len(junto) - 1 porque se tem 20 letras é do 0 ao 19
> 
> outro - 1 porque a primeira letra é 0
> 
> outro - 1 porque está voltando uma letra

```
frase = str(input('Digite uma frase: ')).strip().upper()
palavras = frase.split()
junto = ''.join(palavras)
inverso = ''
for letra in range(len(junto) - 1, -1, -1):
    inverso = inverso + junto[letra]
print(inverso)
```
> Digite uma frase: Fabricio
> 
> OICIRBAF

```
frase = str(input('Digite uma frase: ')).strip().upper()
palavras = frase.split()
junto = ''.join(palavras)
inverso = ''
for letra in range(len(junto) - 1, -1, -1):
    inverso = inverso + junto[letra]
print(junto, inverso)
```
> Digite uma frase: Ana
> 
> ANA ANA
> 
> Ana é palíndromo, pois junto == inverso

```
frase = str(input('Digite uma frase: ')).strip().upper()
palavras = frase.split()
junto = ''.join(palavras)
inverso = ''
for letra in range(len(junto) - 1, -1, -1):
    inverso = inverso + junto[letra]
if inverso == junto:
    print('Temos um PALÍNDROMO!')
else:
    print('A frase digitada NÃO É UM PALÍNDROMO!')
```
> Digite uma frase: Ana
> 
> Temos um PALÍNDROMO!

```
frase = str(input('Digite uma frase: ')).strip().upper()
palavras = frase.split()
junto = ''.join(palavras)
inverso = ''
for letra in range(len(junto) - 1, -1, -1):
    inverso = inverso + junto[letra]
print('O inverso de {} é {}'.format(junto, inverso))
if inverso == junto:
    print('Temos um PALÍNDROMO!')
else:
    print('A frase digitada NÃO É UM PALÍNDROMO!')
```
> O inverso de ATORREDADERROTA é ATORREDADERROTA
> 
> Temos um PALÍNDROMO!

```
frase = str(input('Digite uma frase: ')).strip().upper()
palavras = frase.split()
junto = ''.join(palavras)
inverso = junto[::-1]
print('O inverso de {} é {}'.format(junto, inverso))
if inverso == junto:
    print('Temos um palíndromo')
else:
    print('A frase digitada não é um palíndromo')
```
> inverso = junto[::-1] substitutiu o for

### Maioridade
```
from datetime import date
atual = date.today().year
nasc = int(input('Em que ano a pessoa nasceu? '))
idade = atual - nasc
print('Essa pessoa tem {} anos'.format(idade))
```
> Em que ano a pessoa nasceu? 1993
> 
> Essa pessoa tem 29 anos

```
from datetime import date
atual = date.today().year
nasc = int(input('Em que ano a pessoa nasceu? '))
idade = atual - nasc
if idade >= 21:
    print('Essa pessoa é maior de idade!')
else:
    print('Essa pessoa é menor idade!')
```
> Em que ano a pessoa nasceu? 2005
> 
> Essa pessoa é menor idade!

```
from datetime import date
atual = date.today().year
for pess in range(1, 8):
    nasc = int(input('Em que ano a pessoa nasceu? '))
    idade = atual - nasc
    if idade >= 21:
        print('Essa pessoa é maior de idade!')
    else:
        print('Essa pessoa é menor idade!')
```
> Em que ano a pessoa nasceu? 2002
> 
> Essa pessoa é menor idade!
> 
> Em que ano a pessoa nasceu? 2006
> 
> Essa pessoa é menor idade!
> 
> Em que ano a pessoa nasceu? 2004
> 
> Essa pessoa é menor idade!

```
from datetime import date
atual = date.today().year
totmaior = 0
totmenor = 0
for pess in range(1, 8):
    nasc = int(input('Em que ano a {}ª pessoa nasceu? '.format(pess)))
    idade = atual - nasc
    if idade >= 21:
        totmaior += 1
    else:
        totmenor += 1
print('Ao todo tivemos {} pessoas maiores de idade'.format(totmaior))
print('E também tivemos {} pessoas menores de idade'.format(totmenor))
```
```
print('Ao todo tivemos {} pessoas maiores de idade \n e também tivemos {} pessoas menores de idade'.format(totmaior, totmenor))
```
> Em que ano a 1ª pessoa nasceu? 1993
> 
> Em que ano a 2ª pessoa nasceu? 1990
> 
> Em que ano a 3ª pessoa nasceu? 1999
> 
> Em que ano a 4ª pessoa nasceu? 2005
> 
> Em que ano a 5ª pessoa nasceu? 2012
> 
> Em que ano a 6ª pessoa nasceu? 2009
> 
> Em que ano a 7ª pessoa nasceu? 2010
> 
> Ao todo tivemos 3 pessoas maiores de idade
> 
> E também tivemos 4 pessoas menores de idade

### Maior e Menor Sequência
```
maior = 0
menor = 0
for p in range(1, 6):
    peso = float(input('Peso da {}ª pessoa: '.format(p)))
```
> Peso da 1ª pessoa: 10
> 
> Peso da 2ª pessoa: 15
> 
> Peso da 3ª pessoa: 20
> 
> Peso da 4ª pessoa: 30
> 
> Peso da 5ª pessoa: 40

```
maior = 0
menor = 0
for p in range(1, 6):
    peso = float(input('Peso da {}ª pessoa: '.format(p)))
    if p == 1:
        maior = peso
        menor = peso
    else:
        if peso > maior:
            maior = peso
        if peso < menor:
            menor = peso
print('O maior peso lido foi de {}Kg'.format(maior))
print('O menor peso lido foi de {}Kg'.format(menor))
```
> Peso da 1ª pessoa: 10
> 
> Peso da 2ª pessoa: 15
> 
> Peso da 3ª pessoa: 20
> 
> Peso da 4ª pessoa: 25
> 
> Peso da 5ª pessoa: 30
> 
> O maior peso lido foi de 30.0Kg
> 
> O menor peso lido foi de 10.0Kg

```
maior = 0
menor = 0
pessoamaior = 0
pessoamenor = 0
for p in range(1, 6):
    peso = float(input('Peso da {}ª pessoa: '.format(p)))
    if p == 1:
        maior = peso
        menor = peso
        pessoamaior = p
        pessoamenor = p
    else:
        if peso > maior:
            maior = peso
            pessoamaior = p
        if peso < menor:
            menor = peso
            pessoamenor = p
print('A pessoa com maior peso é a {}ª pessoa com {}Kg'.format(pessoamaior, maior))
print('A pessoa com menor peso é a {}ª pessoa com {}Kg'.format(pessoamenor, menor))
```
> Peso da 1ª pessoa: 5
> 
> Peso da 2ª pessoa: 10
> 
> Peso da 3ª pessoa: 15
> 
> Peso da 4ª pessoa: 20
> 
> Peso da 5ª pessoa: 25
> 
> A pessoa com maior peso é a 5ª pessoa com 25.0Kg
> 
> A pessoa com menor peso é a 1ª pessoa com 5.0Kg

### Analisador Completo
```
somaidade = 0
mediaidade = 0
maioridadehomem = 0
nomevelho = ''
for p in range(1, 5):
    print('---- {}ª PESSOA ----'.format(p))
    nome = str(input('Nome: ')).strip()
    idade = int(input('Idade: '))
    sexo = str(input('Sexo [M/F]: ')).strip()
    somaidade = somaidade + idade
    if p == 1 and sexo in 'Mm':
        maioridadehomem = idade
        nomevelho = nome
    if sexo in 'Mm' and idade > maioridadehomem:
        maioridadehomem = idade
        nomevelho = nome
mediaidade = somaidade / 4
print('A média de idade do grupo é de {} anos'.format(mediaidade))
print('O homem mais velho tem {} anos e se chama {}'.format(maioridadehomem, nomevelho))
```
> ---- 1ª PESSOA ----
> 
> Nome: João
> 
> Idade: 22
> 
> Sexo [M/F]: m
> 
> ---- 2ª PESSOA ----
> 
> Nome: maria
> 
> Idade: 99
> 
> Sexo [M/F]: f
> 
> ---- 3ª PESSOA ----
> 
> Nome: pedro
> 
> Idade: 12
> 
> Sexo [M/F]: m
> 
> ---- 4ª PESSOA ----
> 
> Nome: claudia
> 
> Idade: 85
> 
> Sexo [M/F]: f
> 
> A média de idade do grupo é de 54.5 anos
> 
> O homem mais velho tem 22 anos e se chama João

```
somaidade = 0
mediaidade = 0
maioridadehomem = 0
nomevelho = ''
totmulher20 = 0
for p in range(1, 5):
    print('---- {}ª PESSOA ----'.format(p))
    nome = str(input('Nome: ')).strip()
    idade = int(input('Idade: '))
    sexo = str(input('Sexo [M/F]: ')).strip()
    somaidade = somaidade + idade
    if p == 1 and sexo in 'Mm':
        maioridadehomem = idade
        nomevelho = nome
    if sexo in 'Mm' and idade > maioridadehomem:
        maioridadehomem = idade
        nomevelho = nome
    if sexo in 'Ff' and idade < 20:
        totmulher20 += 1
mediaidade = somaidade / 4
print('A média de idade do grupo é de {} anos'.format(mediaidade))
print('O homem mais velho tem {} anos e se chama {}'.format(maioridadehomem, nomevelho))
print('Ao todo são {} mulheres com menos de 20 anos'.format(totmulher20))
```
> ---- 1ª PESSOA ----
> 
> Nome: jessica
> 
> Idade: 23
> 
> Sexo [M/F]: f
> 
> ---- 2ª PESSOA ----
> 
> Nome: claudio
> 
> Idade: 12
> 
> Sexo [M/F]: m
> 
> ---- 3ª PESSOA ----
> 
> Nome: pedro 
> 
> Idade: 75
> 
> Sexo [M/F]: m
> 
> ---- 4ª PESSOA ----
> 
> Nome: maria
> 
> Idade: 15
> 
> Sexo [M/F]: f
> 
> A média de idade do grupo é de 31.25 anos
> 
> O homem mais velho tem 75 anos e se chama pedro
> 
> Ao todo são 1 mulheres com menos de 20 anos

## Laços de Repetição (while)
```
for c in range(1, 10):
    print(c)
print('Fim')
```
> 1
> 
> 2
> 
> 3
> 
> 4
> 
> 5
> 
> 6
> 
> 7
> 
> 8
> 
> 9
> 
> Fim

```
c = 1
while c < 10:
    print(c)
    c = c + 1
print('Fim')
```
> 1
> 
> 2
> 
> 3
> 
> 4
> 
> 5
> 
> 6
> 
> 7
> 
> 8
> 
> 9
> 
> Fim

```
n = 1
while n != 0:
    n = int(input('Digite um valor: '))
print('Fim')
```
> Você irá digitar números indefinidamente até ser 0
> 
> Digite um valor: 1
> 
> Digite um valor: 2
> 
> Digite um valor: 2
> 
> Digite um valor: 5
> 
> Digite um valor: 0
> 
> Fim

```
r = 'S'
while r == 'S':
    n = int(input('Digite um valor: '))
    r = str(input('Quer continuar? [S/N] ')).upper()
print('Fim')
```
> Digite um valor: 2
> 
> Quer continuar? [S/N] s
> 
> Digite um valor: 3
> 
> Quer continuar? [S/N] s
> 
> Digite um valor: 5
> 
> Quer continuar? [S/N] n
> 
> Fim

```
par = impar = 0
n = 1
while n != 0:
    n = int(input('Digite um valor: '))
    if n % 2 == 0:
        par += 1
    else:
        impar += 1
print('Você digitou {} pares e {} ímpares!'.format(par, impar))
```
> Conta os pares, inclusive o '0'
> 
> Digite um valor: 2
> 
> Digite um valor: 3
> 
> Digite um valor: 6
> 
> Digite um valor: 5
> 
> Digite um valor: 0
> 
> Você digitou 3 pares e 2 ímpares!

```
par = impar = 0
n = 1
while n != 0:
    n = int(input('Digite um valor: '))
    if n != 0:
        if n % 2 == 0:
            par += 1
        else:
            impar += 1
print('Você digitou {} pares e {} ímpares!'.format(par, impar))
```
> Aqui conta os pares, sem o '0'
> 
> Digite um valor: 2
> 
> Digite um valor: 3
> 
> Digite um valor: 6
> 
> Digite um valor: 0
> 
> Você digitou 2 pares e 1 ímpares!

### Validação de dados
```
sexo = str(input('Informe seu sexo: [M/F] ')).strip().upper()[0]
print(sexo)
```
> Informe seu sexo: [M/F] masculino
> 
> M

```
sexo = str(input('Informe seu sexo: [M/F] ')).strip().upper()[0]
while sexo not in 'MmFf':
    sexo = str(input('Dados inválidos. Por favor, informe seu sexo: [M/F] ')).strip().upper()[0]
print('Sexo {} registrado com sucesso'.format(sexo))
```
> Informe seu sexo: [M/F] k
> 
> Dados inválidos. Por favor, informe seu sexo: [M/F] m
> 
> Sexo M registrado com sucesso

### Jogo da Advinhação 2.0
```
from random import randint
computador = randint(0, 10)
print('Sou seu computador... Acabei de pensar em um número entre 0 e 10.')
print('Será que você consegue advinhar qual foi? ')
acertou = False
while not acertou:
    jogador = int(input('Qual é seu palpite? '))
    if jogador == computador:
        acertou = True
print('Acertou!')
```
> Qual é seu palpite? 0
> 
> Qual é seu palpite? 1
> 
> Qual é seu palpite? 8
> 
> Acertou!

```
from random import randint
computador = randint(0, 10)
print('Sou seu computador... Acabei de pensar em um número entre 0 e 10.')
print('Será que você consegue advinhar qual foi? ')
acertou = False
palpites = 0
while not acertou:
    jogador = int(input('Qual é seu palpite? '))
    palpites += 1
    if jogador == computador:
        acertou = True
print('Acertou com {} tentativas. Parabéns!'.format(palpites))
```
> Qual é seu palpite? 0
> 
> Qual é seu palpite? 1
> 
> Qual é seu palpite? 2
> 
> Acertou com 3 tentativas. Parabéns!

```
from random import randint
computador = randint(0, 10)
print('Sou seu computador... Acabei de pensar em um número entre 0 e 10.')
print('Será que você consegue advinhar qual foi? ')
acertou = False
palpites = 0
while not acertou:
    jogador = int(input('Qual é seu palpite? '))
    palpites += 1
    if jogador == computador:
        acertou = True
    else:
        if jogador < computador:
            print('Mais... Tente mais uma vez.')
        elif jogador > computador:
            print('Menos... Tente mais uma vez.')
print('Acertou com {} tentativas. Parabéns!'.format(palpites))
```

> Será que você consegue advinhar qual foi?
> 
> Qual é seu palpite? 4
> 
> Menos... Tente mais uma vez.
> 
> Qual é seu palpite? 3
> 
> Menos... Tente mais uma vez.
> 
> Qual é seu palpite? 0
> 
> Mais... Tente mais uma vez.
> 
> Qual é seu palpite? 1
> 
> Acertou com 4 tentativas. Parabéns!

### Menu de opções
```
from time import sleep
n1 = int(input('Primeiro valor: '))
n2 = int(input('Segundo valor: '))
opcao = 0
while opcao != 5:
    print('''
    [ 1 ] Somar
    [ 2 ] Multiplicar
    [ 3 ] Maior
    [ 4 ] Novos Números
    [ 5 ] Sair do programa
    ''')
    opcao = int(input('>>>>>>> Qual é a sua opção? '))
    if opcao == 1:
        soma = n1 + n2
        print('A soma entre {} e {} é {}'.format(n1, n2, soma))
    elif opcao == 2:
        produto = n1 * n2
        print('O resultado de {} vezes {} é {}'.format(n1, n2, produto))
    elif opcao == 3:
        if n1 > n2:
            maior = n1
        else:
            maior = n2
        print('Entre {} e {}, o maior valor é {}'.format(n1, n2, maior))
    elif opcao == 4:
        print('Informe os números novamente: ')
        n1 = int(input('Primeiro valor: '))
        n2 = int(input('Segundo valor: '))
    elif opcao == 5:
        print('Finalizando...')
    else:
        print('Opção inválida. Tente novamente!')
    print('=-=' * 10)
    sleep(2)
print('Fim do programa! Volte sempre!')
```
> Primeiro valor: 2
> 
> Segundo valor: 3
>
>    [ 1 ] Somar
>    
>    [ 2 ] Multiplicar
>    
>    [ 3 ] Maior
>    
>    [ 4 ] Novos Números
>    
>    [ 5 ] Sair do programa
>    
> Qual é a sua opção? 1
> 
> A soma entre 2 e 3 é 5
> 
> O resultado de 2 vezes 3 é 6
> 
> Entre 2 e 3, o maior valor é 3

### Fatorial 2.0
```
from math import factorial
n = int(input('Digite um número para calcular seu Fatorial: '))
f = factorial(n)
print('O fatorial de {} é {}.'.format(n, f))
```
> Digite um número para calcular seu Fatorial: 7
> 
> O fatorial de 7 é 5040.

```
from math import factorial
n = int(input('Digite um número para calcular seu Fatorial: '))
c = n
f = factorial(n)
while c > 0:
    print('{} x '.format(c), end='')
    c -= 1
print('O fatorial de {} é {}.'.format(n, f))
```
> Digite um número para calcular seu Fatorial: 5
> 
> 5 x 4 x 3 x 2 x 1 x O fatorial de 5 é 120.

```
from math import factorial
n = int(input('Digite um número para calcular seu Fatorial: '))
c = n
f = factorial(n)
while c > 0:
    print('{}'.format(c), end='')
    print(' x ' if c > 1 else ' = ', end='')
    c -= 1
print('O fatorial de {} é {}.'.format(n, f))
```
> Digite um número para calcular seu Fatorial: 5
> 
> 5 x 4 x 3 x 2 x 1 = O fatorial de 5 é 120.

```
n = int(input('Digite um número para calcular seu Fatorial: '))
c = n
f = 1
print('Calculando {}! = '.format(n), end='')
while c > 0:
    print('{}'.format(c), end='')
    print(' x ' if c > 1 else ' = ', end='')
    f = f * c # f *= c
    c -= 1
print('{}'.format(f))
```
> Digite um número para calcular seu Fatorial: 5
> 
> Calculando 5! = 5 x 4 x 3 x 2 x 1 = 120

### Progressão Aritmética 2.0
```
print('-=-' * 10)
primeiro = int(input('Primeiro termo: '))
razao = int(input('Razão da PA: '))
termo = primeiro
cont = 1
total = 0
mais = 10
while mais != 0:
    total = total + mais
    while cont <= total:
        print('{} -> '.format(termo), end='')
        termo += razao
        cont += 1
    print('PAUSA')
    mais = int(input('Quantos termos você quer mostrar a mais? '))
print('FIM')
```
> Gerador de PA
> 
> -=--=--=--=--=--=--=--=--=--=-
> 
> Primeiro termo: 2
> 
> Razão da PA: 2
> 
> 2 -> 4 -> 6 -> 8 -> 10 -> 12 -> 14 -> 16 -> 18 -> 20 -> PAUSA
> 
> Quantos termos você quer mostrar a mais? 10
> 
> 22 -> 24 -> 26 -> 28 -> 30 -> 32 -> 34 -> 36 -> 38 -> 40 -> PAUSA
> 
> Quantos termos você quer mostrar a mais? 0
> 
> FIM

## Sequência de Fibonacci
### Problema quando usa while: se você não define como o cont vai chegar no n, cont = 3 começa com 3 e você digita n = 10, ele nunca vai chegar no n, logo ficará rodando em loop para sempre
```
print('-' * 25)
print('Sequência de Fibonacci')
print('-' * 25)
n = int(input('Quantos termos você quer mostrar? '))
t1 = 0
t2 = 1
print('~'* 25)
print('{} --> {}'.format(t1, t2), end='')
cont = 3
while cont <= n:
    t3 = t1 + t2
    print(' --> {}'.format(t3), end='')
print('FIM')
```
### Resolveu o problema do loop com cont += 1, porém ainda não soma os números
```
print('-' * 25)
print('Sequência de Fibonacci')
print('-' * 25)
n = int(input('Quantos termos você quer mostrar? '))
t1 = 0
t2 = 1
print('~'* 25)
print('{} --> {}'.format(t1, t2), end='')
cont = 3
while cont <= n:
    t3 = t1 + t2
    print(' --> {}'.format(t3), end='')
    cont += 1
print('FIM')
```
> Quantos termos você quer mostrar? 10
> 
> 0 --> 1 --> 1 --> 1 --> 1 --> 1 --> 1 --> 1 --> 1 --> 1FIM

```
print('-' * 25)
print('Sequência de Fibonacci')
print('-' * 25)
n = int(input('Quantos termos você quer mostrar? '))
t1 = 0
t2 = 1
print('~'* 25)
print('{} --> {}'.format(t1, t2), end='')
cont = 3
while cont <= n:
    t3 = t1 + t2
    print(' --> {}'.format(t3), end='')
    t1 = t2
    t2 = t3
    cont += 1
print(' --> FIM')
```
> Quantos termos você quer mostrar? 10
> 
> 0 --> 1 --> 1 --> 2 --> 3 --> 5 --> 8 --> 13 --> 21 --> 34 --> FIM

### Validando Valores
```
while num != 999:
    num = int(input('Digite um número [999 para parar]: '))
print('Acabou! ')
```
> ERRO

```
num = 0
while num != 999:
    num = int(input('Digite um número [999 para parar]: '))
print('Acabou! ')
```
> Funciona, mas é uma improvisação
> 
> Digite um número [999 para parar]: 3
> 
> Digite um número [999 para parar]: 6
> 
> Digite um número [999 para parar]: 999
> 
> Acabou!

```
num = 0
cont = 0
while num != 999:
    num = int(input('Digite um número [999 para parar]: '))
    cont += 1 # cont = cont + 1
print('Você digitou {} números'.format(cont))
```
> Conta os números digitados, inclusive o 999
> 
> Digite um número [999 para parar]: 2
> 
> Digite um número [999 para parar]: 3
> 
> Digite um número [999 para parar]: 5
> 
> Digite um número [999 para parar]: 999
> 
> Você digitou 4 números

```
num = 0
cont = 0
soma = 0
# num = cont = soma = 0
while num != 999:
    num = int(input('Digite um número [999 para parar]: '))
    cont += 1 # cont = cont + 1
    soma += num # soma = soma + num
print('Você digitou {} números e a soma entre eles foi {}'.format(cont, soma))
```
> Soma os números digitados, inclusive o 999
> 
> Digite um número [999 para parar]: 2
> 
> Digite um número [999 para parar]: 6
> 
> Digite um número [999 para parar]: 999
> 
> Você digitou 3 números e a soma entre eles foi 1007

```
num = 0
cont = 0
soma = 0
# num = cont = soma = 0
while num != 999:
    num = int(input('Digite um número [999 para parar]: '))
    cont += 1 # cont = cont + 1
    soma += num # soma = soma + num
print('Você digitou {} números e a soma entre eles foi {}'.format(cont - 1, soma - 999))
```
> Funciona, mas é um improviso
> 
> Digite um número [999 para parar]: 2
> 
> Digite um número [999 para parar]: 4
> 
> Digite um número [999 para parar]: 999
> 
> Você digitou 2 números e a soma entre eles foi 6

```
num = 0
cont = 0
soma = 0
# num = cont = soma = 0
num = int(input('Digite um número [999 para parar]: '))
while num != 999:
    cont += 1 # cont = cont + 1
    soma += num # soma = soma + num
    num = int(input('Digite um número [999 para parar]: '))
print('Você digitou {} números e a soma entre eles foi {}'.format(cont, soma))
```
> Digite um número [999 para parar]: 2
> 
> Digite um número [999 para parar]: 3
> 
> Digite um número [999 para parar]: 5
> 
> Digite um número [999 para parar]: 999
> 
> Você digitou 3 números e a soma entre eles foi 10

### Maior e Menor, Média e While
```
resp = 'S'
soma = quant = media = 0
while resp in 'Ss':
    num = int(input('Digite um número: '))
    soma += num
    quant += 1
    resp = str(input('Quer continuar? [S/N] ')).upper().strip()[0]
media = soma / quant
print('Você digitou {} números e a média foi {}'.format(quant, media))
```
> Digite um número: 2
> 
> Quer continuar? [S/N] s
> 
> Digite um número: 4
> 
> Quer continuar? [S/N] n
> 
> Você digitou 2 números e a média foi 3.0

```
resp = 'S'
soma = quant = media = maior = menor = 0
while resp in 'Ss':
    num = int(input('Digite um número: '))
    soma += num
    quant += 1
    if quant == 1:
        maior = menor = num
    else:
        if num > maior:
            maior = num
        if num < menor:
            menor = num
    resp = str(input('Quer continuar? [S/N] ')).upper().strip()[0]
media = soma / quant
print('Você digitou {} números e a média foi {}'.format(quant, media))
print('O maior valor foi {} e o menor valor foi {}'.format(maior, menor))
```
> Digite um número: 2
> 
> Quer continuar? [S/N] s
> 
> Digite um número: 4
> 
> Quer continuar? [S/N] s
> 
> Digite um número: 6
> 
> Quer continuar? [S/N] n
> 
> Você digitou 3 números e a média foi 4.0
> 
> O maior valor foi 6 e o menor valor foi 2

## Interrompendo repetições while
```
cont = 1
while cont <= 10:
    print(cont, '-> ', end='')
    cont += 1
print('Acabou')
```
> 1 -> 2 -> 3 -> 4 -> 5 -> 6 -> 7 -> 8 -> 9 -> 10 -> Acabou

```
cont = 1
while True:
    print(cont, ' -> ', end='')
    cont += 1
print('Acabou')
```
> LOOP INFINITO

```
n = 0
while n != 999:
    n = int(input('Digite um número: '))
```
> Digite um número: 10
> 
> Digite um número: 20
> 
> Digite um número: 30
> 
> Sem um indicativo de pausa, vai pedir para digitar números em loop

```
n = cont = 0
while cont < 3:
    n = int(input('Digite um número: '))
    cont += 1
```
> Digite um número: 2
> 
> Digite um número: 2
> 
> Digite um número: 2

```
n = s = 0
while n != 999:
    n = int(input('Digite um número: '))
    s += n
print('A soma vale {}'.format(s))
```
> Digite um número: 2
> 
> Digite um número: 3
> 
> Digite um número: 5
> 
> Digite um número: 999
> 
> A soma vale 1009
> 
> o 999 é o flag (o ponto de parada), mas ele é somado também
> 
> poderia resolver colocando a gambiarra s -= 999, mas é só um improviso

```
n = s = 0
while True:
    n = int(input('Digite um número: '))
    if n == 999:
        break
    s += n
print(f'A soma vale {s}') ou print('A soma vale {}'.format(s))
```
> Digite um número: 2
> 
> Digite um número: 3
> 
> Digite um número: 999
> 
> A soma vale 5

```
nome = 'José'
idade = 33
print(f'O {nome} tem {idade} anos') #PYTHON última versão
print('O {} tem {} anos'.format(nome, idade)) #PYTHON ANTIGO
print('O %s tem %d anos' % (nome, idade)) #PYTHON MAIS ANTIGO
salario = 987.35
print(f'O {nome} tem {idade} anos e ganha R${salario:.2f}')
print(f'O {nome:^20} tem {idade} anos e ganha R${salario:.2f}')
```

> O José tem 33 anos
> 
> O José tem 33 anos
> 
> O José tem 33 anos
> 
> O José tem 33 anos e ganha R$987.35
> 
> O         José         tem 33 anos e ganha R$987.35

### Vários números com flag
```
num = soma = 0
while num != 999:
    num = int(input('Digite um valor (999 para parar): '))
    soma += num
print(f'A soma dos valores foi {soma}!')
```
> Soma o 999 junto
> 
> Digite um valor (999 para parar): 22
> 
> Digite um valor (999 para parar): 33
> 
> Digite um valor (999 para parar): 999
> 
> A soma dos valores foi 1054!

```
num = soma = 0
while num != 999:
    num = int(input('Digite um valor (999 para parar): '))
    soma += num
soma -= 999
print(f'A soma dos valores foi {soma}!')
```
> Gambiarra para não somar o 999, mas não é bom
> 
> Digite um valor (999 para parar): 2
> 
> Digite um valor (999 para parar): 6
> 
> Digite um valor (999 para parar): 999
> 
> A soma dos valores foi 8!

```
soma = 0
while True:
    num = int(input('Digite um valor (999 para parar): '))
    soma += num
print(f'A soma dos valores foi {soma}!')
```
> LOOP INFINITO

```
soma = cont = 0
while True:
    num = int(input('Digite um valor (999 para parar): '))
    if num == 999:
        break
    cont += 1
    soma += num
print(f'A soma dos {cont} valores foi {soma}!')
```
> Digite um valor (999 para parar): 3
> 
> Digite um valor (999 para parar): 66
> 
> Digite um valor (999 para parar): 999
> 
> A soma dos 2 valores foi 69!

> Se colocar cont e soma antes do if, eles seriam contados também

### Tabuada 3.0
```
while True:
    n = int(input('Quer ver a tabuada de qual valor? '))
    print('-' * 30)
    for c in range(1, 11):
        print(f'{n} x {c} = {n * c}')
    print('-' * 30)
```
> CONTINUA EM LOOP INDEFINIDAMENTE
> 
> Quer ver a tabuada de qual valor? 2
> 
> ------------------------------
> 
> 2 x 1 = 2
> 
> 2 x 2 = 4
> 
> 2 x 3 = 6
> 
> 2 x 4 = 8
> 
> 2 x 5 = 10
> 
> 2 x 6 = 12
> 
> 2 x 7 = 14
> 
> 2 x 8 = 16
> 
> 2 x 9 = 18
> 
> 2 x 10 = 20
> 
> ------------------------------
> 
> Quer ver a tabuada de qual valor? 3

```
while True:
    n = int(input('Quer ver a tabuada de qual valor? '))
    if n < 0:
        break
    print('-' * 30)
    for c in range(1, 11):
        print(f'{n} x {c} = {n * c}')
    print('-' * 30)
print('PROGRAMA TABUADA ENCERRADO!')
```
> Quer ver a tabuada de qual valor? 2
> 
> ------------------------------
> 
> 2 x 1 = 2
> 
> 2 x 2 = 4
> 
> 2 x 3 = 6
> 
> 2 x 4 = 8
> 
> 2 x 5 = 10
> 
> 2 x 6 = 12
> 
> 2 x 7 = 14
> 
> 2 x 8 = 16
> 
> 2 x 9 = 18
> 
> 2 x 10 = 20
> 
> ------------------------------
> 
> Quer ver a tabuada de qual valor? -1
> 
> PROGRAMA TABUADA ENCERRADO!

### Par ou Ímpar
```
from random import randint
v = 0
while True:
    jogador = int(input('Diga um valor: '))
    computador = randint(0, 11)
    total = jogador + computador
    tipo = ' '
    while tipo not in 'PI':
        tipo = str(input('Par ou Ímpar? [P/I] ')).strip().upper()[0]
    print(f'Você jogou {jogador} e o computador {computador}. Total de {total}. ', end='')
    print('DEU PAR!' if total % 2 == 0 else 'DEU ÍMPAR!')
    if tipo == 'P':
        if total % 2 == 0:
            print('Você VENCEU!')
            v += 1
        else:
            print('Você PERDEU!')
            break
    elif tipo == 'I':
        if total % 2 == 1:
            print('Você VENCEU!')
            v += 1
        else:
            print('Você PERDEU!')
            break
    print('Vamos jogar novamente...')
print(f'GAME OVER! Você venceu {v} vezes.')
```
> Diga um valor: 2
> 
> Par ou Ímpar? [P/I] p
> 
> Você jogou 2 e o computador 1. Total de 3. DEU ÍMPAR!
> 
> Você PERDEU!
> 
> GAME OVER! Você venceu 0 vezes.

> Diga um valor: 2
> 
> Par ou Ímpar? [P/I] i
> 
> Você jogou 2 e o computador 11. Total de 13. DEU ÍMPAR!
> 
> Você VENCEU!
> 
> Vamos jogar novamente...
> 
> Diga um valor: 5
> 
> Par ou Ímpar? [P/I] i
> 
> Você jogou 5 e o computador 3. Total de 8. DEU PAR!
> 
> Você PERDEU!
> 
> GAME OVER! Você venceu 2 vezes.

### Análise de dados do grupo
```
tot18 = totH = totM20 = 0
while True:
    idade = int(input('Idade: '))
    sexo = ' '
    while sexo not in 'MF':
        sexo = str(input('Sexo: [M/F] ')).strip().upper()[0]
    if idade >= 18:
        tot18 += 1
    if sexo == 'M':
        totH += 1
    if sexo == 'F' and idade < 20:
        totM20 += 1
    resp = ' '
    while resp not in 'SN':
        resp = str(input('Quer continuar? [S/N] ')).strip().upper()[0]
    if resp == 'N':
        break
print(f'Total de pessoas com mais de 18 anos: {tot18}')
print(f'Ao todo temos {totH} homens cadastrados. ', end='')
print(f'E temos {totM20} mulheres com menos de 20 anos.')
```
> Idade: 19
> 
> Sexo: [M/F] m
> 
> Quer continuar? [S/N] s
> 
> Idade: 20
> 
> Sexo: [M/F] f
> 
> Quer continuar? [S/N] n
> 
> Total de pessoas com mais de 18 anos: 2
> 
> Ao todo temos 1 homens cadastrados. E temos 0 mulheres com menos de 20 anos.

### Estatística em produtos
```
total = totmil = menor = cont = 0
barato = ' '
while True:
    produto = str(input('Nome do Produto: '))
    preco = float(input('Preço: R$ '))
    cont += 1
    total += preco
    if preco > 1000:
        totmil += 1
    if cont == 1:
        menor = preco
        barato = produto
    else:
        if preco < menor:
            menor = preco
            barato = produto
    resp = ' '
    while resp not in 'SN':
        resp = str(input('Quer continuar? [S/N] ')).strip().upper()[0]
    if resp == 'N':
        break
print('{:-^40}'.format('FIM DO PROGRAMA'))
print(f'O total da compra foi R$ {total:.2f}')
print(f'Temos {totmil} produtos custanddo mais do que R$ 1.000,00')
print(f'O produto de menor preço foi {barato} e custa R$ {menor:.2f}')
```
```
if cont == 1:
        menor = preco
        barato = produto
    else:
        if preco < menor:
            menor = preco
            barato = produto
```
> PODE SER SUBSTITUÍDO POR: 
```
if cont == 1 or preco < menor:
        menor = preco
        barato = produto
```
> Nome do Produto: Playstation
> 
> Preço: R$ 1500
> 
> Quer continuar? [S/N] s
> 
> Nome do Produto: RelógioPreço: R$ 10400
> 
> Quer continuar? [S/N] s
> 
> Nome do Produto: Jogo de prato
> 
> Preço: R$ 50
> 
> Quer continuar? [S/N] n
> 
> ------------FIM DO PROGRAMA-------------
> 
> O total da compra foi R$ 11950.00
> 
> Temos 2 produtos custanddo mais do que R$ 1.000,00
> 
> O produto de menor preço foi Jogo de prato e custa R$ 50.00

### Simulador de Caixa Eletrônico
```
print('=' * 30)
print('{:^30}'.format('Banco Cev'))
print('=' * 30)
valor = int(input('Que valor você quer sacar? R$ '))
total = valor
ced = 50
totced = 0
while True:
    if total >= ced:
        total -= ced
        totced += 1
    else:
        if totced > 0:
            print(f'Total de {totced} cédulas de R$ {ced}')
        if ced == 50:
            ced = 20
        elif ced == 20:
            ced = 10
        elif ced == 10:
            ced = 1
        totced = 0
        if total == 0:
            break
print('=' * 30)
print('Volte sempre ao Banco Cev')
```
> ==============================
> 
>          Banco Cev           
>          
> ==============================
> 
> Que valor você quer sacar? R$ 575
> 
> Total de 11 cédulas de R$ 50
> 
> Total de 1 cédulas de R$ 20
> 
> Total de 5 cédulas de R$ 1
> 
> ==============================
> 
> Volte sempre ao Banco Cev
