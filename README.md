# Desafio Orange Talents

<p align="center">
  <img src="https://img.shields.io/static/v1?label=java&message=15&color=blue&style=for-the-badge&logo=java"/> <img src="https://img.shields.io/static/v1?label=maven&message=4.0.0&color=red&style=for-the-badge&logo=apache"/> <img src="http://img.shields.io/static/v1?label=spring-boot&message=2.4.1&color=red&style=for-the-badge&logo=spring"/>

<img src="http://img.shields.io/static/v1?label=STATUS&message=CONCLUIDO&color=green&style=for-the-badge"/> <img src="http://img.shields.io/static/v1?label=License&message=MIT&color=green&style=for-the-badge"/>
</p>

### Tópicos 

:fa-chevron-right: [Descrição do projeto](#descrição-do-projeto)

:fa-chevron-right: [Funcionalidades](#funcionalidades)

:fa-chevron-right: [Pré-requisitos](#pré-requisitos)

:fa-chevron-right: [Como rodar a aplicação](#como-rodar-a-aplicação-arrow_forward)

## Descrição do projeto 

<p align="justify">
   API REST para um processo de abertura de nova conta no banco. As informações obrigatórias são: Nome, E-mail, CPF e Data de nascimento. A API devolve um resposta adequada para o caso de falha de validação e duplicação.
</p>

## Funcionalidades

:fa-check: Metodo POST: Envio dos parâmetros,

:fa-check: Validação: Todos os parâmetros estão preencidos,

:fa-check: Validação: Nome tem mais de 5 caracteres e menos que 120 caracteres,

:fa-check: Validação e duplicação: E-mail e CPF.

## Pré-requisitos
:fa-arrow-down: [JDK 15](https://www.oracle.com/br/java/technologies/javase-downloads.html)
:fa-arrow-down: [Apache Maven](https://maven.apache.org/download.cgi)
:fa-arrow-down: [Spring Tool Suite 4](https://spring.io/tools)
:fa-arrow-down: [Postman](https://www.postman.com/downloads/)
:fa-arrow-down: [Xampp](https://www.apachefriends.org/pt_br/index.html)

## Dependências
:fa-wrench: H2 Database
:fa-wrench: Spring Boot DevTools 
:fa-wrench: Spring Data JPA
:fa-wrench: Spring Web
:fa-wrench: Validation

## Como rodar a aplicação :fa-cogs:

No terminal, clone o projeto:
```
git clone https://github.com/nauam/Zup-Orange-Talents.git
```
Abra o **Spring Tool Suite 4**, para importar o projeto, faça: *File>Import...>Existing Maven Projects>Next>Browse *(Selecione o camino do projeto)*>Finish*, a partir disso, irá carregar todas as dependencias.

No arquivo **ContaApplication.java**, clique com o *botão direto do mouse>Run As>Spring Boot App*, isso rodará o projeto.

Abra o **Postman**, selecione *POST* em 

	localhost:8080/contas

No **Body**, selecione *JSON (application/json)* , escreva os dados a serem castrados na abertura da nova conta no banco,

####Json

```json
{
	"nome" : "Maria de Nazaré Esteves Tedesco",
	"email" : "nazare.tedesco@outlook.com",
	"cpf": "10131949004",
	"dataNascimento": "24/08/1968"
}
```
 e envie (**Send**).

## Licença 

The [MIT License]() (MIT)

Copyright &copy;  2021 - Desafio Orange Talents (Nauam)