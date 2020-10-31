# Challenge: Node.js concepts

## In this challenge, an application was created to demonstrate what I have learned so far with nodejs.

TABLE OF CONTENTS
=======================

<!--ts-->
  * [Sobre](#Sobre)
  * [Como usar](#como-usar)
    * [Pre Requisitos](#pre-requisitos)
    * [Instalando dependencias](#instalando-dependencias)
    * [Features](#features)
  * [Testes](#testes)
  * [Tecnologias](#tecnologias)
  * [Autor](#autor)
<!--te-->

### Sobre 

  O desafio faz parte do bootcamp GoStack da @RocketSeat, nesse desafio temos que criar uma series de rotas que respeitem a regra de negocio solicitada na descrição do desafio.
  Ao realizar o desafio o mesmo tem que passar nos testes antes de ser enviado para ser avaliado com uma nota final, que vai de 0 a 10.
  No teste conta com 9 tarefas a serem concluidas e que precisam passar pelo teste com sucesso para obter uma boa nota no desafio.

### Como usar

  #### Pré-requisitos

  - [x] Ter o NODEJS instalado na máquina na versão 12 ou superior.
  - [x] Ter o Yarn ou NPM instalado em sua máquina.
  - [x] Saber utilizar o Terminal.
  - [x] Opcional ter o Insomnia ou algum outro aplicativo para testar rotas http.
  - [x] Editor de código ou IDE de sua preferencia.

  #### Instalando dependencias

  Para que você possa instalar as dependencias da API, você pode rodar em seu terminal o comando:

    $ yarn

    $ npm install


  #### Features

  - [x] POST /repositories: A rota deve receber title, url e techs dentro do corpo da requisição, sendo a URL o link para o github desse repositório. Ao cadastrar um novo projeto, ele deve ser armazenado dentro de um objeto no seguinte formato: { id: "uuid", title: 'Desafio Node.js', url: 'http://github.com/...', techs: ["Node.js", "..."], likes: 0 }; Certifique-se que o ID seja um UUID, e de sempre iniciar os likes como 0.

  - [x] GET /repositories: Rota que lista todos os repositórios;

  - [x] PUT /repositories/:id: A rota deve alterar apenas o title, a url e as techs do repositório que possua o id igual ao id presente nos parâmetros da rota;

  - [x] DELETE /repositories/:id: A rota deve deletar o repositório com o id presente nos parâmetros da rota;

  - [x] POST /repositories/:id/like: A rota deve aumentar o número de likes do repositório específico escolhido através do id presente nos parâmetros da rota, a cada chamada dessa rota, o número de likes deve ser aumentado em 1;

### Testes 

  ##### Específicação dos testes:

  - [x] should be able to create a new repository: Para que esse teste passe, sua aplicação deve permitir que um repositório seja criado, e retorne um json com o projeto criado.

  - [x] should be able to list the repositories: Para que esse teste passe, sua aplicação deve permitir que seja retornado um array com todos os repositórios que foram criados até o momento.

  - [x] should be able to update repository: Para que esse teste passe, sua aplicação deve permitir que sejam alterados apenas os campos url, title e techs.
    $ yarn

    $ 
  - [x] should not be able to update a repository that does not exist: Para que esse teste passe, você deve validar na sua rota de update se o id do repositório enviado pela url existe ou não. Caso não exista, retornar um erro com status 400.

  - [x] should not be able to update repository likes manually: Para que esse teste passe, você não deve permitir que sua rota de update altere diretamente os likes desse repositório, mantendo o mesmo número de likes que o repositório já possuia antes da atualização. Isso porque o único lugar que deve atualizar essa informação é a rota responsável por aumentar o número de likes.

  - [x] should be able to delete the repository: Para que esse teste passe, você deve permitir que a sua rota de delete exclua um projeto, e ao fazer a exclusão, ele retorne uma resposta vazia, com status 204.

  - [x] should not be able to delete a repository that does not exist: Para que esse teste passe, você deve validar na sua rota de delete se o id do repositório enviado pela url existe ou não. Caso não exista, retornar um erro com status 400.

  - [x] should be able to give a like to the repository: Para que esse teste passe, sua aplicação deve permitir que um repositório com o id informado possa receber likes. O valor de likes deve ser incrementado em 1 a cada requisição, e como resultado, retornar um json contendo o repositório com o número de likes atualizado.

  - [x] should not be able to like a repository that does not exist: Para que esse teste passe, você deve validar na sua rota de like se o id do repositório enviado pela url existe ou não. Caso não exista, retornar um erro com status 400.
  
  #### Rodando os testes em sua máquina:

  Para rodar os testes em sua máquina é preciso executar o script de testes com o seguinte comando em seu terminal:

    $ yarn test
     OU
    $ npm test

### Tecnologias

    NodeJS
    JavaScript
    Express


### Autor

  Formado no curso técnico em informática, amante de programação e técnologia.
  Estudando o bootcamp GoStack 14 da RockeSeat

  Linkedin ==> https://www.linkedin.com/in/carlos-faita/
  