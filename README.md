[![Build Status](https://travis-ci.org/rmanguinho/clean-ts-api.svg?branch=master)](https://travis-ci.org/rmanguinho/clean-ts-api)
[![Coverage Status](https://coveralls.io/repos/github/rmanguinho/clean-ts-api/badge.svg)](https://coveralls.io/github/rmanguinho/clean-ts-api)
[![Known Vulnerabilities](https://snyk.io/test/github/rmanguinho/clean-ts-api/badge.svg)](https://snyk.io/test/github/rmanguinho/clean-ts-api)
[![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg)](http://standardjs.com)
[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
[![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)

# **Clean Node API**

[![alt text](./public/img/logo-course.png "Link para o treinamento")](https://www.udemy.com/course/tdd-com-mango/?referralCode=B53CE5CA2B9AFA5A6FA1)

---

## [**Link para o curso completo**](https://www.udemy.com/course/tdd-com-mango/?referralCode=B53CE5CA2B9AFA5A6FA1)

Essa API faz parte do treinamento do professor Rodrigo Manguinho (Mango) na Udemy.

O objetivo do treinamento é mostrar como criar uma API com uma arquitetura bem definida e desacoplada, utilizando TDD (programação orientada a testes) como metodologia de trabalho, Clean Architecture para fazer a distribuição de responsabilidades em camadas, sempre seguindo os princípios do SOLID e, sempre que possível, aplicando Design Patterns para resolver alguns problemas comuns.

## [**Link para a documentação da API**](http://fordevs.herokuapp.com/api-docs)

> ## APIs construídas no treinamento

1. [Cadastro](./requirements/signup.md)
2. [Login](./requirements/login.md)
3. [Criar enquete](./requirements/add-survey.md)
4. [Listar enquetes](./requirements/load-surveys.md)
5. [Responder enquete](./requirements/save-survey-result.md)
6. [Resultado da enquete](./requirements/load-survey-result.md)

> ## Princípios

* Single Responsibility Principle (SRP)
* Open Closed Principle (OCP)
* Liskov Substitution Principle (LSP)
* Interface Segregation Principle (ISP)
* Dependency Inversion Principle (DIP)
* Separation of Concerns (SOC)
* Don't Repeat Yourself (DRY)
* You Aren't Gonna Need It (YAGNI)
* Keep It Simple, Silly (KISS)
* Composition Over Inheritance
* Small Commits

> ## Design Patterns

* Factory
* Adapter
* Composite
* Decorator
* Proxy
* Dependency Injection
* Abstract Server
* Composition Root
* Builder
* Singleton

> ## Metodologias e Designs

* TDD
* Clean Architecture
* DDD
* Conventional Commits
* GitFlow
* Modular Design
* Dependency Diagrams
* Use Cases
* Continuous Integration
* Continuous Delivery
* Continuous Deployment

> ## Bibliotecas e Ferramentas

* NPM
* Typescript
* Git
* Docker
* Jest
* MongoDb
* Travis CI
* Swagger
* Bcrypt
* JsonWebToken
* Faker
* Coveralls
* Validator
* Express
* Apollo Server Express
* Graphql
* Graphql ISO Date
* Supertest
* Husky
* Lint Staged
* Eslint
* Standard Javascript Style
* Sucrase
* Nodemon
* Rimraf
* In-Memory MongoDb Server
* MockDate
* Module-Alias
* Copyfiles
* Npm Check
* Bson ObjectId
* Apollo Server Integration Testing

> ## Features do Node

* Documentação de API com Swagger
* API Rest com Express
* GraphQL com Apollo Server
* Log de Erro
* Segurança (Hashing, Encryption e Encoding)
* CORS
* Middlewares
* Nível de Acesso nas Rotas (Admin, User e Anônimo)
* Deploy no Heroku
* Servir Arquivos Estáticos

> ## Features do GraphQL

* Types
* Queries
* Mutations
* Resolvers
* Directives
* Scalars
* Plugins

> ## Features do Git

* Alias
* Log Personalizado
* Branch
* Reset
* Amend
* Tag
* Stash
* Rebase
* Merge

> ## Features do Typescript

* POO Avançado
* Interface
* TypeAlias
* Namespace
* Utility Types
* Modularização de Paths
* Configurações
* Build
* Deploy
* Uso de Breakpoints

> ## Features de Testes

* Testes Unitários
* Testes de Integração (API Rest & GraphQL)
* Cobertura de Testes
* Test Doubles
* Mocks
* Stubs
* Spies
* Fakes

> ## Features do MongoDb

* Connect e Reconnect
* Collections
* InsertOne e InserMany
* Find, FindOne e FindOneAndUpdate
* DeleteMany
* UpdateOne
* Aggregation (Match, Group, Unwind, Lookup, AddFields, Project, Sort)
* ObjectId
* Upsert e ReturnOriginal
* Push, Divide, Multiply, ArrayElemAt, Cond, Sum
* Filter, Map, Reduce, MergeObjects, ConcatArrays

> ## Setup Inicial:

```
[alias]
	s = !git status -s
	c = !git add --all && git commit -m
	l = !git log --pretty=format:'%C(blue) %h %C(red)%d %C(white)%s - %C(cyan)%cn, %C(green)%cr'
```

Criar alias para os comandos do git

```git log --pretty=format:'%C(blue) %h %C(red) %d %C(white) %s - %C(cyan) %cn, %C(green) %cr'```

```%C(color) - cor das proximas informações```

```%h = hash reduzida```

```%d = branch```

```%s = subject ou mensagem do commit```

```%cn = committer name```

```%cr = data do commit```

Conventional Commits

chore = add new config, setup or lib
add git-commit-msg-linter 

```
git c "add commit linter"

************* Invalid Git Commit Message **************
  commit message: add commit linter
  correct format: <type>(<scope>): <subject>
  example: docs: update README add developer tips

  type:
    feat     A new feature
    fix      A bug fix
    docs     Documentation only changes
    style    Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
    refactor A code change that neither fixes a bug nor adds a feature
    test     Adding missing tests or correcting existing ones
    chore    Changes to the build process or auxiliary tools and libraries such as documentation generation
    perf     A code change that improves performance
    ci       Changes to your CI configuration files and scripts
    build    Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)
    temp     Temporary commit that won't be included in your CHANGELOG

  scope:
    Optional, can be anything specifying the scope of the commit change.
    For example $location, $browser, $compile, $rootScope, ngHref, ngClick, ngView, etc.
    In App Development, scope can be a page, a module or a component.

  subject:
    Brief summary of the change in present tense. Not capitalized. No period at the end.```