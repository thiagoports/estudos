### Funções em JavaScript

## O que são funções?

Funções são **blocos de código reutilizáveis** que executam uma tarefa específica. 
Elas ajudam a **organizar, reutilizar e modularizar** o código.

---

### Como declarar uma função

## Forma tradicional (declaração de função)

```javascript
function saudacao() {
  console.log("Olá, mundo!");
}
```

## Função com parâmetros

```javascript
function soma(a, b) {
  return a + b;
}
```

## Expressão de função

```javascript
const multiplicar = function(a, b) {
  return a * b;
};
```

## Arrow function (função de seta)

```javascript
const dividir = (a, b) => {
  return a / b;
};
```

## Como usar (chamar) uma função

```javascript
saudacao(); // Chama a função saudacao

let resultado = soma(5, 3); // resultado = 8
```

## Parâmetros e argumentos

Parâmetros: são os nomes usados na declaração da função.
Argumentos: são os valores passados para a função na hora da execução.

```javascript
function saudacao(nome) {
  console.log("Olá, " + nome);
}

saudacao("Tiago"); // Argumento = "Tiago"
```

## Return
O `return` é usado para retornar um valor de dentro da função.

```javascript
function dobro(x) {
  return x * 2;
}

let resultado = dobro(4); // resultado = 8
```

⚠️ Após `return`, nada mais é executado dentro da função.

## Funções aninhadas

Funções podem ser declaradas dentro de outras funções:

```javascript
function externa() {
  function interna() {
    console.log("Função interna");
  }

  interna();
}
```

### Por que usar funções?

Evita repetição de código

Deixa o código mais limpo e organizado

Facilita testes e manutenção

Modulariza comportamentos

### EXTRA: `alert()` e `prompt()`
`alert()`
Exibe uma mensagem na tela em forma de caixa de alerta.

```javascript
alert("Bem-vindo!");
```
🔔 Ideal para avisos rápidos, mas não é personalizável.

`prompt()`
Exibe uma caixa de entrada para o usuário digitar um valor.

```javascript
let nome = prompt("Qual seu nome?");
alert("Olá, " + nome);
```
📌 Pouco usado, o design é simples e não personalizável, mas útil em testes e scripts rápidos.

### Resumo

| Tipo               | Exemplo básico               | Uso principal                   |
| ------------------ | ---------------------------- | ------------------------------- |
| Função tradicional | `function nome() {}`         | Estrutura comum                 |
| Expressão          | `const nome = function() {}` | Guardar função numa variável    |
| Arrow function     | `const nome = () => {}`      | Sintaxe mais curta e moderna    |
| `alert()`          | `alert("Oi")`                | Mostrar alerta simples          |
| `prompt()`         | `prompt("Digite algo")`      | Obter entrada rápida do usuário |
