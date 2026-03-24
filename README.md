# 🛒 API RESTful de E-commerce

Este projeto é uma API backend desenvolvida com **Node.js** e **Express**, com o objetivo de gerenciar usuários, produtos e categorias em um sistema de e-commerce.

A aplicação conta com autenticação via **JWT**, documentação interativa com **Swagger** e testes automatizados utilizando **Jest** e **Supertest**.

---

## 🚀 Status do Projeto

🟢 Em desenvolvimento

---

## 🧰 Tecnologias Utilizadas

- Node.js
- Express
- Sequelize (ORM)
- PostgreSQL
- JWT (Autenticação)
- Swagger (Documentação da API)
- Jest + Supertest (Testes automatizados)

---

## 📦 Funcionalidades

- 👤 Cadastro e autenticação de usuários
- 🛒 CRUD de produtos
- 🗂️ CRUD de categorias
- 🔐 Proteção de rotas com JWT
- 📄 Documentação interativa com Swagger
- 🧪 Testes automatizados

---

## ⚙️ Pré-requisitos

Antes de começar, você precisa ter instalado:

- Node.js (versão 16 ou superior)
- NPM ou Yarn
- PostgreSQL
- Git

---

## 🔧 Instalação

Clone o repositório:

```bash
git clone https://github.com/isabelefreitas23/Projeto-backend.git

Acesse a pasta do projeto:

cd Projeto-backend

Instale as dependências:

npm install
🔐 Configuração

Crie um arquivo .env na raiz do projeto e configure as variáveis de ambiente:

PORT=3001

DB_HOST=localhost
DB_USER=seu_usuario
DB_PASSWORD=sua_senha
DB_NAME=nome_do_banco
DB_PORT=5432

JWT_SECRET=sua_chave_secreta
▶️ Como rodar o projeto

Para iniciar o servidor em ambiente de desenvolvimento:

npm run dev

A API estará disponível em:

http://localhost:3001
📄 Documentação da API (Swagger)

Após iniciar o projeto, acesse:

http://localhost:3001/api-docs

Você poderá visualizar e testar todos os endpoints diretamente pelo navegador.

📁 Estrutura do Projeto
src/
├── config/         # Configurações (banco, etc)
├── controllers/    # Lógica das requisições
├── models/         # Modelos do banco de dados
├── routes/         # Definição das rotas
├── middlewares/    # Middlewares (auth, validações)
├── services/       # Regras de negócio
├── database/       # Conexão com banco
└── app.js          # Inicialização da aplicação

🔗 Endpoints da API

🔐 Autenticação
POST /auth/register → Cadastro de usuário
POST /auth/login → Login e geração de token

🛒 Produtos
GET /products → Listar produtos
POST /products → Criar produto
PUT /products/:id → Atualizar produto
DELETE /products/:id → Remover produto

🗂️ Categorias
GET /categories
POST /categories
PUT /categories/:id
DELETE /categories/:id

🧪 Testes

Para rodar os testes automatizados:

npm test

Os testes foram desenvolvidos utilizando:

Jest
Supertest

🤝 Contribuindo

Contribuições são sempre bem-vindas!

Faça um fork do projeto
Crie uma branch para sua feature
git checkout -b minha-feature
Commit suas alterações
git commit -m 'Minha nova feature'
Envie para o repositório
git push origin minha-feature
Abra um Pull Request 🚀

📄 Licença

Este projeto está sob a licença MIT.