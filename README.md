

## Funcionalidades

Nesse modulo foi desenvolvida uma API REST com node.js para controle financeiro.

* `GET - /transactions`

  Listar todas as transactions salvas no banco de dados.

* `GET - /transactions/:id`
  
  Pesquisar pelo id um transaction.

* `GET - /transactions/summary`

  Mostrar a soma de entradas e saídas.

* `POST - /transactions`

  Criar uma nova transaction no banco de dados, enviando os campos `title`, `amount` e `type` por meio do `body` da requisição.

## :hammer_and_wrench: Tecnologias

* **Node.Js**
* **Typescript**
* **Zod**
* **Fastify**
  * @fastify/cookie
* **Eslint**
* **Vitest**
* **Supertest**
* **Tsup**
* **Tsx**
* **Sqlit 3** para ambiente de desenvolvimento.
* **PostgreSQL** para ambiente de produção.

## 👷 Requisitos

```bash
# Clone repository

$ git clone https://github.com/laroyprado/ApiRESTful-Rocketseat-Ignite

# Go to server folder

$ cd ApiRESTful-Rocketseat-Ignite

# Install Dependencies

$ npm i

# Rename file .env.example to .env

# Rename file .env.test.example to .env.test

# Run script Knex

$ npm run knex -- migrate:latest

# Run aplication

$ npm run dev

# Access localhost
# http://localhost:3333
```

# RF

- [x] O usuário deve poder criar uma nova transação;
- [x] O usuário deve poder obter um resumo da sua conta;
- [x] O usuário deve poder listar todas transações que já ocorreram;
- [x] O usuário deve poder visualizar uma transação única;

# RN

- [x] A transação pode ser do tipo crédito que somará ao valor total, ou débito subtrairá;
- [x] Deve ser possível identificarmos o usuário entre as requisições;
- [x] O usuário só pode visualizar transações o qual ele criou;
