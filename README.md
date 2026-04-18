# user-flow-api-mongo

Uma API REST simples e eficiente para gerenciamento de usuários, construída com **Node.js**, **Express** e **MongoDB**.

## 🚀 Funcionalidades

- ✅ **Criar** novos usuários
- ✅ **Listar** todos os usuários
- ✅ **Buscar** usuário específico por ID
- ✅ **Atualizar** dados do usuário
- ✅ **Deletar** usuário

## 🛠️ Stack Tecnológico

- **Node.js** - Runtime JavaScript
- **Express** - Framework web minimalista
- **MongoDB** - Banco de dados NoSQL
- **Mongoose** - ODM (Object Data Modeling)
- **Nodemon** - Auto-reload durante desenvolvimento
- **Dotenv** - Gerenciamento de variáveis de ambiente

## 📦 Instalação

### Pré-requisitos

- [Node.js](https://nodejs.org/) instalado
- [MongoDB Community Server](https://www.mongodb.com/try/download) instalado e rodando localmente

### Passos

1. Clone o repositório:
```bash
git clone https://github.com/seu-usuario/user-flow-api-mondo.git
cd user-flow-api-mondo/backend
```

2. Instale as dependências:
```bash
npm install
```

3. Execute a aplicação:

**Modo desenvolvimento:**
```bash
npm run dev
```

**Modo produção:**
```bash
npm start
```

A API estará disponível em `http://localhost:3003`

## 📚 Endpoints da API

### GET `/`
Teste a API
```json
{
  "nome": "lucas"
}
```

### POST `/user`
Criar novo usuário
```json
{
  "nome": "João Silva",
  "idade": 25
}
```

### GET `/user`
Listar todos os usuários

### GET `/user/:id`
Buscar usuário por ID

### PUT `/user/:id`
Atualizar usuário
```json
{
  "nome": "João Santos",
  "idade": 26
}
```

### DELETE `/user/:id`
Deletar usuário

## 🗂️ Estrutura do Projeto

```
.
├── backend/
│   ├── src/
│   │   ├── index.js           # Arquivo principal da API
│   │   └── models/
│   │       └── user.js        # Schema do usuário
│   ├── package.json
│   └── .env
└── README.md
```

## ⚙️ Variáveis de Ambiente

Crie um arquivo `.env` na pasta `backend/`:
```
MONGO_URI=mongodb://localhost/mongocrud
PORT=3003
```

## 🤝 Contribuindo

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e pull requests.

## 📄 Licença

Este projeto está sob a licença ISC.

