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
</p>

## :computer: Descrição:
Esta é uma API que tem como função permitir que um cliente contrate serviços de um profissional através de um atendimento gerenciado por um atendente, o cliente solicita o atendimento de algum(uns) serviço(s), o atendente passa os serviços solicitados para o professional que realizar o serviço. Para cada serviço realizado o profissional receberá uma comissão em percentual do valor do serviço. A aplicação gera um relatório do atendimento e o atendente o passa para o cliente, no relatório tem o valor total dos serviços, quanto tempo vai levar para os serviços serem concluídos e o valor da comisão que o profissional irá receber. Com a execução do projeto é possível acessar a documentação da API desenvolvida com o [Swagger](https://swagger.io/).

## :hammer_and_wrench: Funcionalidades:
- [x]  Criar um novo usuário com `nome`, `email`, `senha`, `CPF` e `telefone`.
- [x]  Criar um novo atendente com `nome`, `email`, `senha`, e `função (administrador | básico)`.
- [x]  Cadastrar um profissonal com `nome` e `telefone`.
- [x]  Cadastrar os serviços prestador com `nome`, `valor`, `tempo`, `porcentagem`.
- [x]  Listar os serviços.
- [x]  Listar os profissionais.
- [x]  Atendente gerar relatório do atendimento com `comissão`, `tempo total`, `valor total`.
- [x]  Fazer login no sistema (atentende | cliente).

## :link: Rotas:
- POST `/users`: cria um novo usuário.
- GET `/users`: retorna todos os usuários.
- GET `/users/{user_id}`: retorna um usuário específico.
- PATCH `users/{user_id}/admin`: torna um usuário em admin.

## :memo: Execução da API:
- Instalação das dependências:
  > yarn
- Execução da API:
  > yarn dev
- Execução dos testes:
  > yarn test

## :information_source: Documentação:
[Atlas API](http://localhost:3333/api-docs)
