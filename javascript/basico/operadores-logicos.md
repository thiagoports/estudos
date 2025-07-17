# Operadores Lógicos em JavaScript

Os **operadores lógicos** são usados para combinar expressões booleanas (true/false) e controlar o fluxo de decisões em um programa.

## 1. `&&` – AND (E lógico)

Retorna `true` **somente se ambas as expressões forem verdadeiras**. Se **qualquer uma for falsa**, o resultado será `false`.

```javascript
true && true    // true
true && false   // false
false && false  // false

let idade = 25;
let temCarteira = true;

if (idade >= 18 && temCarteira) {
  console.log("Pode dirigir");
}
```

## 2. || – OR (OU lógico)

Retorna `true` se pelo menos uma das expressões for verdadeira. Só retorna `false` se ambas forem falsas.
```javascript
true || false   // true
false || false  // false
true || true    // true

let possuiRG = false;
let possuiCNH = true;

if (possuiRG || possuiCNH) {
  console.log("Documento aceito");
}
```

## 3. ! – NOT (NÃO lógico)

Inverte o valor da expressão:

Se for `true`, vira `false`.

Se for `false`, vira `true`.

```javascript
!true     // false
!false    // true

let estaLogado = false;

if (!estaLogado) {
  console.log("Usuário não está logado");
}
```
## Tabela Verdade (Resumida)

`&&` (AND)

| A     | B     | A && B |
| ----- | ----- | ------ |
| true  | true  | true   |
| true  | false | false  |
| false | true  | false  |
| false | false | false  |

`||` (OR)

| A     | B     | A \|\| B |
| ----- | ----- | -------- |
| true  | true  | true     |
| true  | false | true     |
| false | true  | true     |
| false | false | false    |


`!` (NOT)

| A     | !A    |
| ----- | ----- |
| true  | false |
| false | true  |

## Conclusão
Os operadores lógicos são fundamentais para controlar decisões no JavaScript. 
Eles permitem combinar condições e definir regras mais complexas de forma clara e poderosa.
