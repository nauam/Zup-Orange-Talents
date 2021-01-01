
# Desafio Orange Talents

<p align="center">
  <img src="https://img.shields.io/static/v1?label=java&message=15&color=blue&style=for-the-badge&logo=java"/> <img src="https://img.shields.io/static/v1?label=maven&message=4.0.0&color=red&style=for-the-badge&logo=apache"/> <img src="http://img.shields.io/static/v1?label=spring-boot&message=2.4.1&color=red&style=for-the-badge&logo=spring"/>
</p>
<p align="center">
<img src="http://img.shields.io/static/v1?label=STATUS&message=CONCLUIDO&color=green&style=for-the-badge"/> <img src="http://img.shields.io/static/v1?label=License&message=MIT&color=green&style=for-the-badge"/>
</p>

### Tópicos 
:small_blue_diamond: [Descrição do projeto](#descrição-do-projeto)
:small_blue_diamond: [Funcionalidades](#funcionalidades)
:small_blue_diamond: [Pré-requisitos](#pré-requisitos)
:small_blue_diamond: [Dependências](#dependências)
:small_blue_diamond: [Como rodar a aplicação](#como-rodar-a-aplicação-arrow_forward)

## Descrição do projeto 

<p align="justify">
   API REST para um processo de abertura de nova conta no banco. As informações obrigatórias são: Nome, E-mail, CPF e Data de nascimento. 
</p>

## Funcionalidades

:heavy_check_mark: Metodo POST: Envio dos parâmetros,
:heavy_check_mark: Validação: Todos os parâmetros estão preencidos,
:heavy_check_mark: Validação: Nome tem mais de 5 caracteres e menos que 120 caracteres,
:heavy_check_mark: Validação e duplicação: E-mail e CPF.

## Pré-requisitos
:warning: [JDK 15](https://www.oracle.com/br/java/technologies/javase-downloads.html)
:warning: [Apache Maven](https://maven.apache.org/download.cgi)
:warning: [Spring Tool Suite 4](https://spring.io/tools)
:warning: [Postman](https://www.postman.com/downloads/)
:warning: [Xampp](https://www.apachefriends.org/pt_br/index.html)

## Dependências
:wrench: H2 Database
:wrench: Spring Boot DevTools 
:wrench: Spring Data JPA
:wrench: Spring Web
:wrench: Validation

## Como rodar a aplicação :arrow_forward:

No terminal, clone o projeto:
```
git clone https://github.com/nauam/Zup-Orange-Talents.git
```
Abra o **Spring Tool Suite 4**, para importar o projeto, faça: *File>Import...>Existing Maven Projects>Next>Browse *(Selecione o camino do projeto)*>Finish*, a partir disso, irá carregar todas as dependencias.

No arquivo **ContaApplication.java**, clique com o *botão direto do mouse>Run As>Spring Boot App*, isso rodará o projeto.

Abra o **Postman**, selecione *POST* em 

	localhost:8080/contas

No **Body**, selecione *JSON (application/json)* , escreva os dados a serem castrados na abertura da nova conta no banco,
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