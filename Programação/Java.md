# Java

## Curso do Google - Grasshopper
Link para o Curso --> [Link](https://grasshopper.app/pt_br/)

<details><summary>Índice</summary>
 
|Título|Conteúdo|
|------|--------|
|Funções|Argumento, Expressão de Função, Função() {}, ()=>{}, Declaração de Variável, Identificadores|
|Strings|str, num, boolean|
|Variáveis|var, const, let|
|Estrutura de dados||
|Arrays|[], {}, Propriedades, Encadeamento, Indexação da Array|
|IF|if statement, operador de igualdade, multiplicação, divisão, soma, subtração|
|Bloco de Código||
|IF...ELSE||
|Operadores|Matemática Operadora: mais, menos, multiplicação, divisão, módulo, operador e &&, operador ou |
|Laços|Laços de Strings: for...of, while, for; Laços Aninhados|
|Objeto|Atribuições, Atualizações, Expressão Binária|
 
</details>

## Funções

```
- drawBox() é uma função. Uma função diz a um computador para fazer uma determinada coisa.
As funções podem receber argumentos para fornecer informações extras ao computador.
Por exemplo, drawBox(red) tem red como seu argumento, isso diz ao computador que ele deve desenhar uma caixa vermelha.
- drawBox() é o nome da função. Ao adicionar blue entre parênteses (), você está chamando a função com o argumento blue.
Este código cria uma caixa azul.
```

### 1. Argumento
--> Um argumento é uma informação extra fornecida a uma função que diz como ela deve ser executada. Os argumentos são colocados entre parênteses de uma chamada de função. Nem todas as funções requerem argumentos e algumas funções requerem vários argumentos.

```
CÓDIGO DE EXEMPLO
drawBox(red);
print('hello');
```

--> Neste exemplo, red é o argumento para a função drawBox(). Ele diz à função para desenhar uma caixa vermelha.
'hello' é o argumento para a função print(). Ele diz à função o que deve ser impresso.

### 2. Expressão de Função
--> Executa uma sequência de comandos quando chamada. Ela tem três partes:
i. O valor do identificador (o nome da função)
ii. Os parâmetros ou argumentos (os valores entre parênteses)
iii. O corpo da função, que é a sequência de comandos executados quando a função é chamada.

```
CÓDIGO DE EXEMPLO
var printSum = function(num1, num2) {
    print(num1 + num2);
}; 
    printSum(5, 2);
```

Quando printSum(5, 2) é chamado, será impresso 7 na área de saída.

### 3. Função() {}
--> Uma função executa alguma ação ou tarefa definida em seu bloco {}. A parte do código onde a função é criada é chamada a declaração da função. Para usar ou chamar esta função, seu nome é usado entre parênteses ().

```
CÓDIGO DE EXEMPLO
function printSum(num1, num2) {
         print(num1 + num2);}
printSum(5, 2);
```
 
A palavra-chave function cria uma nova função chamada printSum() que recebe dois argumentos. Quando printSum() é chamada, ela soma os dois argumentos.

### 3.1. () => {}
--> Uma função de seta é uma forma compacta de criar uma nova função. Ela usa () => {} em vez da palavra-chave function. Também não precisa de um nome. A melhor prática é usar => em vez da palavra-chave function.

```
CÓDIGO DE EXEMPLO
var add = (num1, num2) => {
    return num1 + num2;};
console.log(add(5, 3));
```

add() aceita dois números como argumentos e os adiciona.

### 4. Declaração de Variável
--> Variáveis são muito comuns na programação. Elas permitem que você faça referência à mesma informação várias vezes. Em JavaScript, as variáveis podem ser definidas usando var e dando à variável um nome exclusivo. Por exemplo, var myVariable = 'my example'.

```
CÓDIGO DE EXEMPLO
var appName = 'Grasshopper';
```

appName pode ser usado no futuro sempre que você quiser "Grasshopper".

### 5. Identificadores
--> Um identificador é um nome que você pode definir para fazer referência ao seu código. Você pode nomear um identificador como quiser, desde que não seja uma palavra-chave JavaScript existente.

```
CÓDIGO DE EXEMPLO
drawBox(red);
```

drawBox e red são identificadores. Eles foram definidos previamente para você.

## Strings

### 1. Str
--> Letras, palavras e frases são chamadas de strings na programação. As aspas são usadas para mostrar o início e o fim de uma string. Por exemplo, 'hello world' é uma string.

```
CÓDIGO DE EXEMPLO
drawBoxes('royg');
```

'royg' é uma string usada na função drawBoxes() para criar caixas vermelhas, laranja, amarelas e verdes.

### 2. Num
--> Um número que pode ser inteiro (como 10) ou decimal (como 3,5).

```
CÓDIGO DE EXEMPLO
var numberOfApples = 10;
var temperature = 74.6;
```

A variável numberOfApples armazena o inteiro (número inteiro) 10. A variável temperature armazena o decimal 74,6.

### 3. Boolean
--> Um boolean é um dos dois valores especiais em JavaScript, true ou false. Eles são úteis para lidar com estados que possuem apenas duas possibilidades.

```
CÓDIGO DE EXEMPLO
var isLearningToCode = true; var shouldWearSocksWithSandals = false;
```

É true que você está aprendendo a programar, mas é false que se deva usar meias com sandálias.

## Variáveis

### 1. Variáveis
--> Uma forma de armazenar um valor para uso posterior, também conhecido como variável. Uma var deve ter um nome (também conhecido como identificador) e, opcionalmente, pode ser atribuído um valor, que pode ser um número, uma string ou um dado mais complexo.

```
CÓDIGO DE EXEMPLO
var cityOfOrigin = 'Pittsburgh';
var cityOfDestination;
cityOfDestination = 'Manila';
```

cityOfOrigin é uma variável que será igual a 'Pittsburgh'. Em seguida, outra variável chamada cityOfDestination é criada e mais tarde recebe um novo valor de 'Manila'.

### 2. Const
--> Um tipo de variável que uma vez criada não pode ser reatribuída. Novos dados ainda podem ser adicionados a variáveis const que são objetos ou arrays, mas não podem ser reatribuídos.

```
CÓDIGO DE EXEMPLO
const arrayOfNumbers = [1, 2, 3];
arrayofNumbers.push(4);
```

arrayOfNumbers não pode ser reatribuída, mas podem ser adicionados novos dados.

### 3. let
--> let declara uma variável como var, exceto que tem um escopo diferente. O escopo de uma variável é a seção do código onde ela pode ser usada. Um let só pode ser usado dentro do bloco de código {}onde é criado.

```
CÓDIGO DE EXEMPLO
var x = 100;
if (x > 0) {
   let x = 25;  
}
print(x);
```

Uma variável chamada x é criada usando var e definida como 100. A if statement é verdadeira, então a variável let x é criada e definida como 25. A variável let permanece dentro do bloco de código {}. A print(x), que está fora do bloco de código da if statement, usa o valor de var x = 100.

## Estrutura de dados

Estruturas de dados são maneiras de armazenar e organizar dados mais complexos do que apenas um único valor primitive. Em JavaScript, os tipos de estrutura de dados mais comuns são arrays e objects.

```
CÓDIGO DE EXEMPLO
var vegetables = ['broccoli', 'carrots', 'spinach'];
var groceries = {
    numberOfApples: 5,
    numberOfBananas: 5,    
vegetables: vegetables
};
```

Observe que um objeto pode conter arrays e vice-versa. Nesse caso, groceries.vegetables seria igual à variável vegetables.

## Arrays

### 1. []
--> Em JavaScript, uma array é uma lista de itens. Os itens podem ser diferentes tipos de dados: números, strings e até mesmo outras arrays. Uma array dentro de outra array é chamada de aninhamento de arrays.

```
CÓDIGO DE EXEMPLO
var exampleArray = ['blue', 'orange', 5, 10, [50, 10]];
```

exampleArray tem 5 itens. Ela contém strings, números e uma array; que tem dois itens que são números.

### 2. {}
--> Um objeto armazena vários valores que possuem nomes de propriedade (ou chave). Isso permite que eles sejam facilmente acessados posteriormente no código.

```
CÓDIGO DE EXEMPLO 
var groceries = { 
    apples: 5,    
    bananas: 2    
};
```
apples e bananas são propriedades do objeto groceries. 5 e 2 são os valores associados a essas propriedades. groceries.apples, por exemplo, é igual a 5.

### 3. Propriedades
--> Um objeto pode armazenar várias informações dentro de uma variável. A notação de ponto é usada para acessar uma propriedade de um objeto. Por exemplo, objectName.propertyName.

```
CÓDIGO DE EXEMPLO
var objectName = {
    propertyName: 'Coding is fun.',
    otherPropertyName: 'this is also a key value'
};
print(objectName.propertyName);
```

Este código imprimirá 'Coding is fun.'

### 4. Encadeamento
--> O encadeamento permite que os programadores apliquem várias chamadas de função diferentes ao mesmo identificador.

```
CÓDIGO DE EXEMPLO
svg.append('circle')
   .attr('fill', 'blue')
   .attr('r', 200);
```

Um círculo SVG é criado com um atributo de azul para seu preenchimento e um raio de 200 aplicado ao mesmo tempo usando .append() e duas chamadas de função .attr() encadeadas.

### 5. Indexação da array
--> Na maioria das linguagens de programação, incluindo JavaScript, as arrays são indexadas a partir de 0. O primeiro item em uma array tem o índice 0. Por exemplo, myArray[0] acessa o primeiro item. Enquanto myArray[3] acessa o 4º item.

```
CÓDIGO DE EXEMPLO
var groceries = ['apples', 'bananas', 'oranges']; 
var fruit = groceries[1];
```

A variável fruit contém o segundo item da array, que é 'bananas'.

## IF

### 1. If Statement
--> As if statements permitem que você execute uma seção específica do código quando um teste for verdadeiro. O código entre parênteses () é o teste. Se o teste for verdadeiro, o código dentro do bloco {} será executado. Se o teste não for verdadeiro, o código dentro do bloco não será executado.

```
CÓDIGO DE EXEMPLO
var aNumber = 5;
if (aNumber === 5) {
   drawBox(blue);
}
if (aNumber === 4) {
   drawBox(red);
}
```

Nesse exemplo, a variável aNumber recebe o número 5. Existem duas if statements. A primeira é verificar se aNumber é igual a 5. A segunda é verificar se é igual a 4. Apenas o primeiro teste if statement é verdadeiro, então seria desenhada uma caixa azul.

### 2. Operador de Igualdade
--> Compara se duas coisas são iguais entre si.

```
CÓDIGO DE EXEMPLO
print(10 === 5);
print(5 === 5);
```

Esse código primeiro verifica se 10 é igual a 5. Como 10 é diferente de 5, é impresso false. O código então verifica se 5 é igual a 5. Como 5 é igual a 5, é impresso true.
- !== diferente
- <= menor igual
- (>=) maior igual (coloquei parênteses para não virar código)

### (=)
Define (ou redefine) o valor armazenado em uma variável. À esquerda está a variável que você gostaria de ajustar e à direita está o novo valor.

```
CÓDIGO DE EXEMPLO
var myNumber = 10;
```

### (*=)
Multiplica o valor associado à variável à esquerda pelo valor à direita e atribui o valor resultante à variável existente.

```
CÓDIGO DE EXEMPLO
var myNumber = 10;
myNumber *= 5;
```

myNumber será igual a 50.

### (/=)
Divide o valor associado à variável à esquerda pelo valor à direita e atribui o valor resultante à variável existente.

```
CÓDIGO DE EXEMPLO
var myNumber = 10;
myNumber /= 5;
```

myNumber será igual a 2.

### (+=)
Adiciona o valor associado à variável à esquerda com o valor à direita e atribui o valor resultante à variável existente.

```
CÓDIGO DE EXEMPLO
var myNumber = 10;
myNumber += 5;
```

myNumber será 15

### (-=)
Subtrai o valor associado à variável à esquerda pelo valor à direita e atribui o valor resultante à variável existente.

```
CÓDIGO DE EXEMPLO
var myNumber = 10;
myNumber -= 5;
```

mynumber será 5

### 3. Bloco d Código
--> Uma sequência de comandos agrupados dentro de chaves {}.

```
CÓDIGO DE EXEMPLO
if (learningToCode === 'fun') {
   print('Coding is awesome!');
   print('I want to solve more puzzles!');
}
```

Se a variável learningToCode for igual a 'fun', o código dentro do bloco de código {} será executado.

### 4. IF... ELSE
--> As declarações if...else realizam um teste para decidir qual código executar. Se o teste for verdadeiro, o bloco if {} será executado. Se o teste for falso, o bloco else {} será executado.

```
CÓDIGO DE EXEMPLO
var number = pickRandom(10);
if (number === 7) {
    print('The number is 7!');
} else {
    print('The number is not 7.');
}
```

Este código escolhe um número aleatório de 1 a 10. Se number for 7, ele imprimirá, 'The number is 7!'. Se number for qualquer outra coisa, ele imprimirá, 'The number is not 7.'

## Operadores

### Matemática Operadora

#### Operador Mais (+)
--> Soma dois valores. Esse operador é mais comumente usado em números e strings.

```
CÓDIGO DE EXEMPLO
var result = 10 + 5;
var fullName = 'Johnny' + ' Appleseed';
```

O valor de result é 15. O operador + pode combinar strings, então o valor de fullName é 'Johnny Appleseed'.

#### Operador Menos (-)
--> Subtrai o valor do lado direito do operador - do valor do lado esquerdo.

```
CÓDIGO DE EXEMPLO
var result = 10 - 5;
```

result conterá o número 5.

#### Operador Multiplicação (*)
--> Multiplica o valor do lado esquerdo pelo valor do lado direito.

```
CÓDIGO DE EXEMPLO
var result = 10 * 5;
```

10 é multiplicado por 5. A variável result contém o número 50.

#### Operador Divisão (/)
--> Divide o valor do lado esquerdo do operador / pelo valor do lado direito.

```
CÓDIGO DE EXEMPLO
var result = 10 / 5;
```

Divide 10 por 5. A variável result manterá o número 2.

#### Operador Módulo (%)
--> Frequentemente chamado de resto ou operador de módulo, % determina todo o valor restante quando o valor à esquerda for dividido pelo valor à direita.

```
CÓDIGO DE EXEMPLO
var result = 10 % 5;
var resultWithRemainder = 12 % 5;
```

result será igual a 0, e resultWithRemainder será igual a 2.

#### Operador e (&&)
--> Combina duas declarações em um valor true ou false. Torna-se true apenas se os lados esquerdo e direito forem ambos true, caso contrário, é false.

```
CÓDIGO DE EXEMPLO
if (1 < 2 && 5 > 0) {
   print('Yes!');
} else {
   print('No');
}
```

Como 1 é menor que 2 e 5 é maior que 0, o teste da if statement () é true e será impresso 'Yes!'.

#### Operador ou (||)
-->Combina duas declarações em um valor true oufalse. Torna-se true se o lado esquerdo ou direito for true, e só é false se os dois lados forem false.

```
CÓDIGO DE EXEMPLO
if (2 === 4 || 1+1 === 2) {
   print('At least one is true.');   
} else {
   print('Both are false.');
}
```

Embora 2 seja diferente de 4, 1 + 1 é igual a 2. Como o lado direito é verdadeiro, o teste da if statement () é verdadeiro e imprime, 'At least one is true.'

## Laços

--> Um laço repete as mesmas linhas de código indefinidamente. As linhas a serem repetidas são circundadas por chaves: {}. Existem diversas maneiras de executar um laço (principalmente em JavaScript).

```
CÓDIGO DE EXEMPLO
for (var element of [1, 2, 3, 4, 5]) {
    print(index);
    print('the loop will go through each number in the array');
}
var index = 0;
while (index < 5) {
index += 1;
print('the while loop will go as long as index is less than 5');
}
```

Os dois laços podem ser usados para obter o mesmo resultado. Em ambos os laços for...of e while, o laço se repetirá 5 vezes.

### Laços de Strings

#### 1. For ... of
--> Um laço repete a seção de código entre chaves {}. Em JavaScript, um laço for of percorre cada elemento em uma array ou string, repetindo o código para cada elemento.

```
CÓDIGO DE EXEMPLO
var groceries = ['apples', 'yogurt', 'toothpaste'];
for (var element of groceries) {
print(element);
}
```

Cada item na array groceries será impresso em sua própria linha.

#### 2. While
--> Um laço while executa o código dentro de seu bloco até que o teste entre parênteses não seja mais verdadeiro.

```
CÓDIGO DE EXEMPLO
let i = 0;
while (i < 3) {
      print('i is less than 3');
      i++;
}
print('i is now 3!');
```

Contanto que i seja menor que 3, o código no bloco de comandos será repetido. Se você esquecer de aumentar i neste código, o laço while se repetirá para sempre e causará uma falha.

#### 3. For
--> Em JavaScript, um laço for clássico repete o mesmo código dentro do bloco {} um número determinado de vezes. Ele é definido em três partes. A primeira parte acontece antes do início do laço e define uma variável de laço (var i = 0;). A segunda parte é um teste que determina se o laço deve continuar se repetindo (i < 10;). E a terceira parte atualiza a variável do laço cada vez que ele se repete (i = i + 1).

```
CÓDIGO DE EXEMPLO
for (var i = 0; i < 10; i = i + 1) {
    print(i);
    print('the loop will go as long as i is less than 10.');
}
```

Neste exemplo, a variável do laço (i) começa em 0. O código no {} continuará se repetindo enquanto i for menor do que 10. E i é aumentado em 1 a cada laço. Esse código imprime os números de 0 a 9.

### Laços Aninhados

--> Um laço aninhado é um laço dentro de outro laço. Embora os laços aninhados possam ser úteis, se você tiver muitos, pode tornar a execução do código lenta ou difícil de entender.

```
CÓDIGO DE EXEMPLO
for (var outerNumber of [1, 2, 3, 4, 5]) {
    for (var nestedNumber of [6, 7, 8, 9]) {    
        print(outerNumber, nestedNumber);       
    }
}
```

Esse código imprimiria 1,6, 1,7, 1,8 e 1,9. E então outerNumber mudará para 2, e o laço interno imprimirá 2,6, depois 2,7 e assim por diante.

## Objeto

### 1. Atribuições
--> Define (ou redefine) o valor armazenado em uma variável. À esquerda está a variável que você gostaria de ajustar, no meio está o operador e à direita está o valor que será aplicado ao operador, que resulta em um novo valor.

```
CÓDIGO DE EXEMPLO
var x = 2;
x += 2;
```

x será igual a 4 quando o código for executado.

### 2. Atualizações
--> Uma forma abreviada de atualizar o valor de uma variável usando algum tipo de arithmetic operator.

```
CÓDIGO DE EXEMPLO
var x = 5;
x++;
```

x será igual a 6.

### 3. Expressão Binária
--> Um operador que fica entre dois valores e calcula algum tipo de resultado a partir desses dois valores.

```
CÓDIGO DE EXEMPLO
var isEqual = x === 42;
```

Se x é um número e é igual a 42, a variável isEqual será true.

## Manipulação de Strings

### 1. Length
--> Strings e Arrays têm uma propriedade .length. Para uma string, isso representa o número total de caracteres. Para arrays, isso representa o número total de elementos.

```
CÓDIGO DE EXEMPLO
var sentence = 'Some text.';
    print(sentence.length);


var list = ['hi', 1, sentence];
    print(list.length);
```

O 1º comando de impressão imprimirá 10, pois há 8 letras, 1 espaço e 1 ponto final na string sentence. O 2º comando de impressão imprimirá 3, pois há 3 elementos dentro da array list.

### 2. Includes
--> Quando o método .includes() é aplicado a uma string (ou array), ele verifica se o valor entre parênteses pode ser encontrado dentro da string (ou array). Retorna verdadeiro se encontrar o valor e falso se não encontrar.

```
CÓDIGO DE EXEMPLO
var words = 'haystackneedlehaystack';
console.log(words.includes('needle'));

var list = ['i', 4, 'e'];
console.log(list.includes('e'));
```

O 1º resultado será true porque a string, 'needle', pode ser encontrada dentro de 'haystackneedlehaystack'. O 2º resultado também é true porque 'e' está dentro da array, no índice 2.

### 3. Replace
--> O método .replace() pode ser anexado a uma string para alterar uma seção dela. O 1º argumento será usado para encontrar a 1ª correspondência exata e, em seguida, o 2º argumento a substituirá.

```
CÓDIGO DE EXEMPLO
var quote = 'Never say never';
quote = quote.replace('never', 'goodbye');
print(quote);
```

O método .replace() procura por 'never' na citação. É sensível a maiúsculas e minúsculas, então o resultado final é Never say goodbye.

### 4. Variáveis Globais e Locais
--> Na programação, o escopo determina onde uma variável está acessível. As variáveis podem ter escopo ***global*** ou ***local***.

i. Uma variável global pode ser usada em todo o código. A chave var geralmente cria variáveis globais. 
ii. Uma variável local só pode ser usada dentro do bloco onde é declarada. A chave let permite que você crie variáveis locais.


No código abaixo, a variável myLocalNumber é declarada usando a chave let. Isso significa que ele só existe dentro do bloco da if statement. O impossibleCalculation não funcionará porque a variável myLocalNumber não existe fora da if statement.

```
var myGlobalNumber = 5;
    if (myGlobalNumber > 3) { 
    let myLocalNumber = 4; 
} 
var impossibleCalculation = myGlobalNumber + myLocalNumber
```

A chave var geralmente cria variáveis globais. A chave let permite que você crie variáveis locais.

### 5. Operador Ternário (?)
--> Operadores ternários são uma maneira de escrever if...else statements com menos código. Eles começam com o teste e, depois do símbolo ?, é o código rodado se o teste for verdadeiro. A última parte, após o símbolo :, é o código que será rodado se o teste for falso.

```
CÓDIGO DE EXEMPLO
if (1 === 1) {
    print('all is right in the universe');
} else {
    print('something is wrong...');
}

1 === 1 ? print('all is right in the universe') : print('something is wrong...');

```

Veja um exemplo de uma if...else statement testando se 1 é igual a 1; e o mesmo código usando um operador ternário.

### 6. Incremento (++)
--> Adiciona 1 a um valor numérico existente.

```
CÓDIGO DE EXEMPLO
var counter = 1;
counter++;
counter será igual a 2.
```

### 7. Decremento (--)
--> Subtrai 1 de um valor numérico existente.

```
CÓDIGO DE EXEMPLO
var counter = 2;
counter--;
```

counter será igual a 1.

### 8. (+=)
--> Adiciona o valor associado à variável à esquerda com o valor à direita e atribui o valor resultante à variável existente.

```
CÓDIGO DE EXEMPLO
var myNumber = 10;
myNumber += 5;
```

myNumber será igual a 15.

### 9. (-=)
--> Subtrai o valor associado à variável à esquerda pelo valor à direita e atribui o valor resultante à variável existente.

```
CÓDIGO DE EXEMPLO
var myNumber = 10;
myNumber -= 5;
```

myNumber será igual a 5.

### 10. (*=)
--> Multiplica o valor associado à variável à esquerda pelo valor à direita e atribui o valor resultante à variável existente.

```
CÓDIGO DE EXEMPLO
var myNumber = 10;
myNumber *= 5;
```

myNumber será igual a 50

### 11. Console
--> O console é um objeto exibido como texto quando você roda seu código. O lugar onde o texto está também é conhecido como console.

```
CÓDIGO DE EXEMPLO
console.log('test string');
```

Este código escreverá 'test string' no console.

### 12. Log
--> O método .log() é usado para escrever o resultado de texto no console. console.log() funciona da mesma maneira que print(), mas console.log() também funciona fora do Grasshopper.

```
CÓDIGO DE EXEMPLO
console.log('Start the code!');
let x = 10;
console.log(x);
```

O código imprimirá:
> 'Start the code!'
> 
> 10 

## FUNÇÕES

### 1. Return
--> Quando uma função é concluída, a saída pode ser enviada de volta para o local de onde foi chamada. Para isso, é usada a palavra-chave return.

```
CÓDIGO DE EXEMPLO
function sumNumbers(a, b) {
    var answer = a + b;
    return answer;
}

print(sumNumbers(3, 5));
```

A função print() chama a função sumNumbers com os argumentos 3 e 5. sumNumbers soma os argumentos e envia o resultado de volta usando return. O comando print() obtém a resposta e, em seguida, imprime o número 8.

### 2. Recursão
--> Recursão é quando uma função chama a si mesma a partir de sua própria definição. Deve haver sempre uma condição final, ou caso básico, para que a função não continue chamando ela mesma para sempre.

```
CÓDIGO DE EXEMPLO
function ftl(n) {
    if (n === 1) {
        return 1;
    }
    return n * ftl(n - 1);
}

console.log(ftl(3));
```

A função ftl pega um número n e multiplica por todos os números inteiros antes dele. Portanto, o ftl(3) é 3 2 1. Cada vez que essa função efetua a recursão, ela subtrai 1 do valor do argumento até que o caso básico de n === 1 seja encontrado. ftl(3)→(3 * ftl(2)) ftl(2)→(2 * ftl(1)) ftl(1)→ 1 Portanto, ftl(3) retorna (3 * ( 2 * (1))) que é 6.

### 3. True
--> true é um valor booleano. O outro valor booleano é false. No código, se o teste de uma if statement () for true então o código no bloco {} será rodado.

```
CÓDIGO DE EXEMPLO
if (true) {
    print('yes');
}
var question = 1 + 1=== 2;
if (question) {
    print('yes again');
}
```

Este código imprimirá 'sim' e 'sim novamente'. O código entre parênteses () da if statement é o teste. Se o teste for verdadeiro, o código das chaves {} será rodado. true é verdadeiro, então é impresso "sim". Para a question, como 1 + 1 é igual a 2, question está armazenando o valor true.

### 4. False
--> false é um valor booleano. O outro valor booleano é true. No código, se o teste de uma if statement () for false então o código no bloco {} não será rodado.

```
CÓDIGO DE EXEMPLO
var equation = 1 === 2;
if (equation === false) {
    print("The equation is false.");
}
if (false) {
    print("This will never print.");
}
```

Este código imprimirá, "A equação é falsa." Como 1 é diferente de 2, a variável equation armazena o valor false. A 1ª if statement verifica se o valor da equation é false, e é, então o 1º comando de impressão é rodada.

### 5. Retorno de Chamada
--> Quando uma função é usada como argumento, ela é chamada de uma função de retorno de chamada. Funções que usam retorno de chamada são úteis por causa de sua flexibilidade, pois o código rodado pode se alterar dependendo de qual retorno de chamada é usado.

```
CÓDIGO DE EXEMPLO
let array = [2, 4, 6];
function print(num) {
    console.log(num);
}
array.forEach(print);
```

O método de array .forEach() leva a função de retorno de chamada print() como argumento e aplicará essa função a cada item da array.

## MANIPULAÇÃO DE ARRAY

### 1. Usar .length com um API
--> A array listOfDestinations é importada de uma API remota chamada 'grasshopper.travel'.

```
import { listOfDestinations } from 'grasshopper.travel';
let numberOfDestinations = listOfDestinations.length;
console.log('There are ' + numberOfDestinations + ' to choose from.');
```
Contar o número total de itens em uma array, nesse caso conta quantos locais tem no listOfDestinations.

### 2. Usar .slice de um array
--> Cria uma array que é um subconjunto de outra array. São necessários 2 argumentos para indicar onde a nova array começará e terminará (fim não incluído). Os argumentos usam indexação da array.

```
CÓDIGO DE EXEMPLO
var myArray = ['oranges', 'apples', 'bananas', 'carrots', 'milk'];
var newArray = myArray.slice(1, 3);
newArray será igual a ['apples', 'bananas'].
```

```
import { transportation } from 'grasshopper.travel';
let cities = [
  'London',
  'London',
  'London',
  'Lagos',
  'Lisbon',
  'Louisville',
  ___
];
console.log(cities.slice(2, 6));
console.log(transportation.slice(2, 6));
```

O método .slice() cria uma nova array copiando uma subseção de outra array. São necessários 2 argumentos: um índice de array onde começar a copiar e um índice onde terminar (fim não incluído).

### 3. .push
--> Adiciona um valor ao final de uma array.

```
CÓDIGO DE EXEMPLO
var myArray = [];
myArray.push(1);
```

myArray será igual a [1].

### 4. .pop
--> Remove um valor no final de uma array.

```
CÓDIGO DE EXEMPLO
var myArray = [5];
myArray.pop();
myArray ficará vazio assim que o código for rodado.
```

### 5. Operador de Propagação (...)
--> O operador de propagação é usado para adicionar todos os elementos individuais de uma array em outra array. Pode-se pensar nele como se os colchetes [] fossem retirados para que apenas os itens dentro dele permanecessem.

```
CÓDIGO DE EXEMPLO
let dogs = ['Retriever', 'Shepherd', 'Terrier'];
let pets = ['Hedgehog', ...dogs, 'Turtle'];
for (let animal of pets) {
    console.log(animal);
}
```

Sem o operador de propagação (...) antes de dogs, as 3 strings 'Retriever','Shepherd','Terrier' seriam impressas como um único item e o resultado seria:

> Hedgehog 
> 
> Retriever,Shepherd,Terrier 
> 
> Turtle 

Adicionar o operador de propagação (...dogs) transforma o resultado em 5 linhas separadas:

> Hedgehog
> 
> Retriever 
> 
> Shepherd 
> 
> Terrier 
> 
> Turtle 
