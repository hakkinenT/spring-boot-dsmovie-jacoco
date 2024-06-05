
# DSMovie

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](https://github.com/hakkinenT/spring-boot-dsmovie-jacoco/blob/main/LICENSE) 
![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)
![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![Hibernate](https://img.shields.io/badge/Hibernate-59666C?style=for-the-badge&logo=Hibernate&logoColor=white)

## Tabela de Conteúdo
- [Sobre o projeto](#sobre-o-projeto)
- [Modelo Conceitual](#modelo-conceitual)
- [Documentação da API](#documentação-da-api)
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

<a id="documentação-da-api"></a>
## Documentação da API
1. [Rode a aplicação](#rodando-localmente)
2. Acesse o endereço abaixo
  ```bash
    http://localhost:8080/swagger-ui.html
  ```


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
