<p align="center">
  <img src=".github/capa-ignite-nodejs.png" alt="Ignite Node.js">
</p>

<br>

<h1 align="center">
  Ignite

  <br>

  Trilha Node.js (aulas)
</h1>

<br>

<p align="center">
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="Node.js">
  <img src="https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E" alt="JavaScript">
  <img src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript">
  <img src="https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white" alt="Express.js">
  <img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL">
  <img src="https://img.shields.io/badge/JWT-e53d00?style=for-the-badge&logo=JSON%20web%20tokens&logoColor=white" alt="JWT">
  <img src="https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white" alt="Docker">
</p>

## :computer: Descrição:
Esta é uma API que tem como função permitir que um cliente contrate serviços de um profissional através de um atendimento gerenciado por um atendente, o cliente solicita o atendimento de algum(uns) serviço(s), o atendente passa os serviços solicitados para o professional que os realiza. Para cada serviço realizado o profissional receberá uma comissão em percentual do valor do serviço. A aplicação gera um relatório do atendimento e o atendente o passa para o cliente, no relatório tem o valor total dos serviços, quanto tempo vai levar para os serviços serem concluídos e o valor da comisão que o profissional irá receber. Com a execução do projeto é possível acessar a documentação da API desenvolvida com o [Swagger](https://swagger.io/).

## :hammer_and_wrench: Funcionalidades:
- [x]  Criar um novo usuário com `nome`, `email`, `senha`, `CPF` e `telefone`.
- [x]  Criar um novo atendente com `nome`, `email`, `senha`.
- [x]  Cadastrar um profissonal com `nome` e `telefone`.
- [x]  Cadastrar os serviços prestador com `nome`, `valor`, `tempo`, `porcentagem`.
- [x]  Listar os serviços.
- [x]  Listar os profissionais.
- [x]  Atendente gerar relatório do atendimento com `comissão`, `tempo total`, `valor total`.
- [x]  Fazer login no sistema (atentende | cliente).

## :link: Rotas:
- POST `/clients`: cria um novo cliente.
- POST `/attendants`: cria um novo atendente.
- POST `/professionals`: cria um novo profissional.
- POST `/services`: cria um novo serviço.
- POST `/treatment`: cria o atendimento.
- POTS `/summary`: cria o relatório
- GET `/professionals`: retorna todos os profisionais cadastrados.
- GET `/services`: retorna todos os serviços que são prestados.
- GET `/summary/{client_id}`: retorna o relatório do usuário.
- `localhost:3333/api-docs`: documentação da API com Swagger.

## :memo: Execução da API:
- Instalar as dependências, iniciar o banco de dados, rodas as migrations, rodar o seed e executar a API:
  > docker-compose up
- Execução dos testes unitários:
  > yarn test

## :information_source: Documentação:
[Atlas API](http://localhost:3333/api-docs)
