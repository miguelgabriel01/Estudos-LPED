
````markdown
# Operadores, Tipos e Variáveis

---

## 1. Variáveis

### O que são?

Variáveis são espaços na memória do computador que armazenam dados temporariamente para que possam ser usados,
manipulados ou alterados durante a execução do programa.

### Como declarar variáveis em JavaScript?

Desde o ECMAScript 6 (ES6), JavaScript utiliza três palavras-chave para declarar variáveis:

- **var** → Mais antiga, tem escopo de função e permite ser redeclarada. Atualmente, é pouco recomendada.
- **let** → Tem escopo de bloco (ou seja, funciona dentro de chaves {}) e permite que o valor seja alterado.
- **const** → Também tem escopo de bloco, mas o valor não pode ser reatribuído depois que foi declarado.

### Exemplos:

```javascript
var nome = "Ana";
let idade = 30;
const cidade = "São Paulo";
````

### Diferença de escopo:

```javascript
if (true) {
  var x = 10;
  let y = 20;
  const z = 30;
}

console.log(x); // 10
console.log(y); // Erro
console.log(z); // Erro
```

---

## 2. Tipos de Dados

### JavaScript é uma linguagem de tipagem dinâmica

Isso significa que você não precisa especificar o tipo de dado da variável. O JavaScript entende o tipo de acordo com o valor atribuído.

### Tipos primitivos

* **String** → Textos

```javascript
let nome = "Carlos";
```

* **Number** → Números inteiros ou decimais

```javascript
let idade = 25;
let altura = 1.75;
```

* **Boolean** → Verdadeiro ou falso

```javascript
let aprovado = true;
```

* **Undefined** → Variável declarada, mas sem valor atribuído

```javascript
let endereco;
console.log(endereco); // undefined
```

* **Null** → Valor intencionalmente vazio

```javascript
let resposta = null;
```

* **Symbol** → Identificadores únicos (avançado)

* **BigInt** → Números inteiros muito grandes

### Tipo objeto (não primitivo)

* **Object** → Pares chave-valor

```javascript
let pessoa = {
  nome: "Carlos",
  idade: 30
};
```

* **Array** → Lista ordenada de valores

```javascript
let frutas = ["maçã", "banana", "laranja"];
```

* **Function** → Funções também são objetos

```javascript
function saudacao() {
  console.log("Olá!");
}
```

### Verificando tipos

```javascript
let nome = "Carlos";
console.log(typeof nome); // string

let idade = 30;
console.log(typeof idade); // number

let ativo = true;
console.log(typeof ativo); // boolean

let vazio = null;
console.log(typeof vazio); // object (bug histórico)

let indefinido;
console.log(typeof indefinido); // undefined
```

---

## 3. Operadores

### Operadores aritméticos

| Operador | Descrição        | Exemplo      |
| -------- | ---------------- | ------------ |
| +        | Soma             | 10 + 5 = 15  |
| -        | Subtração        | 10 - 5 = 5   |
| \*       | Multiplicação    | 10 \* 5 = 50 |
| /        | Divisão          | 10 / 5 = 2   |
| %        | Resto da divisão | 10 % 3 = 1   |
| \*\*     | Exponenciação    | 2 \*\* 3 = 8 |

### Operadores de atribuição

| Operador | Descrição                  | Exemplo                  |
| -------- | -------------------------- | ------------------------ |
| =        | Atribuição                 | x = 10                   |
| +=       | Soma e atribuição          | x += 5 (x = x + 5)       |
| -=       | Subtração e atribuição     | x -= 5 (x = x - 5)       |
| \*=      | Multiplicação e atribuição | x \*= 5 (x = x \* 5)     |
| /=       | Divisão e atribuição       | x /= 5 (x = x / 5)       |
| %=       | Resto e atribuição         | x %= 5 (x = x % 5)       |
| \*\*=    | Exponenciação e atribuição | x \*\*= 2 (x = x \*\* 2) |

### Operadores de comparação

| Operador | Descrição                             | Exemplo           |
| -------- | ------------------------------------- | ----------------- |
| ==       | Igual (valor)                         | 5 == "5" → true   |
| ===      | Estritamente igual (valor e tipo)     | 5 === "5" → false |
| !=       | Diferente (valor)                     | 5 != "5" → false  |
| !==      | Estritamente diferente (valor e tipo) | 5 !== "5" → true  |
| >        | Maior que                             | 10 > 5 → true     |
| <        | Menor que                             | 5 < 10 → true     |
| >=       | Maior ou igual                        | 10 >= 10 → true   |
| <=       | Menor ou igual                        | 5 <= 5 → true     |

### Operadores lógicos

| Operador | Descrição | Exemplo                |
| -------- | --------- | ---------------------- |
| &&       | E (and)   | true && false → false  |
| \|\|     | OU (or)   | true \|\| false → true |
| !        | NÃO (not) | !true → false          |

### Operadores de incremento e decremento

| Operador | Descrição       | Exemplo    |
| -------- | --------------- | ---------- |
| ++       | Incremento (+1) | x++ ou ++x |
| --       | Decremento (-1) | x-- ou --x |

```javascript
let x = 5;
x++;
console.log(x); // 6

