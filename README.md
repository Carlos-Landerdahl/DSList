# Aplicação Backend do Sistema de Listas de Games (DSList)

Este é o arquivo README para a aplicação backend do sistema de listas de games. Nesta aplicação, você pode criar listas personalizadas de jogos e movimentar os itens dentro das listas para reorganizá-los.
![Modelo do Sistema de Listas de Games](https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/dslist-model.png)


## Tecnologias Utilizadas:

- Java
- Spring Boot
- JPA (Java Persistence API)
- H2 (Banco de Dados em Memória)
- PostgreSQL (Banco de Dados Relacional)
- Railway (Hospedagem e Integração CI/CD)
- Docker

## Configuração do Ambiente

### Pré-requisitos

Certifique-se de ter as seguintes ferramentas instaladas em seu ambiente de desenvolvimento:

- Java Development Kit (JDK) 8 ou superior
- Maven
- Docker

### Configuração do Banco de Dados

A aplicação utiliza tanto o banco de dados H2 em memória para desenvolvimento quanto o PostgreSQL para ambiente de produção. Para configurar a conexão com o banco de dados, siga as etapas abaixo:

1. Abra o arquivo `src/main/resources/application.properties`.
2. Para o ambiente de desenvolvimento, certifique-se de que as seguintes linhas estejam descomentadas:
3. `spring.datasource.url=jdbc:h2:mem:testdb`
4. `spring.datasource.username=sa`
5. `spring.datasource.password=`
6. Para o ambiente de produção com PostgreSQL, certifique-se de que as seguintes linhas estejam descomentadas:
7. `spring.datasource.url=jdbc:postgresql://localhost:5432/nome_do_banco`
8. `spring.datasource.username=seu_usuario`
9. `spring.datasource.password=sua_senha`

Substitua `nome_do_banco`, `seu_usuario` e `sua_senha` pelas informações corretas de configuração do seu banco de dados PostgreSQL.

### Executando a Aplicação

1. Abra o terminal na pasta raiz do projeto.
2. Execute o seguinte comando para construir o projeto e executar os testes:
4. `mvn clean install`
3. Em seguida, execute o comando abaixo para iniciar a aplicação:
5. `mvn spring-boot:run`

A aplicação backend será executada na porta padrão 8080.

#### Projeto feito no INTENSIVÃO JAVA SPRING  do Nélio Alves.



