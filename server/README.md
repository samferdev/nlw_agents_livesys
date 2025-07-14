# NLW Agents

Este projeto foi desenvolvido durante o evento **NLW (Next Level Week) da Rocketseat**.

## Descrição

API para gerenciamento de salas (rooms), utilizando Fastify, Drizzle ORM e PostgreSQL.

---

## Principais Tecnologias e Bibliotecas

- **[Fastify](https://fastify.dev/):** Framework web rápido e eficiente para Node.js.
- **[@fastify/cors](https://github.com/fastify/fastify-cors):** Middleware para CORS.
- **[Zod](https://zod.dev/):** Validação de esquemas e tipos.
- **[fastify-type-provider-zod](https://github.com/fastify/type-provider-zod):** Integração de Zod com Fastify.
- **[Drizzle ORM](https://orm.drizzle.team/):** ORM moderno para TypeScript.
- **[drizzle-seed](https://github.com/drizzle-team/drizzle-seed):** Seed para popular o banco de dados.
- **[PostgreSQL](https://www.postgresql.org/):** Banco de dados relacional.
- **[Docker](https://www.docker.com/):** Facilita o setup do banco de dados.
- **[TypeScript](https://www.typescriptlang.org/):** Tipagem estática para JavaScript.

---

## Padrões de Projeto

- **Validação de dados:** Utiliza Zod para validação e tipagem.
- **Separação de responsabilidades:** Rotas, validações e lógica de banco de dados organizadas em arquivos distintos.
- **Migrations e Seeds:** Gerenciados via Drizzle ORM e drizzle-seed.

---

## Setup e Configuração

### 1. Clone o repositório

```bash
git clone <url-do-repo>
cd server
```

### 2. Instale as dependências

```bash
npm install
```

### 3. Configure as variáveis de ambiente

Crie um arquivo `.env` na raiz do projeto com:

```
PORT=3333
DATABASE_URL=postgres://docker:docker@localhost:5432/agents
```

### 4. Suba o banco de dados com Docker

```bash
docker-compose up -d
```

### 5. Rode as migrations e o seed

```bash
npm run db:seed
```

### 6. Inicie o servidor

```bash
npm run dev
```

---

## Exemplos de Requisições

- **Health check:** `GET /health`
- **Listar salas:** `GET /rooms`

---

## Observações

- O projeto utiliza Drizzle ORM para migrations e seeds.
- O banco de dados padrão é PostgreSQL, configurado via Docker.
- O endpoint principal está disponível em `http://localhost:3333`. 