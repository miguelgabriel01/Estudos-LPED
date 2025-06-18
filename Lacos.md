
````markdown
# 🔁 Laços de Repetição em JavaScript

## 📖 O que são laços de repetição?

Laços de repetição (ou estruturas de repetição) são comandos que permitem executar **um bloco de código várias vezes**,
de acordo com uma condição ou com a quantidade de itens em uma lista.

Eles evitam que o programador precise repetir manualmente o mesmo código várias vezes.

---

## 🔢 Tipos de laços em JavaScript:

---

## 1️⃣ **`for`** – Laço Contado

### ✔️ Usado quando sabemos **quantas vezes queremos repetir**.

### 📑 Sintaxe:

```javascript
for(inicialização; condição; incremento){
    // Bloco de código a ser executado
}
````

### 🛠️ Exemplo:

```javascript
for(let i = 1; i <= 5; i++){
    console.log("Repetição número: " + i);
}
```

---

## 2️⃣ **`forEach()`** – Laço para Arrays

### ✔️ Usado para percorrer **cada item de um array** de forma bem simples.

### 📑 Sintaxe:

```javascript
array.forEach(function(item){
    // Bloco de código que usa o item
});
```

### 🛠️ Exemplo:

```javascript
let frutas = ["Maçã", "Banana", "Laranja"];

frutas.forEach(function(fruta){
    console.log("Eu gosto de " + fruta);
});
```

> 🔸 **Observação:** O `forEach` **só funciona em arrays**.

---

## 3️⃣ **`while`** – Laço com condição no início

### ✔️ Executa o bloco **enquanto a condição for verdadeira**.

### 📑 Sintaxe:

```javascript
while(condicao){
    // Bloco de código
}
```

### 🛠️ Exemplo:

```javascript
let contador = 1;

while(contador <= 5){
    console.log("Contador vale: " + contador);
    contador++;
}
```

> 🔸 **Se a condição começar falsa, o bloco não será executado nenhuma vez.**

---

## 4️⃣ **`do...while`** – Laço com condição no final

### ✔️ Executa o bloco **pelo menos uma vez**, e depois repete **enquanto a condição for verdadeira**.

### 📑 Sintaxe:

```javascript
do {
    // Bloco de código
} while(condicao);
```

### 🛠️ Exemplo:

```javascript
let contador = 1;

do {
    console.log("Contador vale: " + contador);
    contador++;
} while(contador <= 5);
```

> 🔸 **O bloco será executado ao menos uma vez, mesmo que a condição seja falsa.**

---

## 🚦 Comparativo rápido dos laços:

| Laço         | Quando usar                                               |
| ------------ | --------------------------------------------------------- |
| `for`        | Quando sabe o número de repetições                        |
| `forEach()`  | Para percorrer todos os itens de um array                 |
| `while`      | Quando não sabe exatamente quantas vezes irá repetir      |
| `do...while` | Quando precisa executar ao menos uma vez, e depois testar |

---

````markdown
# 🔢 Exercícios de Laços com `for` em JavaScript

---

## 📌 Imprimir os números negativos de 1 em 1, de -1 até -20

```javascript
for(var i = -1; i >= -20; i--){
    console.log(i);
}
````

---

## 📌 Imprimir os números de 3 em 3, de 0 até 30

```javascript
for(var i = 0; i <= 30; i += 3){
    console.log(i);
}
```

---

## 📌 Imprimir os números de 3 em 3, de 0 até -30

```javascript
for(var i = 0; i >= -30; i += -3){
    console.log(i);
}
```

---

## 📌 Imprimir os 10 primeiros números ímpares

```javascript
for(var i = 0; i <= 20; i++){
    if(i % 2 != 0){
        console.log(i);
    }
}
```

---

## 📌 Imprimir os 20 primeiros números divisíveis por 3

```javascript
for(var i = 0; i <= 30; i++){
    if(i % 3 == 0){
        console.log(i);
    }
}
```

---

## 📌 Imprimir os quadrados dos 10 primeiros números inteiros

```javascript
for(var i = 0; i <= 10; i++){
    var imprimirNumerosAoQuadrado = i ** 2;
    console.log(imprimirNumerosAoQuadrado);
}
```

---

## 📌 Imprimir os números entre 0 e 25 em ordem decrescente

```javascript
for(var i = 25; i >= 0; i--){
    console.log(i);
}
```

---

```


## 🚀 Conclusão

Os laços de repetição são ferramentas poderosas que permitem tornar nossos programas mais eficientes,
evitando códigos repetitivos.

Saber escolher qual laço usar depende do problema que você está resolvendo:

* Precisa repetir um número fixo de vezes? 👉 Use `for`.
* Está lidando com uma lista (array)? 👉 Use `forEach`.
* Precisa repetir até que uma condição se torne falsa? 👉 Use `while`.
* Quer garantir que o bloco rode pelo menos uma vez? 👉 Use `do...while`.

---

```