let y = 5;
y--;
console.log(y); // 4
```

### Operador ternário (condicional)

```javascript
let idade = 18;
let status = (idade >= 18) ? "Maior de idade" : "Menor de idade";
console.log(status); // Maior de idade
```

---

## Conclusão

Compreender **variáveis, tipos e operadores** é essencial, pois são a base da lógica de programação em qualquer linguagem, e no JavaScript eles têm características próprias como:

* Tipagem dinâmica (uma variável pode mudar de tipo).
* Escopos diferentes para var, let e const.
* Operadores que permitem construir desde cálculos até estruturas condicionais.

---

# 🚀 Exercícios

## 🟢 Nível 1

### Perímetro de um triângulo equilátero

```javascript
var aresta = 10;
var perimetro = aresta * 3;

console.log("Perimetro do triangulo: " + perimetro);
```

### Perímetro de um quadrado

```javascript
var aresta = 10;
var perimetro = aresta * 4;

console.log("Perimetro do quadrado: " + perimetro);
```

### Perímetro de um retângulo

```javascript
var ladoDoRetanguloA = 10;
var ladoDoRetanguloB = 10;
var ladoDoRetanguloC = 15;
var ladoDoRetanguloD = 15;

var perimetro = ladoDoRetanguloA + ladoDoRetanguloB + ladoDoRetanguloC + ladoDoRetanguloD;

console.log("Perimetro do retangulo: " + perimetro);
```

### Perímetro de um pentágono

```javascript
var ladoDoPentagonoA = 15;
var ladoDoPentagonoB = 15;
var ladoDoPentagonoC = 15;
var ladoDoPentagonoD = 15;
var ladoDoPentagonoE = 15;

var perimetro = ladoDoPentagonoA + ladoDoPentagonoB + ladoDoPentagonoC + ladoDoPentagonoD + ladoDoPentagonoE;

console.log("Perimetro do pentagono: " + perimetro);
```

### Converter segundos em horas

```javascript
// Converter segundos em horas

/**
 1 hora = 60 minutos;
 1 minuto = 60 segundos;

 segundos → minutos → horas
 ou diretamente: segundos ÷ 3600
*/

var segundos = 120000;

var resultadoConversao = segundos / 60 / 60;

console.log("Horas:", resultadoConversao);
```

---

## 🟡 Nível 2

### Média aritmética de seis números

```javascript
var numeroA = 10;
var numeroB = 7;
var numeroC = 8;
var numeroD = 4;
var numeroE = 3;
var numeroF = 6;

var mediaAritimetica = (numeroA + numeroB + numeroC + numeroD + numeroE + numeroF) / 6;

console.log("Media aritimetica: " + mediaAritimetica);
```

### Índice de Massa Corporal (IMC)

```javascript
var peso = 77;
var altura = 1.65;

var resultadoImc = peso/(altura*altura);

console.log("Resultado do IMC: " + resultadoImc);
```

### Volume de um cilindro

```javascript
var areaBase = 10;
var altura = 15;

var resultadoVolumeCilindro = areaBase * altura;

console.log("Volume do cilindro: " + resultadoVolumeCilindro);
```

### Área de um triângulo isósceles

```javascript
var baseTriangulo = 15;
var alturaTriangulo = 33;

var resultadoAreaTriangulo = (baseTriangulo * alturaTriangulo) / 2;

console.log("Área do triângulo isósceles: " + resultadoAreaTriangulo);
```

---

## 🔴 Nível 3

### Escolher o maior entre dois números

```javascript
var numeroA = 15;
var numeroB = 15;

if(numeroA > numeroB){
  console.log("O numero: " + numeroA + " é maior que o numero " + numeroB);
}else if(numeroA < numeroB){
  console.log("O numero: " + numeroB + " é maior que o numero " + numeroA);
}else{
  console.log("Numeros iguais '-'");
}
```

### Trocar valores entre duas variáveis

```javascript
var numeroUm = 10;
var numeroDois = 30;
var numeroC = 0;

numeroC = numeroUm;
numeroUm = numeroDois;
numeroDois = numeroC;

console.log("NumeroUm: " + numeroUm + "/ " + "NumeroDois: " + numeroDois);
```

```

```
