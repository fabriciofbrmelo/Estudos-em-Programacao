Soma
n1 = int(input('Digite um valor: '))
n2 = int(input('Digite um valor: '))
s = n1 + n2
# print('A soma entre', n1, 'e', n2, 'vale', s)
print('A soma entre {} e {} vale {}'.format(n1, n2, s))

a = input('Digite algo: ')
print('O tipo primitivo desse valor é: ', type(a))
print('Só tem espaços? ', a.isspace())
print('É um número? ', a.isnumeric())
print('É alfabético? ', a.isalpha())
print('É alfanumérico? ', a.isalnum())
print('Está em maiúsculas? ', a.isupper())
print('Está em minúsculas? ', a.islower())
print('Está capitalizada? ', a.istitle())

Operadores Aritméticos
1 = int(input('Um valor: '))
n2 = int(input('Outro valor: '))
s = n1 + n2
m = n1 * n2
d = n1 / n2
di = n1 // n2
e = n1 ** n2
print('A soma é {}, \n o produto é {} e a \n divisão é {:.3f}'.format(s, m, d), end= '>>>')
print('Divisão inteira {} e potência {}'.format(di, e))

