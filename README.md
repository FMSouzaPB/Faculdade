# Faculdade
Sistema de Reserva de Hotel com Spring Boot

Descrição

Este projeto é um sistema simples de reserva de hotel desenvolvido com Spring Boot. Ele permite aos usuários listar hotéis, fazer reservas e gerenciar essas reservas. Este projeto foi criado como parte de uma tarefa de faculdade para demonstrar a utilização do Spring Boot.

Tecnologias Utilizadas

Spring Boot
Spring Data JPA
MySQL
Maven

Funcionalidades

Listagem de hotéis
Criação de novos hotéis
Criação de reservas
Listagem de todas as reservas

Como Executar

Pré-requisitos

JDK 11 ou superior
Maven
MySQL

Configuração do Banco de Dados

Crie um banco de dados no MySQL.
Atualize o arquivo src/main/resources/application.properties com suas credenciais de banco de dados.

spring.datasource.url=jdbc:mysql://localhost:3306/(Meu_Banco_de_dados)
spring.datasource.username=seu_usuario
spring.datasource.password=sua_senha

Executando a Aplicação

Clone o repositório para a sua máquina local.
Navegue até a pasta raiz do projeto através do terminal.
Execute o comando mvn spring-boot:run.
A aplicação estará disponível em http://localhost:8080.

Endpoints da API

Hotéis
GET /hotels: lista todos os hotéis.

POST /hotels: cria um novo hotel.

Exemplo de corpo da solicitação:

{
  "nome": "Nome do Hotel",
  "localizacao": "Localização do Hotel"
}


Reservas
GET /reservas: lista todas as reservas.

POST /reservas: cria uma nova reserva.

Exemplo de corpo da solicitação:

{
  "hotel": {
    "id": 1
  },
  "dataCheckIn": "2023-01-01",
  "dataCheckOut": "2023-01-05"
}

Autor

Francisco Maven De Souza Alves
