# Sistema de Gestão de Clientes
📋 Descrição

Sistema web desenvolvido em Java com JSF para gerenciamento de cadastro de clientes. A aplicação permite realizar operações básicas de CRUD (Create, Read, Update e Delete) e integra-se com o serviço ViaCEP para consulta automática de endereços.


# 🛠️ Tecnologias Utilizadas

-   Java 8
-   JavaServer Faces (JSF)
-   PrimeFaces 8.0
-   JPA/Hibernate
-   Banco de dados H2 (em memória)
-   Maven
- Tomcat na versão 8.5

## ⚙️ Funcionalidades

-   Cadastro de clientes
-   Pesquisa de clientes por nome
-   Edição de dados cadastrais
-   Exclusão de registros
-   Busca automática de endereço por CEP
-   Validação de email único
-   Interface responsiva

## 🚀 Como Executar o Projeto

### Pré-requisitos

-   JDK 8 ou superior
-   Maven
-   Servidor de aplicação (ex: Tomcat 8 ou superior)
### Configuração

1.  Clone o repositório:

	`git clone https://github.com/seu-usuario/nome-do-repositorio.git`

2.  Navegue até o diretório do projeto:

	`cd nome-do-repositorio`

3.  Compile o projeto:

	`mvn clean install`

4.  Deploy o arquivo WAR gerado no seu servidor de aplicação.

### Acesso

-   Aplicação: [http://localhost:8080/crud_cliente](http://localhost:8080/nome-do-projeto)
-   Console H2: [http://localhost:8080/crud_cliente/h2-console](http://localhost:8080/nome-do-projeto/h2-console)
    -   JDBC URL: jdbc:h2:mem:clientedb
    -   User: sa
    -   Password: (deixar em branco)
   
## 📝 Detalhes da Implementação

### Modelo de Dados

A entidade Cliente possui os seguintes atributos:

-   ID (Long, auto-incremento)
-   Nome (String, obrigatório)
-   Email (String, obrigatório, único)
-   Telefone (String)
-   CEP (String, obrigatório)
-   Endereço (String, obrigatório)
-   Bairro (String, obrigatório)
-   Cidade (String, obrigatório)
-   Estado (String, obrigatório)

### Camadas da Aplicação

-   **Bean**: Contém os managed beans do JSF que controlam a interface
-   **DAO**: Camada de acesso a dados com as operações no banco
-   **Model**: Classes de modelo/entidades JPA
-   **Service**: Serviços da aplicação, incluindo integração com ViaCEP
-   **Util**: Classes utilitárias, como gerenciamento de EntityManager

## 🤝 Contribuindo

-   Faça um fork do projeto
-   Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
-   Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
-   Push para a branch (`git push origin feature/AmazingFeature`)
-   Abra um Pull Request

## 📄 Licença

Este projeto está sob a licença de Isaac Nunes. 

# ✒️ Autor


**Isaac Nunes - @isaacnngt - isaacnngt@gmail.com** 

## 🎁 Expressões de Gratidão

-   Conte a outras pessoas sobre este projeto 📢
-   Um agradecimento publicamente 🤓
