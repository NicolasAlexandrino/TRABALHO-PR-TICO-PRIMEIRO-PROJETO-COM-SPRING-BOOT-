# API de Cadastro de Produtos

**Autor:** Nicolas Alexandrino
**Professor:** Anderson Soares
**Disciplina:** Desenvolvimento Back-End com Java

## Descrição
Este é o meu primeiro projeto utilizando Spring Boot, construído para o trabalho prático da disciplina de Desenvolvimento Back-End com Java. Trata-se de uma API REST simples para gerenciar o cadastro e a consulta de produtos. 

A aplicação foi organizada em camadas (Model, Repository, Service e Controller) e utiliza uma lista em memória para armazenar os dados temporariamente, sem a necessidade de um banco de dados externo.

## Tecnologias utilizadas
* Java
* Spring Boot
* Maven

## Como executar
1. Certifique-se de ter o Java e uma IDE (como VS Code, IntelliJ ou Eclipse) instalados em sua máquina.
2. Clone este repositório em seu computador.
3. Abra a pasta do projeto na sua IDE.
4. Aguarde o Maven baixar as dependências do projeto automaticamente.
5. Execute a classe principal `ProjetoApplication.java`.
6. O servidor irá iniciar na porta 8080. A API estará acessível em `http://localhost:8080`.

## Endpoints

* **GET /produtos** 
  Retorna a lista de todos os produtos cadastrados. Pode ser testado diretamente abrindo a URL `http://localhost:8080/produtos` no navegador.

* **POST /produtos**
  Cadastra um novo produto na lista. Requer o envio de um corpo (body) no formato JSON, como no exemplo abaixo:
  
  ```json
  {
    "nome": "Monitor Gamer",
    "preco": 1200.00
  }
