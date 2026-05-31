# Product Management API

API REST desenvolvida com Java e Spring Boot para gerenciamento de produtos.

Este projeto foi criado com objetivo de praticar conceitos fundamentais do desenvolvimento backend moderno utilizando Java, Spring Boot, PostgreSQL e Docker.

## Tecnologias Utilizadas

* Java 17
* Spring Boot 3
* Spring Web
* Spring Data JPA
* PostgreSQL 16
* Docker
* Maven
* Lombok

## Arquitetura

O projeto segue uma arquitetura em camadas:

```text
controller  -> Recebe requisições HTTP
service     -> Regras de negócio
repository  -> Acesso aos dados
entity      -> Modelagem das entidades
```

## Funcionalidades

* Criar produto
* Listar produtos
* Buscar produto por ID
* Atualizar produto
* Remover produto

## Executando o Projeto

### 1. Clonar o repositório

```bash
git clone https://github.com/seu-usuario/product-management-api.git
```

### 2. Subir o PostgreSQL

```bash
docker compose up -d
```

### 3. Executar a aplicação

```bash
mvn spring-boot:run
```

A aplicação ficará disponível em:

```text
http://localhost:8080
```

## Endpoints

### Criar produto

POST /products

```json
{
  "name": "Notebook",
  "price": 4500
}
```

### Listar produtos

GET /products

### Buscar produto por ID

GET /products/{id}

### Atualizar produto

PUT /products/{id}

```json
{
  "name": "Notebook Gamer",
  "price": 6500
}
```

### Remover produto

DELETE /products/{id}

## Banco de Dados

O banco PostgreSQL é executado em container Docker através do arquivo docker-compose.yml.

## Aprendizados

Durante o desenvolvimento deste projeto foram praticados os seguintes conceitos:

* Desenvolvimento de APIs REST
* Spring Boot
* Injeção de Dependências
* JPA/Hibernate
* Persistência de dados com PostgreSQL
* Docker
* Maven
* Arquitetura em camadas
* Operações CRUD

## Próximas Melhorias

* DTOs
* Bean Validation
* Tratamento global de exceções
* Swagger/OpenAPI
* Spring Security + JWT
* Testes unitários
* Dockerização completa da aplicação
* Deploy em nuvem

```
```
