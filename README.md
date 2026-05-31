# Spring Boot CRUD API

Projeto de estudo desenvolvido para praticar conceitos fundamentais do ecossistema Spring Boot.

A aplicação implementa um CRUD (Create, Read, Update e Delete) de produtos utilizando uma API REST integrada ao PostgreSQL.

O projeto foi desenvolvido seguindo o tutorial "Seu primeiro CRUD em Java com Spring", servindo como base para aprendizado de desenvolvimento backend com Java.

## Tecnologias

* Java 17
* Spring Boot 3
* Spring Data JPA
* PostgreSQL
* Docker
* Maven

## Conceitos praticados

* API REST
* Controllers
* Services
* Repositories
* JPA/Hibernate
* Persistência de dados
* Injeção de dependência
* Docker Compose
* Integração com PostgreSQL

## Estrutura do projeto

```text
src
├── controller
├── entity
├── repository
├── service
└── resources
```

## Funcionalidades

* Criar produto
* Buscar produto por ID
* Atualizar produto
* Excluir produto

## Executando o projeto

### Subir o PostgreSQL

```bash
docker compose up -d
```

### Executar a aplicação

```bash
mvn spring-boot:run
```

A API ficará disponível em:

```text
http://localhost:8081
```

## Endpoints

| Método | Endpoint        | Descrição         |
| ------ | --------------- | ----------------- |
| POST   | /api/stock      | Criar produto     |
| GET    | /api/stock/{id} | Buscar produto    |
| PUT    | /api/stock/{id} | Atualizar produto |
| DELETE | /api/stock/{id} | Excluir produto   |

## Próximos passos

Melhorias que pretendo implementar para aprofundar os estudos:

* DTOs
* Bean Validation
* Tratamento global de exceções
* Swagger/OpenAPI
* Testes unitários
* Spring Security com JWT
* Deploy da aplicação

```
```
