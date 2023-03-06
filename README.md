# Boas-vindas ao repositório do projeto ES6 e Testes Unitários!

  - Escrever testes unitários utilizando o módulo Jest do NodeJS para verificar o correto funcionamento das funções;
  - Escrever funções de forma que elas atendam a testes já implementados;
  - Escrever testes e funções utilizando uma abordagem de desenvolvimento orientado a testes.
 
 ---
![Badge em Desenvolvimento](http://img.shields.io/static/v1?label=STATUS&message=CONCLUIDO&color=GREEN&style=for-the-badge)

---

## ✔️ Técnicas e tecnologias utilizadas

- ``ES6``
- ``Testes Unitários``

---
# Orientações

<details>
  <summary><strong>📝 ES6 e Testes Unitários</strong></summary><br />

  Este repositório contém um template de uma aplicação NodeJS (observe a existência do arquivo package.json). Após clonar o projeto e instalar as dependências através do `npm install`, você não precisará realizar nenhuma configuração adicional. Todos os arquivos estritamente necessários para finalizar o projeto já estão criados, não sendo necessária a criação de outros arquivos. Você deverá completar as funções e testes unitários de forma a satisfazer os requisitos listados na seção **Requisitos do projeto**.

  As funções a serem implementadas estão dentro da pasta `src` e seus respectivos testes estão na pasta `tests`. O nome dos arquivos também segue uma ordem definida. Basicamente, os arquivos de teste possuem o nome do arquivo alvo (arquivo da funcionalidade) acrescido do nome `.spec.js`.

  Há um arquivo como `src/exemplo.js` que contém a implementação de uma função e um arquivo como `tests/exemplo.spec.js` com os testes unitários referentes à função presente no arquivo `src/exemplo.js`.

  Cada função possui um bloco de comentários em suas primeiras linhas explicando qual é o trabalho que a função deve realizar.

</details>

# Passo a Passo

---
### 1. Implemente a função `average`

### 2. Implemente os casos de teste para a função `numbers`

### 3. Implemente a função `vqv`

### 4. Implemente os casos de teste para a função `circle`

### 5. Implemente a função `createStudent`

### 6. Implemente os casos de teste para a função `productDetails`

### 7. Implemente as funções `calculator` e `arrayGenerator`

### 8. Implemente a função `myCounter`

### 9. Implemente os casos de teste para a função `getCharacter`

### 10. Implemente a função `createMenu`, bem como seus casos de teste

<details>
  <summary>Esse último requisito vai guiar você por um rico processo de Desenvolvimento Orientado a Testes ou TDD - Test Driven Development</summary></br>

  Imagine a seguinte situação: você é responsável por escrever o código do sistema de pedidos de um restaurante através do qual será possível cadastrar um menu. Dado que um menu foi cadastrado, o sistema deve disponibilizar um objeto que permite:

  - Ler o menu cadastrado;
  - Fazer pedidos;
  - Verificar o que foi pedido;
  - Somar o valor da conta.

  A estrutura deste código e deste objeto já está definida e você precisa implementá-la. Você encontrará mais detalhes sobre a estrutura a ser seguida e exemplos do retorno da função no arquivo `src/restaurant.js`. 
  Você deverá se orientar através dos tópicos abaixo para garantir o bom desenvolvimento do sistema.

  **IMPORTANTE - BOAS PRÁTICAS TDD: COMECE PELO TESTE 1 DO ARQUIVO `tests/restaurant.spec.js`** 

  Se surgirem dúvidas, não deixe de consultar o nosso conteúdo sobre [TDD](https://app.betrybe.com/course/fundamentals/introducao-a-javascript-es6-e-testes-unitarios/primeiros-passos-em-jest/eb321d06-e126-4c84-8d7e-6134973bf081/conteudos/b02b5214-5797-436a-9c3f-aa9344361bd9/testando-em-pequenos-passos/d33319dc-ee06-4e09-97d6-4db1ac440e25?use_case=side_bar).

  1. No arquivo `tests/restaurant.spec.js`, escreva um teste que verifica se a função `createMenu()` retorna um objeto que possui a chave `fetchMenu`, a qual tem como valor uma função.

  2. No arquivo `tests/restaurant.spec.js`, escreva um teste que verifica se `'objetoRetornado.fetchMenu()'` retorna um objeto cujas chaves são somente `food` e `drink`, considerando que a função `createMenu()` foi chamada com o objeto: `{ food: {}, drink: {} }`.

  3. No arquivo `tests/restaurant.spec.js`, escreva um teste que verifica se o menu passado pra função `createMenu()` é idêntico ao menu recuperado pela função `'objetoRetornado.fetchMenu()'`.

  4. No arquivo `src/restaurant.js`, crie uma função `createMenu()` que, recebendo um objeto como parâmetro, retorna esse objeto com o seguinte formato: { fetchMenu: () => objetoPassadoPorParametro }.

  5. No arquivo `tests/restaurant.spec.js`, escreva um teste que verifica se `'objetoRetornado.consumption'`, após a criação do menu, retorna um array vazio.

  6. No arquivo `src/restaurant.js`, adicione ao objeto retornado por `createMenu()` uma chave `consumption` que, como valor inicial, tem um array vazio.

  7. No arquivo `tests/restaurant.spec.js`, escreva um teste que verifica se ao chamar uma função associada à chave `order` no objeto retornado, passando uma string como parâmetro (como `objetoRetornado.order('coxinha')`), tal string é adicionada ao array retornado em `objetoRetornado.consumption`.

  8. No arquivo `src/restaurant.js`, crie uma função, separada da função `createMenu()`, que, ao receber uma string como parâmetro, adiciona essa string ao array de `objetoRetornado.consumption`. Essa nova função será adicionada à chave `order`.

  9. No arquivo `tests/restaurant.spec.js`, escreva um teste que verifica se ao adicionar três pedidos, dentre bebidas e comidas, o array `objetoRetornado.consumption` contém os itens pedidos.

  10. No arquivo `tests/restaurant.spec.js`, escreva um teste que verifica se a função `order` aceita que pedidos repetidos sejam acrescidos a `consumption`.

  11. No arquivo `tests/restaurant.spec.js`, escreva um teste que verifica que, ao chamar `objetoRetornado.pay()`, retorna-se a soma dos preços de tudo que foi pedido, conforme registrado em `objetoRetornado.consumption`.

  12. No arquivo `src/restaurant.js`, adicione ao objeto retornado por `createMenu()` uma chave `pay` com uma função que percorre por todos os itens de `objetoRetornado.consumption`, soma o preço deles e retorna o valor somado acrescido de 10%. DICA: para isso, você precisará percorrer tanto o objeto da chave `food` quanto o objeto da chave `drink`.

</details>
