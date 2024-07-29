
# DSMovie

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](https://github.com/hakkinenT/spring-boot-dsmovie-jacoco/blob/main/LICENSE) 
![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)
![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![Hibernate](https://img.shields.io/badge/Hibernate-59666C?style=for-the-badge&logo=Hibernate&logoColor=white)

## Tabela de Conteúdo
- [Sobre o projeto](#sobre-o-projeto)
- [Modelo Conceitual](#modelo-conceitual)
- [Requisitos](#requisitos)
- [Documentação da API](#documentação-da-api)
    - [Acessando localmente](#acessando-localmente) 
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Rodando localmente](#rodando-localmente)
- [Rodando os testes](#rodando-os-testes)
- [Autores](#autores)

<a id="sobre-o-projeto"></a>
## Sobre o projeto
Este projeto foi desenvolvido ao longo do curso Java Spring Expert da DevSuperior, ministrado pelo Professor Nelio Alves. O  objetivo deste projeto foi desenvolver uma API  de filmes e avaliações de filmes, aplicando os conceitos de Testes Unitários e de Integração e também de cobertura de testes usando a ferramenta Jacoco.

<a id="modelo-conceitual"></a>
## Modelo Conceitual
![App Class Diagram](https://github.com/hakkinenT/assets/blob/master/dsmovie-modelo-conceitual.png)

<a id="requisitos"></a>
## Requisitos
- [Java JDK (versão 17 ou superior)](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)
- [Git](https://git-scm.com/downloads) - Sistema de controle de versão de código aberto
- [Uma conta no Github](https://github.com/) - Plataforma de controle de versões
- [Postman](https://www.postman.com/downloads/) ou [Insomnia](https://insomnia.rest/download) - Ferramentas para testar a API

<a id="documentação-da-api"></a>
## Documentação da API

<a id="acessando-localmente"></a>
### Acessando localmente

1. [Rode a aplicação localmente](#rodando-localmente)
2. Gere um token de acesso
- Abra um ferramenta para testar a API (Postman, Insomnia...)
- Acesse a url abaixo:
```bash
http://localhost:8080/oauth2/token
```
- Na aba Authorization, acrescente as seguintes informações:
    - Em Auth Type selecione Basic Auth
    - Preencha os campos Username e Password com os seguintes valores:

        | Campo   | Valor       | Descrição                           |
        | :---------- | :--------- | :---------------------------------- |
        | Username | {{client-id}} | Valor do client-id definido no application.properties |
        | Password | {{client-secret}} | Valor do client-secret definido no application.properties |

- Envie a requisição e obtenha o token
- Acesse o endereço:
```bash
  http://localhost:8080/swagger-ui.html
```
- Adicone o token em Authorize
- Acesse as rotas

<a id="tecnologias-utilizadas"></a>
## Tecnologias Utilizadas

- Java
- Spring Boot
- Banco de Dados H2
- JPA/Hibernate
- Bean Validation
- Spring Security
- OAuth2
- JUnit
- Spring Security Test
- Jacoco

<a id="rodando-localmente"></a>
## Rodando localmente

Clone o projeto

```bash
  git clone https://github.com/hakkinenT/spring-boot-dsmovie-jacoco
```

Entre no diretório do projeto

```bash
  cd spring-boot-dsmovie-jacoco
```

Instale as dependências

```bash
  mvn install
```

Rode a aplicação

```bash
  ./mvnw spring-boot:run
```

<a id="rodando-os-testes"></a>
## Rodando os testes

Para rodar os testes, rode o seguinte comando

```bash
    mvn test
```

<a id="autores"></a>
## Autores

- [@hakkinenT](https://github.com/hakkinenT)
