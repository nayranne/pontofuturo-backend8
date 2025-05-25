# 🚀 PontoFuturo Backend

Backend da plataforma **PontoFuturo**, que permite a **conversão de pontos de programas de fidelidade e cashback em aportes para fundos de previdência privada**.

## 🔗 Tecnologias Utilizadas
- **Node.js**
- **Express**
- **MongoDB**
- **Mongoose**
- **JWT**
- **BcryptJS**
- **Dotenv**
- **CORS**

## 📁 Estrutura do Projeto
```
pontofuturo-backend/
├── .replit
├── replit.nix
├── package.json
├── .env.example
├── README.md
├── app.js
└── src/
    ├── config/
    ├── controllers/
    ├── middlewares/
    ├── models/
    ├── routes/
    └── services/
```

## ⚙️ Instalação e Execução Local
### 🔥 Pré-requisitos:
- Node.js instalado (>= 18)
- MongoDB Atlas ou local
- Git instalado

### ✅ Passo a passo:
1. Clone o repositório:
```bash
git clone https://github.com/nayranne/pontofuturo-backend.git
cd pontofuturo-backend
```

2. Instale as dependências:
```bash
npm install
```

3. Configure o arquivo `.env`:
```plaintext
SECRET=seu_segredo_jwt
MONGO_URI=sua_string_de_conexao_do_mongodb
PORT=3000
```

4. Execute o servidor:
```bash
npm start
```
✔️ O backend estará rodando em:
```
http://localhost:3000
```

## 🚀 Como Executar no Replit
1. Crie um novo Repl.
2. Importe do GitHub ou envie os arquivos.
3. No console execute:
```bash
npm install
npm start
```
4. Crie o arquivo `.env` no Replit:
```
SECRET=seu_segredo_jwt
MONGO_URI=sua_string_de_conexao_do_mongodb
PORT=3000
```
5. O link do backend será algo como:
```
https://pontofuturo-backend.seunome.repl.co
```

## 🔐 Variáveis de Ambiente
| Variável   | Descrição                         |
| ----------- | ---------------------------------- |
| `SECRET`    | Chave secreta para JWT            |
| `MONGO_URI` | String de conexão MongoDB         |
| `PORT`      | Porta do servidor (padrão 3000)   |

## 📦 Comandos Disponíveis
| Comando        | Descrição                |
|----------------|---------------------------|
| `npm install`  | Instala dependências      |
| `npm start`    | Inicia o servidor         |

## 📑 Documentação da API
### 🔐 Autenticação
- `POST /api/auth/register` — Cadastro
- `POST /api/auth/login` — Login (retorna token)

### 💰 Aportes
- `GET /api/aportes` — Listar aportes (🔐)

### 🎯 Pontos
- `GET /api/pontos/saldo` — Consultar saldo (🔐)
- `POST /api/pontos/converter` — Converter pontos (🔐)

### 📜 Rota de Teste
- `GET /api/hello` — Teste do servidor

## 🔐 Autenticação JWT
Header para rotas protegidas:
```
Authorization: Bearer <seu_token_jwt>
```

## 💡 Melhorias Futuras
- Integração com APIs de pontos
- Dashboard frontend
- Deploy profissional

## 👨‍💻 Desenvolvido por Nayranne com apoio do ChatGPT 🚀
