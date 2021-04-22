# Teste de Front-end 99Jobs
Este teste é apresentado aos candidatos as vagas de desenvolvimento Front-end para avaliar os quesitos técnicos.

### O Desafio

Seu objetivo é criar um simples app, com uma página de listagem de oportunidades e outra página com um formulário com os dados da vaga selecionada.

* Implementar o HTML/CSS da página de listagem conforme [layout].
* Fazer o site responsivo respeitando os Breakpoints.
* Buscar estado inicial da listagem através da Api.

### Pré-requisitos:

- Deve ser possível listar as oportunidades;
- Editar dados da oportunidade selecionada.
- Fazer a persistência dos dados no `localStorage` ou `IndexedDB`;

Para ter o estado inicial da lista de oportunidades utilizar este recurso abaixo:

> GET

### O que esperamos:

- A página ser responsiva;
- Padrão de Projeto e boas práticas;
- Permitir edição da oportunidade;
- Criar um passo a passo de como rodar sua aplicação [(Sugestão)](https://github.com/wearehive/project-guidelines/blob/master/README.sample.md);
- Criar uma breve descrição da solução utilizada.
- Não é permitido a utilização de nenhum framework ou o uso de qualquer biblioteca (exceto para testes unitário e tasks de build), recomendado uso de ECMAScript 6+;

### Plus:

- Testes unitários;;
- Uso de pré-processador css;
- Testes End to End;

 ** Use sua criatividade para criar a página para listar os dados cadastrados **
 
## Instalando API
 
A API sera rodada em [nodeJs](https://nodejs.org/en/), caso nao tenha instalado: 
 
```
sudo apt install nodejs
sudo apt install npm
```
 
Com o projeto baixado na maquina, abra a pasta da api em uma outra aba do terminal

```
cd ./teste-front-end/opportunity_server/
```

Instale a dependencia `serve`

```
npm i -g serve
```

Inicie a api

```
serve
```

Pronto! A api de oportundiades estará rodando na porta `5000`.

## API

Chamada:
> GET http://localhost:5000/opportunities.json

Retorno:
```
[
   {
      title: 'Exemplo 1',
      location: '23, Rua a',
      tags: [
         'tag 1',
         'tag 2',
         ...
      ],
      salary: '1000-1500',
      published_at: '2021-01-01'
   },
   ...
]
```
