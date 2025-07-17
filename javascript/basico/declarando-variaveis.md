# Declaração de Variáveis em JavaScript

Em JavaScript, usamos variáveis para armazenar dados. Existem três principais formas de declarar variáveis:

- `let`
- `const`
- `var` (forma antiga, geralmente evitada hoje)

---

## `let`

Usado para declarar **variáveis que podem ser reatribuídas**.

```javascript
let nome = "João";
nome = "Carlos"; // válido
console.log(nome); // Carlos
```

# Características do `let`:

Pode ter seu valor alterado.

Tem escopo de bloco (só existe dentro do bloco onde foi declarada).

Não pode ser redeclarada no mesmo escopo.
```javascript
let idade = 20;
{
  let idade = 30;
  console.log(idade); // 30 (escopo interno)
}
console.log(idade); // 20 (escopo externo)
```

## `const`

Usado para declarar constantes, ou seja, valores que não podem ser reatribuídos.
```javascript
const PI = 3.14159;
PI = 3.14; // ERRO: não pode alterar valor de uma const
```

# Características do `const`:

Não pode ser reatribuída.

Também tem escopo de bloco.

É comum usar `const` para valores fixos e funções que não mudarão.
```javascript
const usuario = {
  nome: "Maria",
  idade: 22
};

usuario.nome = "Ana"; // Isso é permitido (o objeto pode ser alterado)
```
⚠️ Importante: `const` impede a reatribuição da variável, mas não torna o conteúdo interno imutável (em objetos e arrays).

## `var` forma antiga

`var` é a forma mais antiga de declarar variáveis e hoje é desaconselhada no código moderno.

# Problemas do `var`:

Escopo de função, não de bloco.

Pode ser redeclarada no mesmo escopo, o que pode causar bugs.
```javascript
var linguagem = "JavaScript";
var linguagem = "Python"; // permitido com var (mas confuso!)
console.log(linguagem); // Python
```

## Quando usar cada um?
| Palavra-chave | Pode alterar valor? | Escopo    | Uso recomendado                   |
| ------------- | ------------------- | --------- | --------------------------------- |
| `let`         | Sim                 | De bloco  | Variáveis que mudam de valor      |
| `const`       | Não (referência)    | De bloco  | Constantes e preferido por padrão |
| `var`         | Sim                 | De função | **Evitar no código moderno**      |

# Dica de boas práticas

Use const por padrão, e só use let quando você realmente precisar alterar o valor.

Evite var, pois pode causar comportamentos inesperados.
```javascript
const nome = "Lucas";
let idade = 30;
```

