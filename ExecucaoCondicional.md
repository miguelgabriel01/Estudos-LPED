
# Execução Condicional em JavaScript

## O que é Execução Condicional?

A **execução condicional** é um conceito fundamental na lógica de programação que permite que um programa tome decisões durante sua execução. Isso significa que, dependendo de uma condição (verdadeira ou falsa), o programa pode executar um bloco de código ou outro.

Quando desenvolvemos um programa, muitas vezes precisamos que ele **faça algo apenas se determinada situação acontecer**, e que faça outra coisa se não acontecer. Isso é o que chamamos de controle de fluxo com condições.

## Como funciona?

A execução condicional é baseada em **expressões booleanas**, que são aquelas que resultam em dois valores possíveis:

- **`true`** (verdadeiro)
- **`false`** (falso)

Dependendo do resultado da condição, o programa escolhe qual caminho seguir.

## Estruturas Condicionais em JavaScript

### 1. `if`

Executa um bloco de código **se** a condição for verdadeira.

```javascript
if (condicao) {
  // Código executado se a condição for verdadeira
}
```

### 2. `if ... else`

Permite executar um bloco de código **se a condição for verdadeira** e outro bloco **se a condição for falsa**.

```javascript
if (condicao) {
  // Código executado se a condição for verdadeira
} else {
  // Código executado se a condição for falsa
}
```

### 3. `if ... else if ... else`

Permite testar várias condições em sequência.

```javascript
if (condicao1) {
  // Executa se condicao1 for verdadeira
} else if (condicao2) {
  // Executa se condicao2 for verdadeira
} else {
  // Executa se nenhuma das anteriores for verdadeira
}
```

## Operadores utilizados nas condições

### Operadores Relacionais:

| Operador | Significado                           |
| -------- | -------------------------------------- |
| `>`      | Maior que                             |
| `<`      | Menor que                             |
| `>=`     | Maior ou igual                         |
| `<=`     | Menor ou igual                         |
| `==`     | Igual (valor)                         |
| `===`    | Estritamente igual (valor e tipo)     |
| `!=`     | Diferente (valor)                     |
| `!==`    | Estritamente diferente (valor e tipo) |

### Operadores Lógicos:

| Operador | Significado                            |
| -------- | -------------------------------------- |
| `&&`     | E lógico (ambas condições verdadeiras) |
| `||`     | OU lógico (pelo menos uma condição verdadeira) |
| `!`      | NÃO lógico (inverte o valor booleano)  |

## Aplicações na prática

A execução condicional permite resolver problemas do dia a dia, como:

- Verificar se um número é par ou ímpar.
- Conferir se um valor está dentro de determinado intervalo.
- Validar dados inseridos por um usuário.
- Executar cálculos dependendo de regras específicas.

## Exercícios Práticos – Execução Condicional

### 1. Testar se o quadrado de um número é maior do que ele multiplicado por 10

```javascript
var numero = 10;

if(numero * numero > numero * 10){
  console.log("sim, o resultado é maior que o valor do passado x 10");
  console.log("Resultado valor passado elevado ao cubo: " + numero * numero);
}else{
  console.log("Não, o valor passado não é maior que multiplicado por 10");
  console.log("Resultado do valor passado multiplicado por 10: " + numero*10);
}
```

### 2. Testar se um número é divisível por 3 e por 4

```javascript
var numero = 12;

if(numero % 3 === 0 && numero % 4 === 0){
  console.log("Sim, o valor passado é dividivel por 3 e por 4.");
}else{
  console.log("Não, o valor passado não é divisiel por 3 e por 4.");
}
```

### 3. Testar se um número é divisível por 3 mas não por 4

```javascript
var numero = 9;
if (numero % 3 === 0 && numero % 4 !== 0) {
  console.log("Sim, o valor passado é divisível por 3, mas não por 4.");
} else {
  console.log("Não, o valor passado não é divisível por 3 ou é divisível por 4.");
}
```

### 4. Testar se um número é divisível por 2 ou por 7

```javascript
var numero = 14;
if (numero % 2 === 0 || numero % 7 === 0) {
  console.log("Sim, o valor passado é divisível por 2 ou por 7.");
} else {
  console.log("Não, o valor passado não é divisível nem por 2 nem por 7.");
}
```

### 5. Multiplicar dois números e verificar se o resultado é negativo

```javascript
var numeroUm = -10;
var numeroDois = 3;

var resultadoMultiplicacao = numeroUm * numeroDois;

if(resultadoMultiplicacao < 0){
        console.log("O resultado da multiplicação retornou um resultado negativo");
}else{
    console.log("O resultado da multiplicação retornou um valor positivo");
}
```

### 6. Imprimir dois números em ordem crescente

```javascript
var numeroUm = 19;
var numeroDois = 87;

if(numeroUm > numeroDois){
    console.log(numeroUm + "," + numeroDois);
}else{
    console.log(numeroDois + "," + numeroUm);
}
```

### 7. Imprimir dois números em ordem decrescente

```javascript
var numeroUm = 19;
var numeroDois = 87;

if(numeroUm < numeroDois){
    console.log(numeroDois + "," + numeroUm);
}else{
    console.log(numeroUm + "," + numeroDois);
}
```

### 8. Elevar um número ao quadrado e informar se o resultado é maior do que 100

```javascript
var numero = 11;
var resultadoElevadoAoCubo = numero * numero;

if(resultadoElevadoAoCubo > 100){
        console.log("O resultado da elevacao do numero ao cubo retornou um valor maior que 100");
}else{
    console.log("O resultado da elevacao do numero ao cubo retornou um valor menor que 100");
}
```

## Conclusão

Através da execução condicional, conseguimos fazer com que nossos programas sejam mais inteligentes, capazes de tomar decisões e executar diferentes caminhos dependendo da situação. Entender e praticar esse conceito é essencial para qualquer pessoa que deseja se tornar um bom desenvolvedor.
