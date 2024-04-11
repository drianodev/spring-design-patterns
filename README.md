# Projeto Spring Design Patterns

Este repositório contém um exemplo de aplicação Spring Boot que demonstra o uso de padrões de projeto para construir uma API RESTful para gerenciamento de clientes e endereços.

## Tecnologias Utilizadas

- Java 17
- Spring Boot 3.2.4
- Spring Data JPA
- Spring Web
- Spring Cloud OpenFeign
- H2 Database (em ambiente de execução)
- SpringDoc OpenAPI (Swagger)

## Estrutura do Projeto

O projeto está estruturado da seguinte forma:

- **src/main/java/br.com.drianodev.springdesignpatterns**: Contém os pacotes Java da aplicação.
    - **controller**: Contém os controladores REST da API.
    - **entity**: Contém as entidades JPA.
    - **repository**: Contém as interfaces de repositório JPA.
    - **service**: Contém as interfaces e implementações dos serviços da aplicação.
- **src/main/resources**: Contém arquivos de configuração e recursos da aplicação.
    - **application.properties**: Arquivo de configuração do Spring Boot.
- **pom.xml**: Arquivo de configuração do Maven.

## Executando a Aplicação

Para executar a aplicação, siga estas etapas:

1. Certifique-se de ter o Java 17 e o Maven instalados em sua máquina.
2. Clone este repositório para o seu ambiente local.
3. Navegue até o diretório raiz do projeto e execute o seguinte comando no terminal:

   ```
   mvn spring-boot:run
   ```

4. A aplicação será iniciada e estará disponível em `http://localhost:8080`.

## Documentação da API

A documentação da API está disponível utilizando o Swagger UI. Após iniciar a aplicação, acesse `http://localhost:8080/swagger-ui.html` para visualizar e interagir com a documentação da API.

## Funcionalidades Principais

- **Cadastro de Cliente**: Permite cadastrar novos clientes fornecendo os dados necessários, incluindo o endereço do cliente.
- **Atualização de Cliente**: Permite atualizar os dados de um cliente existente.
- **Exclusão de Cliente**: Permite excluir um cliente existente.
- **Consulta de Todos os Clientes**: Retorna uma lista com todos os clientes cadastrados.
- **Consulta de Cliente por ID**: Retorna os detalhes de um cliente específico com base no ID fornecido.