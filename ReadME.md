# Aplicativo de Controle de Finanças Pessoais

## Descrição do Projeto

O Aplicativo de Controle de Finanças Pessoais é um projeto Java com Spring que permite aos usuários gerenciar suas finanças de forma eficiente. Os usuários podem registrar despesas, receitas e criar orçamentos.

## Segmento

Este projeto pertence ao segmento de **Fintech**, fornecendo ferramentas para que os usuários controlem suas finanças pessoais, economizem dinheiro e melhorem seu bem-estar financeiro.

## Tecnologias Utilizadas

- Java
- Spring Framework (Spring Boot)
- Banco de Dados (por exemplo, MySQL)
- RabbitMQ (Opcional, para mensageria)
- Swagger (Documentação da API)

## Entidades

O sistema lida com as seguintes entidades:

- **Usuário:** Representa um usuário do aplicativo com informações como nome, email e senha.
- **Conta Bancária:** Permite aos usuários criar e gerenciar suas contas bancárias.
- **Categoria de Despesa/Receita:** Categoriza despesas e receitas.
- **Transação:** Registra transações financeiras, incluindo data, valor, descrição, categoria e a conta associada.

## Endpoints (Controllers)

### UserController

- **POST /api/user/register:** Cria uma nova conta de usuário.
- **POST /api/user/login:** Autentica o usuário.

### AccountController

- **POST /api/account/create:** Cria uma nova conta bancária.
- **GET /api/account/{accountId}:** Obtém informações detalhadas de uma conta.

### TransactionController

- **POST /api/transaction/create:** Registra uma nova transação financeira.
- **GET /api/transaction/{transactionId}:** Obtém detalhes de uma transação específica.

### CategoryController

- **POST /api/category/create:** Cria novas categorias de despesas/receitas.
- **GET /api/category/list:** Lista todas as categorias disponíveis.

## Configuração e Execução

1. Clone este repositório: `git clone https://github.com/`
2. Configure as informações do banco de dados no arquivo `application.properties`.
3. Execute a aplicação Spring Boot.

## Documentação da API

A documentação da API pode ser acessada em `/swagger-ui.html`. Use o Swagger para explorar e testar os endpoints da API.

## Licença

Este projeto é distribuído sob a licença [MIT](LICENSE).
