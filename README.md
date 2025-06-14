📚 API REST - Escola
API RESTful desenvolvida com Node.js e Express para gerenciar dados escolares, incluindo alunos, professores, turmas e disciplinas.

🚀 Tecnologias Utilizadas
Node.js

Express.js

MongoDB (via Mongoose)

JSON Web Tokens (JWT) para autenticação

Dotenv para variáveis de ambiente

📦 Instalação
Clone o repositório:

bash
Copiar
Editar
git clone https://github.com/S4antiago33/api-rest-escola.git
cd api-rest-escola
Instale as dependências:

bash
Copiar
Editar
npm install
Configure as variáveis de ambiente:

Crie um arquivo .env na raiz do projeto e adicione as seguintes variáveis:

env
Copiar
Editar
PORT=3000
MONGODB_URI=mongodb://localhost:27017/escola
JWT_SECRET=sua_chave_secreta
Inicie o servidor:

bash
Copiar
Editar
npm start
O servidor estará disponível em http://localhost:3000.

🛠️ Endpoints
Alunos
GET /alunos - Lista todos os alunos

GET /alunos/:id - Retorna um aluno específico

POST /alunos - Cria um novo aluno

PUT /alunos/:id - Atualiza um aluno existente

DELETE /alunos/:id - Remove um aluno

Professores
GET /professores - Lista todos os professores

GET /professores/:id - Retorna um professor específico

POST /professores - Cria um novo professor

PUT /professores/:id - Atualiza um professor existente

DELETE /professores/:id - Remove um professor

Turmas
GET /turmas - Lista todas as turmas

GET /turmas/:id - Retorna uma turma específica

POST /turmas - Cria uma nova turma

PUT /turmas/:id - Atualiza uma turma existente

DELETE /turmas/:id - Remove uma turma

Disciplinas
GET /disciplinas - Lista todas as disciplinas

GET /disciplinas/:id - Retorna uma disciplina específica

POST /disciplinas - Cria uma nova disciplina

PUT /disciplinas/:id - Atualiza uma disciplina existente

DELETE /disciplinas/:id - Remove uma disciplina

🔐 Autenticação
A autenticação é realizada via JWT. Para acessar rotas protegidas:

Faça login:

bash
Copiar
Editar
POST /login
Envie as credenciais no corpo da requisição:

json
Copiar
Editar
{
  "email": "usuario@example.com",
  "senha": "sua_senha"
}
Receba o token JWT e inclua-o no cabeçalho das requisições subsequentes:

http
Copiar
Editar
Authorization: Bearer seu_token_jwt
🧪 Testes
Para executar os testes (caso implementados):

bash
Copiar
Editar
npm test
📄 Licença
Este projeto está licenciado sob a MIT License.
