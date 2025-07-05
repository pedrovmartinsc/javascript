# Fundamentos do JavaScript Clássico

## INTEGRAÇÕES
~~~ html
./index.html

<!DOCTYPE html>

<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JavaScript</title>
</head>
<body>    
    <script defer>
        console.log("Hello World!");
    </script>
</body>

</html>
~~~

### Intengrar JavaScript de forma externa

- Criar diretório ***src*** na raiz do projeto  
- Criar arquivo ***script.js*** na raiz do diretório ***src***
- Integrar de forma externa o arquivo ***script.js*** no arquivo ***index.html***

~~~ html
./index.html

<!DOCTYPE html>

<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JavaScript</title>
</head>
<body>    
    <script src="./src/script.js"></script>
</body>

</html>
~~~

## COMENTÁRIOS

### Comentário de linha

~~~ javascript
./src/script.js

/* comentário de bloco simples */

~~~

### Comentário de bloco com marcadores

~~~ javascript

/**
 * comentário de bloco com marcador
 */

~~~
### Atribuição de valor

~~~ javascript
./src/script.js

var number;

number = 5;

~~~

### Reatribuição de valor

~~~ javascript
./src/script.js

var number = 5;

number = 10;

~~~

### Nomenclaturas

- Caracteres permitidos para iniciar a nomenclatura de um identificador

~~~ javascript
./src/script.js

//letras
var number;
var Number;

// sublinhado
var _number;

//cifrão
var $number;

- Não pode começar um identificador com uma palavra reservada do Java Script

~~~

- Case-sensitive

~~~ javascript
./src/script.js

// "number é diferente de "Number"

~~~

- Nomenclaturas compostas

~~~ javascript
./src/script.js

// camel case
var myName;

// pascal case
var MyName;

// snake case
var my_name;

~~~
## TIPOS DE DADO

### Primitivos

~~~ javascript
./src/script.js

//string
var name = "Alex";
var surname = "Bessa";

//number
var age = 29;
var weight = 85.6;

//flow number
var weight = 85.6;

// boolean
var active = true;
var permission = false;

//underfined
var contains;
console.log(contains);

// null
var data = null;

~~~

### Não Primitivos

~~~ javascript
./src/script.js

// array
var values = [1, "Alex",true, null];

//object Literal
var person = {name: "Alex", age: 29};

var person = {
    name:"Alex",
    age: "29",
};

console.log(person[1])

// function
var message = fuction(){};

~~~

### Inspecionar tipo
~~~ javascript
./src/script.js

// typeof
var age = 29;
console.log(typeof age);

~~~

### Coerção de tipo
- Implícita

~~~ javascript
./src/script.js

// Tudo se torna uma String nesse caso
var age = 29;
var weight = "86.5";
var result = age + weight;
console.log(typeof age);

~~~

- Explícita

~~~ javascript
./src/script.js

// Number()
var weight = Number("85.6");
console.log(typeof weight);

// String()
var age = String(29);
console.log(typeof age);

// Boolean()
var active = Boolean(0);
console.log(typeof active);

~~~

### Operadores
~~~ javascript
./src/script.js

// Aritmético

var num1 = 10;
var num2 = 2;

// Adição
var sum = num1 + num2;

// Subtração
var sub = num1 - num2;

// Multiplicação
var mult = num1 * num2;

// Divisão
var div = num1 / num2;

// Módulo / Resto
var mod = num1 % num2;

// Incremento
num1++

// Decremento
num1--

// Atribuição Simples
var age = 29;

// Atribuição de Adição
var balance = 10;
balance += 5;

balance -= 5;

~~~

