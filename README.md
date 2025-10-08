# 🧑‍💻 Sistema de Cadastro de Usuários

Aplicação **Full Stack** desenvolvida com **Node.js**, **Express**, **Prisma (MongoDB)** e **React (Vite)**.  
Permite **cadastrar, listar, editar e excluir usuários**, integrando um **backend RESTful** com um **frontend moderno e responsivo**.

---

## 🚀 Tecnologias Utilizadas

### **Backend (API)**
- [Node.js](https://nodejs.org/)
- [Express](https://expressjs.com/)
- [Prisma ORM](https://www.prisma.io/)
- [MongoDB](https://www.mongodb.com/)
- [Cors](https://www.npmjs.com/package/cors)

### **Frontend (Interface)**
- [React](https://react.dev/)
- [Vite](https://vitejs.dev/)
- [Axios](https://axios-http.com/)

---

## 📁 Estrutura do Projeto

```
📦 projeto-cadastro-usuarios 
 ┣ 📂 api
 ┃ ┣ 📂 prisma
 ┃ ┃ ┗ 📜 schema.prisma
 ┃ ┣ 📜 server.js
 ┃ ┣ 📜 package.json
 ┃ ┣ 📜 package-lock.json
 ┃ ┣ 📜 .gitignore
 ┃ ┗ 📜 info.txt-BD

 ┣ 📂 cadastro-usuarios
 ┃ ┣ 📂 public
 ┃ ┃ ┗ 📜 vite.svg
 ┃ ┣ 📂 src
 ┃ ┃ ┣ 📂 assets
 ┃ ┃ ┃ ┗ 📜 icons8-trash-24.svg
 ┃ ┃ ┣ 📂 pages/Home
 ┃ ┃ ┃ ┣ 📜 index.jsx
 ┃ ┃ ┃ ┗ 📜 style.css
 ┃ ┃ ┣ 📂 services
 ┃ ┃ ┃ ┗ 📜 api.js
 ┃ ┃ ┣ 📜 index.css
 ┃ ┃ ┗ 📜 main.jsx
 ┃ ┣ 📜 vite.config.js
 ┃ ┣ 📜 eslint.config.js
 ┃ ┣ 📜 index.html
 ┃ ┣ 📜 package.json
 ┃ ┣ 📜 package-lock.json
 ┃ ┣ 📜 README.md
 ┃ ┗ 📜 .gitignore

 ┗ 📜 README.md
```

---

## ⚙️ Configuração do Backend (API)

### 1️⃣ Instalar dependências
```bash
cd api
npm install
```

### 2️⃣ Criar o arquivo `.env`
Dentro da pasta `api`, crie um arquivo `.env` com o seguinte conteúdo:

```env
DATABASE_URL="mongodb+srv://emersontlsd_db_user:QexgsXidc5neKBtY@<seu-cluster>.mongodb.net/?retryWrites=true&w=majority"
```

> 🔒 **Importante:** substitua `<seu-cluster>` pela URL do seu cluster no **MongoDB Atlas**.

### 3️⃣ Gerar o cliente Prisma
```bash
npx prisma generate
```

### 4️⃣ Executar o servidor
```bash
node server.js
```

A API será executada em:  
👉 **http://localhost:3000**

---

## 🔗 Endpoints da API

| Método | Endpoint | Descrição | Corpo da Requisição |
|:------:|:----------|:----------|:-------------------|
| **POST** | `/usuarios` | Cria um novo usuário | `{ "name": "João", "email": "joao@email.com", "age": "25" }` |
| **GET** | `/usuarios` | Lista todos os usuários | — |
| **PUT** | `/usuarios/:id` | Atualiza um usuário pelo ID | `{ "name": "Novo Nome", "email": "novo@email.com", "age": "30" }` |
| **DELETE** | `/usuarios/:id` | Remove um usuário pelo ID | — |

---

## 💻 Configuração do Frontend (React + Vite)

### 1️⃣ Instalar dependências
```bash
cd cadastro-usuarios
npm install
```

### 2️⃣ Configurar o arquivo `src/services/api.js`
Verifique se o backend está sendo chamado corretamente:
```js
baseURL: 'http://localhost:3000'
```

### 3️⃣ Executar o projeto
```bash
npm run dev
```

O frontend abrirá automaticamente em:  
👉 **http://localhost:5173**

---

## 🧩 Funcionalidades Principais

✅ Cadastrar novos usuários  
✅ Listar usuários em tempo real  
✅ Excluir usuários com um clique  
✅ Interface moderna e responsiva  
✅ Integração direta com API REST via Axios  

---

## 🎨 Layout (CSS)

O estilo foi criado com **CSS puro**, priorizando:
- Cores escuras (modo dark)
- Bordas arredondadas  
- Botões com feedback visual  
- Layout limpo e responsivo  

---

## 🧠 Melhorias Futuras

- Implementar edição direta no frontend  
- Adicionar notificações de sucesso/erro  
- Paginação de usuários  
- Validação de formulários  
- Autenticação com JWT  

---

## 👨‍💻 Autor

**Emerson Souza**  
💼 Desenvolvedor Full Stack  
📞 [WhatsApp (https://wa.me/5561982858372)]  
📧 [E-mail (emersontlsd@gmail.com)]  
🧑‍💻 [GitHub (https://github.com/Emersontlsd)]
