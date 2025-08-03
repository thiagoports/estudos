# Introdução ao Node.js

## O que é Node.js?

Node.js é um **ambiente de execução JavaScript** do lado do servidor, construído sobre o **motor V8** do Google Chrome. Ele permite que você rode código JavaScript fora do navegador.

- **Linguagem:** JavaScript
- **Plataforma:** Server-side (backend)
- **Desempenho:** Rápido e leve, graças ao motor V8
- **Modelo:** Event-driven, não bloqueante (assíncrono)

---

## Para que serve o Node.js?

- Criar **APIs e servidores web**
- Criar **sistemas em tempo real** (como chats ou jogos multiplayer)
- Automatizar tarefas com **scripts**
- Trabalhar com **microserviços**
- Usado em conjunto com frameworks como **Express**, **NestJS**, entre outros

---

## Comandos básicos para iniciar um projeto

### 1. Iniciando um projeto

# Diferença entre `npm init` e `npm init -y`

## `npm init`

Esse comando **inicia um novo projeto Node.js** interativamente, perguntando passo a passo os dados que devem ser inseridos no `package.json`.

### O terminal vai perguntar:
- nome do projeto
- versão
- descrição
- ponto de entrada (ex: index.js)
- comando de teste
- repositório git
- autor
- licença

📦 Resultado: um `package.json` **personalizado conforme suas respostas**.

---

## `npm init -y` (ou `npm init --yes`)

Esse comando **cria automaticamente o `package.json` com valores padrão**, sem fazer perguntas.

### Exemplo dos valores padrão:
```json
{
  "name": "meu-projeto",
  "version": "1.0.0",
  "main": "index.js",
  "license": "ISC"
}
```
---

### 2. Criando um servidor básico `index.js`

```javascript
const http = require('http');

const server = http.createServer((req, res) => {
  res.write('Olá, mundo!');
  res.end();
});

server.listen(3000, () => {
  console.log('Servidor rodando em http://localhost:3000');
});
```

### Executar o servidor: `node index.js`

## Dicas finais

Para reiniciar o servidor automaticamente, use o pacote nodemon:

`npm install -D nodemon`

Adicione isso no `package.json`:

```json
"scripts": {
  "start": "node index.js",
  "dev": "nodemon index.js"
}
```

## Node.js é a base para muitos frameworks e ferramentas modernas de desenvolvimento web.

