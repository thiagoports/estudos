# Tipos de Dados em JavaScript

JavaScript possui **tipos de dados dinâmicos**, ou seja, o tipo de uma variável é determinado automaticamente durante a execução do código. Os tipos se dividem em dois grupos:

- **Primitivos**: simples e imutáveis.
- **Objetos**: estruturas complexas que podem armazenar múltiplos valores e comportamentos.

## 1. Number

O tipo `Number` representa **tanto inteiros quanto números de ponto flutuante**.

```javascript
let idade = 25;
let altura = 1.75;
```

## Números Especiais (Special Numbers):

Infinity – resultado de uma operação como 1 / 0.
-Infinity – negativo de Infinity.
NaN (Not a Number) – resultado de uma operação inválida com números, como 0 / "texto".

```javascript
console.log(1 / 0);       // Infinity
console.log(-1 / 0);      // -Infinity
console.log("abc" * 3);   // NaN
```

## 2. String 

Strings representam sequências de caracteres. Podem ser definidas usando aspas simples, duplas ou crase (para template literals).
(Padrão da maioria das linguagens)

```javascript
let nome = "Ana";
let sobrenome = 'Silva';
let saudacao = `Olá, ${nome} ${sobrenome}!`; // Template literal
```

## 3. Boolean

O tipo Boolean representa valores lógicos: verdadeiro (true) ou falso (false).

```javascript
let maiorDeIdade = true;
let temCarteira = false;
```

Muito usado em estruturas de decisão e comparações:
let resultado = 10 > 5; // true

## 4. Empty Values

# null
Representa ausência proposital de valor. Deve ser atribuído pelo programador.
```javascript
let usuario = null; // sem valor definido ainda
```
# undefined
Representa uma variável declarada mas não inicializada, ou seja, sem valor atribuído.
```javascript
let idade;
console.log(idade); // undefined
```

⚠️ null e undefined são diferentes: null é um valor definido intencionalmente, undefined é o padrão para variáveis não atribuídas.

## 5. Object

Objetos são estruturas que armazenam pares de chave-valor e são o tipo mais usado para representar dados complexos.

```javascript
let pessoa = {
  nome: "João",
  idade: 30,
  ativo: true
};
```

Também é possível criar objetos de outros tipos como:

# Arrays: listas ordenadas
```javascript
let frutas = ["maçã", "banana", "laranja"];
```
# Funções: também são objetos em JS
```javascript
function saudacao() {
  console.log("Olá!");
}
```
