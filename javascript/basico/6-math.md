# Objeto Math em JavaScript

## 🔹 O que é o objeto Math?

O `Math` é um **objeto embutido** em JavaScript que fornece funções e constantes matemáticas. Ele **não é um construtor**, ou seja, não é usado com `new`.

---

## 🔹 Como usar?

Você acessa os métodos do `Math` diretamente:

```javascript
let x = Math.sqrt(16); // x = 4
```

# Principais métodos do Math

## `Math.abs(x)`

Retorna o valor absoluto (positivo) de `x`.
```javascript
Math.abs(-7); // 7
```

## `Math.ceil(x)`

Arredonda `x` pra cima (próximo inteiro maior)
```javascript
Math.ceil(4.2); // 5
```

## `Math.floor(x)`

Arredonda `x` pra baixo (próximo inteiro menor)
```javascript
Math.floor(4.9); // 4
```

## `Math.round(x)`

Arredonda `x` para o inteiro mais próximo
```javascript
Math.round(4.5); // 5
Math.round(4.4); // 4
```

## `Math.max(a, b, ...)`

Retorna o maior valor entre os argumentos
```javascript
Math.max(10, 20, 30); // 30
```

## `Math.min(a, b, ...)`

Retorna o menor valor entre os argumentos
```javascript
Math.min(10, 20, 30); // 10
```

## `Math.random()`

Retorna um valor aleatório entre 0 (inclusivo) e 1 (exclusivo)
```javascript
let aleatorio = Math.random(); // ex: 0.473829
```

Também dá pra fazer entre dois valores (escolha do usuário)
```javascript
// Aleatório entre 1 e 10
let numero = Math.floor(Math.random() * 10) + 1;
```

## `Math.sqrt(x)`

Retorna a raiz quadrada de `x`
```javascript
Math.sqrt(25); // 5
```

## `Math.pow(base, expoente)`

Retorna a potência da base elevada ao expoente
```javascript
Math.pow(2, 3); // 8
```

## `Math.PI`

Retorna o valor de π (pi)
```javascript
let pi = Math.PI; // 3.141592653589793
```

## `Outras constantes úteis`

```javascript
Math.E        // base do logaritmo natural (~2.718)
Math.LN2      // logaritmo natural de 2 (~0.693)
Math.LN10     // logaritmo natural de 10 (~2.302)
Math.LOG2E    // log de E na base 2 (~1.442)
Math.LOG10E   // log de E na base 10 (~0.434)
Math.SQRT1_2  // raiz quadrada de 1/2 (~0.707)
Math.SQRT2    // raiz quadrada de 2 (~1.414)
```

# 📌 Resumo dos métodos

| Método           | Descrição                             |
| ---------------- | ------------------------------------- |
| `Math.abs(x)`    | Valor absoluto                        |
| `Math.ceil(x)`   | Arredonda para cima                   |
| `Math.floor(x)`  | Arredonda para baixo                  |
| `Math.round(x)`  | Arredonda para o inteiro mais próximo |
| `Math.max(a, b)` | Maior valor                           |
| `Math.min(a, b)` | Menor valor                           |
| `Math.random()`  | Número aleatório entre 0 e 1          |
| `Math.sqrt(x)`   | Raiz quadrada                         |
| `Math.pow(x, y)` | Potência                              |
| `Math.PI`        | Constante π                           |
