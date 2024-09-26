# CashControl API

CashControl API é uma api projetada para auxiliar os usuários no gerenciamento de suas finanças. Esta aplicação oferece funcionalidades como criação de usuários, autenticação, registro de transações financeiras e consulta de saldo. Os dados dos usuários são armazenados localmente usando SQLite.

## Tecnologias Utilizadas

- **Node.js**: Ambiente de execução JavaScript do lado do servidor.
- **TypeScript**: Superset de JavaScript que adiciona tipagem estática e outras funcionalidades ao código.
- **Express.js**: Framework web para Node.js que facilita a criação de APIs.
- **Prisma**: ORM (Object-Relational Mapping) para interagir com o banco de dados de forma simplificada.
- **JWT (JsonWebToken)**: Usado para autenticação, permitindo a geração de tokens seguros de autenticação.
- **Bcrypt.js**: Usado para a hash e comparação segura de senhas.
- **SQLite**: Banco de dados local para armazenamento de dados de usuário.

## Instalação

1. **Clone o Repositório**:
   ```bash
   git clone https://github.com/KevynMurilo/ApiTs.git
   
## Instale as Dependências:
cd ApiTs
npm install

## Configure o Banco de Dados:
Certifique-se de ter um banco de dados SQLite configurado e acessível. Você pode modificar as configurações no arquivo prisma/schema.prisma.

## Execute o Servidor:
npm run dev
O servidor estará disponível em http://localhost:3333.

## Rotas
- **POST /users**: Cria um novo usuário.
- **POST /login**: Autentica um usuário e retorna um token JWT.
- **GET /me**: Retorna informações do usuário autenticado.
- **GET /balance**: Retorna o saldo do usuário autenticado.
- **POST /receive**: Cria uma nova transação de recebimento.
- **GET /receives**: Retorna a lista de transações de recebimento do usuário autenticado.
- **DELETE /receives/delete**: Deleta uma transação de recebimento.

## Middlewares
- **isAuthenticated**: Verifica se o usuário está autenticado.

## Observações
- Este projeto utiliza TypeScript para uma melhor organização e tipagem do código.
- Recomenda-se configurar um banco de dados SQLite ou outro banco de dados compatível com Prisma.
