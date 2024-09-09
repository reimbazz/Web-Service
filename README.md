# Projeto: Estudo de Spring Boot e JPA

## Descrição
Este é um projeto pessoal desenvolvido por **Pedro Reimberg de Oliveira** para aprimorar meus conhecimentos em **Spring Boot** e **JPA (Java Persistence API)**. O projeto consiste em uma aplicação simples de CRUD (Create, Read, Update, Delete), conectada a um banco de dados, com foco na implementação de **padrões de desenvolvimento** e **boas práticas** ao utilizar essas tecnologias.

## Funcionalidades
- **CRUD completo**: Implementação das operações básicas de cadastro, consulta, atualização e exclusão de registros.
- **Uso do Spring Boot** para configuração automática e simplificada da aplicação.
- **Persistência de dados com JPA/Hibernate**, utilizando um banco de dados relacional.
- **Uso de Repositories e Services**: Estrutura de camadas para garantir a separação de responsabilidades.
- **Tratamento de exceções**: Gerenciamento centralizado de exceções e erros na API.
- **Documentação com Swagger**: Interface amigável para testar os endpoints diretamente pelo navegador.

## Estrutura do Projeto
- **src/main/java/com/seuusuario/projectname**: Código-fonte do projeto.
  - **controller**: Controladores REST responsáveis por receber as requisições HTTP e direcioná-las para a camada de serviço.
  - **service**: Implementação da lógica de negócio e manipulação de dados.
  - **repository**: Interface JPA Repository que facilita a interação com o banco de dados.
  - **model**: Classes que representam as entidades do banco de dados.
  - **exception**: Tratamento de exceções específicas da aplicação.
  
## Como Executar
1. Clone o repositório para sua máquina local:
   ```bash
   git clone https://github.com/reimbazz/Web-Service.git
   ```
2. Configure o banco de dados:
   - Certifique-se de que o banco de dados está em execução e acessível.
   - Atualize o arquivo `application.properties` com as credenciais e configurações do banco de dados.
   
   Exemplo de `application.properties`:
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/seu-banco-de-dados
   spring.datasource.username=seu-usuario
   spring.datasource.password=sua-senha
   spring.jpa.hibernate.ddl-auto=update
   ```

3. Execute o projeto via Maven ou IDE (IntelliJ, Eclipse, etc.):
   - Pelo terminal:
     ```bash
     ./mvnw spring-boot:run
     ```
   - Ou pela IDE, execute a classe principal `CourseApplication.java`.

4. Acesse a aplicação:
   - A aplicação estará disponível em `http://localhost:8080`.
   - Para acessar a documentação Swagger, acesse `http://localhost:8080/swagger-ui.html`.

## Tecnologias Utilizadas
- **Spring Boot**: Framework utilizado para simplificar o desenvolvimento de aplicações Java com configuração mínima.
- **JPA/Hibernate**: API de persistência de dados que facilita a manipulação de bancos de dados relacionais.
- **MySQL**: Banco de dados utilizado para armazenar os dados da aplicação.
- **Maven**: Ferramenta de gerenciamento de dependências e build.
- **Swagger**: Utilizado para a documentação e teste de endpoints da API.

## Aprendizados
Durante o desenvolvimento deste projeto, aprimorei meus conhecimentos em:
- **Spring Boot**: Configuração e estruturação de uma aplicação moderna usando padrões do framework.
- **JPA/Hibernate**: Mapeamento objeto-relacional, persistência de dados e relacionamento entre entidades.
- **Boas práticas de desenvolvimento**: Separação de camadas (Controller, Service, Repository) e uso de injeção de dependências.
- **Tratamento de Exceções**: Implementação de handlers globais para capturar e tratar exceções personalizadas.

## Contribuição
Contribuições são bem-vindas! Se tiver sugestões, melhorias ou correções, sinta-se à vontade para abrir issues e enviar pull requests.

## Contato
Para mais informações ou dúvidas sobre o projeto, você pode entrar em contato comigo através dos seguintes meios:
- **Email**: pedro.reimberg.oliveira@gmail.com
- **LinkedIn**: [Pedro Reimberg de Oliveira](https://www.linkedin.com/in/pedro-reimberg-de-oliveira-500615163/)