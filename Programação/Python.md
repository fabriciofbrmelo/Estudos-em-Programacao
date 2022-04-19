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

Seno, cosseno e tangente
'''import math
an = float(input('Digite o ângulo que você deseja: '))
seno = math.sin(math.radians(an))
cosseno = math.cos(math.radians(an))
tangente = math.tan(math.radians(an))
print('O ângulo de {:.2f} tem \n o seno de {:.2f}, \n o cosseno de {:.2f} \n e a tangente de {:.2f}'.format(an, seno, cosseno, tangente))'''

from math import radians, sin, cos, tan
an = float(input('Digite o ângulo que você deseja: '))
seno = sin(radians(an))
cosseno = cos(radians(an))
tangente = tan(radians(an))
print('O ângulo de {:.2f} tem \n o seno de {:.2f}, \n o cosseno de {:.2f} \n e a tangente de {:.2f}'.format(an, seno, cosseno, tangente))

Bháskara
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

    print('x1: {}, x2: {}'.format(x1, x2)
