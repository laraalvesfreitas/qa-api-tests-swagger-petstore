# Testes de API - Swagger Petstore

## Sobre o projeto

Este repositório apresenta a execução de testes de API utilizando a Swagger Petstore, com foco na funcionalidade **Pet**.

Foram realizados testes funcionais cobrindo o fluxo completo de **CRUD (Create, Read, Update, Delete)**, incluindo cenários positivos e negativos, com validação de:

- Status codes
- Estrutura de resposta
- Tipos de dados
- Regras de negócio da API

Os testes foram executados utilizando o Postman, com documentação de evidências e organização dos cenários para garantir **rastreabilidade e reprodutibilidade**.

---

## Objetivo

Demonstrar habilidades práticas em:

- Testes de API REST
- Criação de casos de teste
- Identificação e documentação de bugs
- Análise crítica de comportamento da API

---

## Escopo dos testes

Os testes foram realizados no endpoint `/pet`, contemplando:

- Criação de pet (POST)
- Consulta de pet por ID (GET)
- Atualização de pet (PUT)
- Exclusão de pet (DELETE)
- Upload de imagem

---

## Tipos de testes executados

- Testes positivos (fluxo esperado)
- Testes negativos (validação de erros)
- Testes de validação de tipos de dados
- Testes exploratórios

---

## Bugs identificados

Durante os testes, foram identificadas inconsistências importantes na API:

- API permite criação de pet sem campos obrigatórios
- API retorna erro **500** ao receber tipo inválido
- API expõe erro interno (`NumberFormatException`) ao receber dados inválidos

*Detalhes disponíveis na pasta `/bugs`*

---

##  Estrutura do repositório

`/casos-de-teste → Casos de teste documentados`

`/bugs → Relatos de bugs encontrados`

`/evidencias → Prints das execuções`


---

## Ferramentas utilizadas

- Postman
- Swagger Petstore

---

## Observações

- A API apresenta comportamento permissivo, aceitando dados inválidos em alguns cenários.
- Foram identificadas inconsistências entre a documentação e o comportamento real da API.
- A API pode retornar campos adicionais com valores padrão mesmo quando não enviados no request.

---

## Conclusão

Este projeto demonstra a aplicação prática de testes de API, com foco em análise crítica, identificação de falhas e documentação estruturada, simulando um cenário real de atuação em Quality Assurance.



*Obs: Foi utilizada inteligência artificial como apoio na revisão gramatical e formatação do conteúdo.*
