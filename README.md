
# DSMovie

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](https://github.com/hakkinenT/spring-boot-dsmovie-jacoco/blob/main/LICENSE) 
![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)
![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![Hibernate](https://img.shields.io/badge/Hibernate-59666C?style=for-the-badge&logo=Hibernate&logoColor=white)

# DSMovie 🎬

API REST para avaliação de filmes, desenvolvida com foco em **qualidade de código**, **testes automatizados** e **análise de cobertura de testes** utilizando **Jacoco**.

## 🚀 Funcionalidades
- Cadastro e listagem de filmes
- Avaliação de filmes por usuários
- Cálculo automático da média de avaliações
- Validações e tratamento de exceções

## 🛠️ Tecnologias Utilizadas
- Java
- Spring Boot
- Spring Data JPA
- PostgreSQL
- JUnit
- Mockito
- Jacoco
- Maven

## ▶️ Como executar o projeto

### Pré-requisitos
- Java 17+
- Maven
- PostgreSQL (ou Docker)

### Passos
1. Clone o repositório:
```bash
git clone https://github.com/hakkinenT/spring-boot-dsmovie-jacoco.git
```
2. Acesse o diretório do projeto:

```bash
cd spring-boot-dsmovie-jacoco
```

3. Execute a aplicação:
```bash
mvn spring-boot:run
```

4. A aplicação estará disponível em:
```arduino
http://localhost:8080
```

## 🔐 Autenticação e Autorização

A API utiliza JWT (JSON Web Token) para autenticação.

Após realizar o login, o token retornado deve ser enviado no header das requisições protegidas:

```http
Authorization: Bearer <token>
```

## 📌 Endpoints

### 🔓 Públicos

| Método | Rota             | Descrição                    |
|------|------------------|------------------------------|
| GET  | /movies          | Lista filmes (paginado)      |
| GET  | /movies/{id}     | Busca filme por ID           |


### 🔒 Protegidos

| Método | Rota             | Descrição              |
|------|------------------|------------------------|
| POST | /movies          | Cria um novo filme     |
| PUT  | /movies/{id}     | Atualiza um filme      |
| DELETE | /movies/{id}   | Remove um filme        |
| POST | /scores                 | Avalia um filme                        |

A rota de avaliação permite que usuários atribuam notas aos filmes,
sendo utilizada para o cálculo da média de avaliações exibida na listagem.

## 📦 Testando a API com Postman

O projeto disponibiliza arquivos do Postman para facilitar o teste da API:

- 📁 Collection: contém todas as requisições da API

- 🌍 Environment: contém variáveis de ambiente, como URL base e token

Como utilizar:

1. Abra o Postman

2. Importe a collection (.json)

3. Importe o environment (.json)

4. Selecione o environment no Postman

5. Execute a requisição de login para obter o token

6. As requisições protegidas utilizarão automaticamente o token salvo no environment

## 🧪 Testes e Qualidade
- Testes unitários com JUnit
- Uso de Mockito para mocks
- Análise de cobertura de código com **Jacoco**

Executar todos os testes:
```bash
mvn test
```

## 📊 Cobertura de Testes

Este projeto utiliza **Jacoco** para análise de cobertura de testes.

Após executar os testes, o relatório pode ser acessado em:

```html
target/site/jacoco/index.html
```

## 📌 Objetivo do Projeto

Projeto com foco em boas práticas de testes, métricas de qualidade e confiabilidade de software.
## Autores

- [@hakkinenT](https://github.com/hakkinenT)
