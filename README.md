
# ⚙️ Backend CRUD Produtos (Spring Boot)

Esta é a API RESTful responsável pelo gerenciamento de produtos da aplicação. Desenvolvida com **Java** e **Spring Boot**, a aplicação fornece todos os recursos necessários para persistência de dados, validações de negócio e integração com banco de dados relacional.

## 🚀 Tecnologias Utilizadas

* **Java 17+**: Linguagem de programação estável e performática.
* **Spring Boot 3.x**: Framework para criação de microserviços e APIs.
* **Spring Data JPA**: Para mapeamento objeto-relacional (ORM) e abstração de consultas.
* **Database (H2/MySQL/PostgreSQL)**: Persistência de dados confiável.
* **Maven**: Gestão de dependências e automação de build.
* **Bean Validation (Hibernate Validator)**: Garantia de integridade dos dados recebidos.
* **Lombok**: Para um código mais limpo e produtivo.

## 🛠️ Funcionalidades da API

A API segue os padrões REST e disponibiliza os seguintes recursos:

| Método | Endpoint          | Descrição                         |
| :----- | :---------------- | :-------------------------------- |
| **POST** | `/api/produtos`     | Cadastra um novo produto          |
| **GET** | `/api/produtos`     | Lista todos os produtos           |
| **GET** | `/api/produtos/{id}`| Detalhes de um produto específico |
| **PUT** | `/api/produtos/{id}`| Atualiza os dados de um produto   |
| **DELETE** | `/api/produtos/{id}`| Remove um produto do estoque      |

## 📂 Estrutura do Projeto

A organização segue o padrão de camadas para facilitar testes e manutenção:

backend-crud-produtos-springboot/
├── src/main/java/com/mvdevelop/crud/
│   ├── controller/    # Camada de exposição dos recursos REST
│   ├── service/       # Camada de regras de negócio
│   ├── repository/    # Interface de comunicação com o banco de dados
│   ├── model/         # Entidades JPA (Produtos, Categorias)
│   └── dto/           # Data Transfer Objects (Payloads de entrada/saída)
└── src/main/resources/
    └── application.properties # Configurações do banco e servidor
🔧 Configuração e Execução
Pré-requisitos
JDK 17+ instalado.

Maven instalado.

Passo a Passo
Clone o repositório:

Bash

git clone [https://github.com/mvdevelop/backend-crud-produtos-springboot.git](https://github.com/mvdevelop/backend-crud-produtos-springboot.git)
cd backend-crud-produtos-springboot
Configure o banco de dados: Verifique o arquivo src/main/resources/application.properties para garantir que as credenciais do banco estejam corretas.

Inicie a aplicação:

Bash

mvn spring-boot:run
A API estará disponível em http://localhost:8080.

## 👨‍💻 Autor
Desenvolvido por mvdevelop.

GitHub: @mvdevelop

## 📄 Licença
Este projeto está sob a licença MIT.
