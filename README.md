# Java Spring Boot Application with Docker

Projeto desenvolvido com **Java e Spring Boot**, com foco na **containerização de aplicações utilizando Docker**.

A aplicação foi empacotada em uma imagem Docker e executada dentro de um container, utilizando mapeamento de portas para acesso local.

## 🐳 Tecnologias

- Docker
- Dockerfile
- Java
- Spring Boot
- Maven
- Git
- GitHub

## 📋 Sobre o projeto

O objetivo principal deste projeto foi colocar em prática conceitos fundamentais de **Docker e containerização de aplicações**.

Durante o desenvolvimento, foram trabalhados conceitos como:

- Criação de Dockerfile
- Construção de imagens Docker
- Execução de containers
- Mapeamento de portas
- Utilização de imagens base
- Multi-stage build
- Empacotamento de aplicações Java em JAR
- Execução de aplicações Spring Boot dentro de containers
- Versionamento do projeto com Git e GitHub

## 🐳 Dockerfile

O projeto utiliza um **Dockerfile com Multi-Stage Build**.

Na primeira etapa, o Maven é utilizado para realizar o build da aplicação e gerar o arquivo `.jar`.

Na segunda etapa, é utilizada uma imagem mais leve contendo apenas o ambiente necessário para executar a aplicação Java.

Essa abordagem permite separar o processo de **build** do ambiente final de **execução**.

### Estrutura simplificada

```text
Código Java
     ↓
   Maven
     ↓
   JAR
     ↓
 Dockerfile
     ↓
 Docker Image
     ↓
 Docker Container
     ↓
 Spring Boot
