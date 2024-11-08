# Fundamentos Node.js

Este projeto é uma aplicação Node.js que demonstra os fundamentos do desenvolvimento de servidores HTTP, manipulação de streams e operações básicas de CRUD em um banco de dados JSON.

## Estrutura do Projeto

### Descrição dos Arquivos

- `db.json`: Arquivo JSON que armazena os dados do banco de dados.
- `package.json`: Arquivo de configuração do npm com as dependências e scripts do projeto.
- `src/`: Diretório que contém o código-fonte principal da aplicação.
  - `database.js`: Implementa a classe `Database` para operações CRUD.
  - `middlewares/json.js`: Middleware para parsear o corpo das requisições JSON.
  - `routes.js`: Define as rotas da aplicação.
  - `server.js`: Configura e inicia o servidor HTTP.
  - `utils/`: Diretório com utilitários.
    - `build-route-path.js`: Função para construir expressões regulares de rotas.
    - `extract-query-params.js`: Função para extrair parâmetros de query strings.
- `streams/`: Diretório com exemplos de manipulação de streams.
  - `buffer.js`: Exemplo de criação e manipulação de buffers.
  - `fake-upload-to-http-stream.js`: Exemplo de upload de dados via stream HTTP.
  - `stream-http-server.js`: Exemplo de servidor HTTP que manipula streams.

## Instalação

1. Clone o repositório:
   ```sh
   git clone git@github.com:Caarlos7x/ignite-nodejs-01-fundamentos-nodejs.git


2. Navegue até o diretório do projeto:
    ```sh
    cd aulas/01-fundamentos-nodejs


3. Instale as dependências:
    ```sh
    npm install

## Uso

- Para iniciar o servidor em modo de desenvolvimento, execute:
    ```sh
    npm run dev

O servidor estará disponível em http://localhost:3000.

## Rotas
- `GET /users`: Retorna a lista de usuários.
- `POST /users`: Cria um novo usuário.
- `PUT /users/:id`: Atualiza um usuário existente.
- `DELETE /users/:id`: Remove um usuário.

## Exemplos de Streams
- `buffer.js`: Executa um exemplo de manipulação de buffers.
- `fake-upload-to-http-stream.js`: Simula o upload de dados via stream HTTP.
- `stream-http-server.js`: Inicia um servidor HTTP que manipula streams.

## Licença
Este projeto está licenciado sob a licença ISC.
