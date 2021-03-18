## Índice

- [Índice](#índice)
- [Fundamentos de Node](#fundamentos-de-node)
- [Funcionamento do Node](#funcionamento-do-node)
- [Problemas que o Node resolve](#problemas-que-o-node-resolve)
- [Conceitos de API](#conceitos-de-api)
- [REST](#rest)
- [Métodos HTTP](#métodos-http)
- [Status Code](#status-code)
- [Tipos de Parâmetros](#tipos-de-parâmetros)
- [Boa práticas de API](#boa-práticas-de-api)

## Fundamentos de Node
Plataforma opensource que permite a execução javascript do lado do servidor.

## Funcionamento do Node
Composto da V8(google) interpretador javascript + libuv(multiplataforma com foco)
em I/O assíncrono + módulos nativos.

Arquitetura Event Loop
-Call Stack
-Single Thread
-Non Block I/O
-Módulos nativos(http, filesystem, buffer,dns)

A lista de funções na call stack, o event loop ouve essas funções, uma por requisição
por vez, encaminha para uma thread disponível e assim sucessivamente. Possuí quatro threads
disponives, sendo porssivel adaptar para mais theads. Por ser uma fila, o que entra por ultimo é o que sai primeiro.

O Node possui gerenciadores de pacotes (npm e yarn) para gerenciar as bibliotecas a
serem utilizadas nos projetos e também podemos criar nossas proprias bibliotecas
para disponibilizar para a comunidade.

Existem frameworks para se trabalhar com o Node a exemplo:
express, adonis, nest, etc ...

## Problemas que o Node resolve
Criado por Ryan Dahl ao observar a barra de progresso do Flicker.
As tecnologias não davam bom suporte para o processo de I/O. Assim era necessário 
uma linguagem para resolver o problema das requisições da barra de progresso do Flicker.

## Conceitos de API
Interface de programação de aplicativos, conjunto de especificações de possíveis
interações entre aplicações, determina como uma aplicação irá se comunicar com
a outra.

## REST
Representation State Transfer.Modelo de arquitetura. Possui regras para que seja definido a arquitetura REST: Client-Server, Stateless, Cache, Inteface Uniforme,Camadas,Código sob Demanda 

## Métodos HTTP

GET - leitura
POST - criação
PUT - atualização
PATCH - atualização parcial
DELETE - deletar

## Status Code
1XX - Informativo - a solicitação foi aceita ou o processo continua em andamento 
2XX - Confirmação
 - 200 - requisição bem sucedida
 - 201 - Created - usado em POST apos uma criação
3XX - Redirecionamento
 - 301 - Moved Permanetly
 - 302 - Moved
4XX - Erro do Cliente
 - 400 - Bad Request
 - 401 - Unauthorized
 - 403 - Forbidden
 - 404 - Not Found
 - 422 - Unprocessable Entity
5XX - Erro Servidor - servidor falhou ao concluir a solicitação
 - 500 - Internal Server Error
 - 502 - Bad Gateway
 -   
## Tipos de Parâmetros
- Header Params - token, controle de sessão ...
- Query Params - inseridos ao final da url: definidos por chave valor com delimitador  de separação &.
- Route Params - inseridos no meio da rota: buscas, alteração.
- Body Params - inseridos no corpo da requisição.


## Boa práticas de API
- Utilizar corretamento os metodos HTTP
- Utilização correta do status no retorno das repostas
- Padrão de nomenclatura
- 