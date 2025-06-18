````markdown
# Operadores Lógicos em JavaScript

## 📖 O que são Operadores Lógicos?

Operadores lógicos são ferramentas fundamentais em qualquer linguagem de programação. Eles permitem criar **expressões lógicas**,
que resultam em **verdadeiro (`true`) ou falso (`false`)**,com base na combinação de duas ou mais condições.

Eles são essenciais para que o programa tome decisões mais complexas.

---

## 🚦 Quais são os operadores lógicos?

| Operador | Nome         | Descrição                                             |
|----------|--------------|-------------------------------------------------------|
| `&&`     | E lógico     | **Todas as condições precisam ser verdadeiras.**     |
| `||`     | OU lógico    | **Pelo menos uma condição precisa ser verdadeira.**  |
| `!`      | NÃO lógico   | **Inverte o valor lógico.** Se for `true`, vira `false` e vice-versa.|

---

## 🔧 Como funciona cada um?

### `&&` (E lógico)

Só retorna `true` se **TODAS as condições forem verdadeiras**.

```javascript
if (idade >= 18 && possuiCNH) {
    console.log("Pode dirigir");
} else {
    console.log("Não pode dirigir");
}
````

---

### `||` (OU lógico)

Retorna `true` se **pelo menos uma** das condições for verdadeira.

```javascript
if (dia === "sábado" || dia === "domingo") {
    console.log("É final de semana!");
} else {
    console.log("É dia útil.");
}
```

---

### `!` (NÃO lógico)

Inverte o valor lógico da condição.

```javascript
let temCartao = false;

if (!temCartao) {
    console.log("Você precisa de um cartão para continuar.");
}
```

---

## 💻 Exercícios Práticos – Operadores Lógicos

---

### 🏆 1. Encontrar o maior número entre três números

```javascript
var primeiroNumero = 10;
var segundoNumero = 33;
var terceiroNumero = 14;

if(primeiroNumero > segundoNumero && primeiroNumero > terceiroNumero){
    console.log("O maior numero fornecido é o: " + primeiroNumero);
}else if(segundoNumero > primeiroNumero && segundoNumero > terceiroNumero){
    console.log("O maior numero fornecido é o: " + segundoNumero);
}else if(terceiroNumero > primeiroNumero && terceiroNumero > segundoNumero){
    console.log("O maior numero fornecido é o: " + terceiroNumero);
}else{
    console.log("Numeros iguais*");
}
```

---

### 🔐 2. Validação simples de login (email e senha)

```javascript
let email = "biel@gmail.com";
let password = "teste123";

if(email === "biel@gmail.com" && password === "teste123"){
    console.log("Usuario logado com sucesso!");
}else{
    console.log("Credenciais invalidas");
}
```

---

### ✈️ 3. Verificar se uma pessoa pode fazer uma viagem

A pessoa precisa ter mais de 18 anos **ou** estar acompanhada dos pais.

```javascript
let idade = 16;
let acompanhadoDosPais = true;

if(idade >= 18 || acompanhadoDosPais){
    console.log("Pode viajar.");
}else{
    console.log("Não pode viajar.");
}
```

---

### 🔢 4. Verificar se um número está dentro de um intervalo

Verificar se o número está entre 10 e 20.

```javascript
let numero = 15;

if(numero >= 10 && numero <= 20){
    console.log("O número está entre 10 e 20.");
}else{
    console.log("O número NÃO está entre 10 e 20.");
}
```

---

### 🔑 5. Sistema simples de verificação de acesso

O usuário só pode acessar se tiver cadastro **e** se não estiver bloqueado.

```javascript
let possuiCadastro = true;
let estaBloqueado = false;

if(possuiCadastro && !estaBloqueado){
    console.log("Acesso liberado.");
}else{
    console.log("Acesso negado.");
}
```

---

## 🚀 Conclusão

Operadores lógicos são fundamentais para criar **decisões mais inteligentes nos programas**, permitindo combinar condições e controlar o fluxo da aplicação.

Eles estão presentes em praticamente todo código que envolve verificações, validações, regras de negócio e tomadas de decisão.

---
```
