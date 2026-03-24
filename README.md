# API RESTful de E-commerce

## Descrição

Este projeto consiste em uma aplicação backend desenvolvida com o objetivo de fornecer uma API robusta, escalável e segura para gerenciamento de recursos. A solução foi estruturada seguindo boas práticas de arquitetura, organização de código e padronização de endpoints, permitindo fácil manutenção e evolução.

---

## Requisitos

Antes de iniciar, certifique-se de possuir os seguintes requisitos instalados no ambiente:

- Node.js (versão 16 ou superior)
- Gerenciador de pacotes (NPM ou Yarn)
- Banco de dados PostgreSQL (ou outro compatível, conforme configuração)
- Git

---

## Instalação

Clone o repositório:

```bash
git clone https://github.com/seu-usuario/seu-projeto.git

Acesse o diretório do projeto:

cd seu-projeto

Instale as dependências:

npm install
Configuração

Crie um arquivo .env na raiz do projeto e configure as variáveis de ambiente conforme necessário:

PORT=3000
DB_HOST=localhost
DB_PORT=5432
DB_USER=usuario
DB_PASSWORD=senha
DB_NAME=banco_de_dados
JWT_SECRET=chave_secreta

Certifique-se de que o banco de dados esteja criado e acessível com as credenciais informadas.

Execução

Para iniciar o projeto em ambiente de desenvolvimento:

npm run dev

Para execução em produção:

npm start

A aplicação estará disponível em:

http://localhost:3000
Estrutura do Projeto
src/
├── config/         # Configurações gerais
├── controllers/    # Controladores das rotas
├── models/         # Modelos de dados
├── routes/         # Definição das rotas
├── middlewares/    # Middlewares da aplicação
├── services/       # Regras de negócio
├── database/       # Conexão com banco de dados
└── app.js          # Inicialização da aplicação

Uso da API

Autenticação

POST /auth/login

Exemplo de requisição:

{
  "email": "usuario@email.com",
  "password": "123456"
}

Resposta esperada:

{
  "token": "jwt_token_aqui"
}
Produtos
GET /products

Retorna a lista de produtos cadastrados.

POST /products

Exemplo de requisição:

{
  "name": "Produto Exemplo",
  "price": 100.0,
  "categoryId": 1
}
Testes

Para executar os testes automatizados:

npm test

Os testes são realizados utilizando frameworks apropriados para validação de endpoints e regras de negócio.

Contribuição

Para contribuir com o projeto:

Realize um fork do repositório
Crie uma branch para sua modificação:

git checkout -b minha-alteracao

Realize o commit das alterações:

git commit -m "Descrição da alteração"

Envie para o repositório remoto:

git push origin minha-alteracao

Abra um Pull Request