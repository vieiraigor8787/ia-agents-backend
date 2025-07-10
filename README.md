# agents aiG 🤖

Backend do projeto **agents aiG** utilizando Node.js, Fastify, Drizzle ORM e PostgreSQL.

## 🚀 Tecnologias & Bibliotecas

- **Node.js**: Ambiente de execução JavaScript.
- **Fastify**: Framework web para APIs rápidas e eficientes.
- **drizzle-orm**: ORM para integração com banco de dados PostgreSQL.
- **drizzle-seed**: Seed de dados para ambiente de desenvolvimento.
- **zod**: Validação de esquemas e tipos.
- **@fastify/cors**: Middleware para CORS.
- **postgres**: Cliente PostgreSQL para Node.js.
- **biome**: Linter e formatter para código.
- **Docker**: Containerização do banco de dados PostgreSQL.

## 🧩 Padrões de Projeto

- **Modularização**: Separação de rotas, conexão e schema do banco.
- **Type-safe**: Uso de Zod e TypeScript para garantir tipos seguros.
- **Migrations**: Gerenciadas via Drizzle ORM.
- **.env**: Configuração de variáveis de ambiente.

## ⚙️ Setup & Configuração

1. **Clone o repositório e instale as dependências:**

   ```sh
   npm install
   ```

2. **Configure o arquivo `.env`:**
   Copie `.env.example` para `.env` e preencha as variáveis necessárias.

3. **Suba o banco de dados PostgreSQL com Docker:**

   ```sh
   docker-compose up -d
   ```

4. **Execute o Drizzle Kit para preparar o banco de dados:**

   ```sh
   npx drizzle-kit migrate
   ```

5. _(Opcional)_ **Popule o banco com dados de seed:**

   ```sh
   npm run db:seed
   ```

6. **Inicie o servidor em modo desenvolvimento:**
   ```sh
   npm run dev
   ```
