# Bem vindo ao repositório do projeto Js Unit Tests

## Comentários
Foram desenvolvidos testes e funções, todos testes utilizam o módulo Jest do NodeJs, e foi utilizado o ES Lint para avaliar o código.

---

## Instalação do projeto localmente:

1. No terminal, em um diretório de sua escolha, clonar o repositório:

```
git clone git@github.com:lucas-da-silva/js-unit-tests.git
```

2. Dentro do reposítorio, existe o diretório tests que contem os testes, e no diretório src estão as funções que são testadas. :rocket:
  - Está especificado nos requisitos quais testes e funções eu fiz, ou que foram criadas pelas Trybe; 

--- 

## Requisitos

### 1. Implemente a função `average`

<details>
  <summary>A função average recebe um array de tamanho variável e retorna a média dos valores recebidos. Caso a função receba algum valor não numérico ou um array vazio, o valor `undefined` deve ser retornado.</summary><br/> 
  
  Todos os resultados devem ser arredondados para valores inteiros. Ex: 4,6 vira 5; 1,3 vira 1. O arquivo `average.spec.js` contém os testes para `average` já implementados. Implemente a função no arquivo `src/average.js` de forma que ela atenda aos testes propostos.

</details>

---

### 2. Implemente os casos de teste para a função `numbers`

<details>
  <summary>A função `numbers` recebe um array de tamanho variável e retorna `true` se todos os parâmetros forem do tipo 'number' e `false` caso contrário.</summary><br/> 
  
  Essa função já está implementada no arquivo `src/numbers.js`. Escreva pelo menos quatro testes para essa função para garantir que a implementação de `numbers` está correta.

</details>

---

### 3. Implemente a função `vqv`

<details>
  <summary>Use template literals para escrever uma função que recebe o seu nome e a sua idade e retorna o parágrafo descrito abaixo:</summary><br/>

  ```javascript
  `Oi, meu nome é Tunico!
  Tenho 30 anos,
  trabalho na Trybe e mando muito em programação!
  #VQV!`
  ```

  Caso a função seja chamada sem nenhum parâmetro, o valor `undefined` deve ser retornado. O arquivo `vqv.spec.js` contém os testes para `vqv` já implementados. Implemente a função no arquivo `src/vqv.js` de forma que ela atenda aos testes propostos.

</details>

---

### 4. Implemente os casos de teste para a função `circle`

<details>

  <summary>A função `circle` recebe o raio de um círculo e retorna um objeto contendo as suas informações: Raio, Área e Circunferência. Se não for especificado um raio, a função retorna `undefined`.</summary></br>
  
  Essa função já está implementada no arquivo `src/circle.js`. Escreva pelo menos seis testes para essa função para garantir que a implementação de `circle` está correta.

</details>

---

### 5. Implemente a função `createStudent`

<details>
<summary>A função `createStudent` recebe como parâmetro um **nome**, e retorna um objeto contendo duas chaves:</summary></br>

  1. **name**, contendo o nome passado como parâmetro;
  2. **feedback**, contendo uma função que retorna a frase 'Eita pessoa boa!' ao ser chamada.

  O arquivo `createStudent.spec.js` contém os testes para `createStudent` já implementados. Implemente a função no arquivo `src/createStudent.js` de forma que ela atenda aos testes propostos.

</details>

---

### 6. Implemente os casos de teste para a função `productDetails`

<details>
  <summary>A função `productDetails` recebe duas strings que representam nomes de produtos, e retorna um array contendo dois objetos com os detalhes dos respectivos produtos:</summary></br>

  ```javascript
  productDetails('Alcool gel', 'Máscara');
  ```

  **Retorna:**

  ```js
  [
    {
      name: 'Alcool gel'
      details: {
        productId: 'Alcool gel123'
      }
    },
    {
      name: 'Máscara'
      details: {
        productId: 'Máscara123'
      }
    }
  ]
  ```

  Essa função já está implementada no arquivo `src/productDetails.js`. Escreva pelo menos cinco testes para essa função no arquivo `tests/productDetails.js` para garantir que a implementação de `productDetails` está correta.

</details>

---

### 7. Implemente as funções `calculator` e `arrayGenerator`

<details>
  <summary>A função `calculator` recebe dois números inteiros como parâmetro e retorna um objeto com as seguintes chaves:</summary></br>
  - sum;
  - mult;
  - div;
  - sub.

  Para cada chave atribua como valor a operação correspondente à sua chave:
  - `sum:` retorna o resultado da soma dos dois números;
  - `mult:` retorna o resultado da multiplicação dos dois números;
  - `div:` retorna o resultado da divisão dos dois números;
  - `sub:` retorna o resultado da subtração dos dois números.

  Os resultados das divisões devem sempre ser arredondados para baixo.

  Parâmetros:
  - Dois números inteiros.

  Comportamento:
  ```javascript
  calculator(1, 2); // { sum: 3, mult: 2, div: 0, sub: -1 }
  ```

  Já a função `arrayGenerator` converte objetos em arrays, de chaves, valores ou ambos. Ela deve receber dois parâmetros:

  - o primeiro parâmetro deve ser uma string que indica o tipo de conversão;
  - o segundo parâmetro deve ser um objeto semelhante ao que é retornado pela função calculator que você acabou de desenvolver.

  Parâmetros:
  - Uma string que indica o tipo de conversão;
  - Um objeto no formato { sum: 3, mult: 2, div: 0, sub: -1 };

  Comportamento:
  ```javascript
  arrayGenerator('keys', { sum: 3, mult: 2, div: 1, sub: 0 }) // [ 'sum', 'mult', 'div', 'sub' ]
  arrayGenerator('values', { sum: 3, mult: 2, div: 1, sub: 0 }) // [ 3, 2, 1, 0 ]
  arrayGenerator('entries', { sum: 3, mult: 2, div: 1, sub: 0 }) // [ [ 'sum', 3 ], [ 'mult', 2 ], [ 'div', 1 ], [ 'sub', 0 ] ]
  ```
  O arquivo `objPlayground.spec.js` contém os testes para `calculator` e `arrayGenerator` já implementados. Implemente as funções no arquivo `src/objPlayground.js` de forma que ela atenda aos testes propostos.

</details>

---

### 8. Implemente a função `myCounter`

<details>
  <summary>A função myCounter possui dois loops aninhados que inserem valores dentro de um array. Como podemos perceber, eles vão adicionando valores ao array até sua condição de parada.</summary></br>

   Corrija a função `myCounter`, sem eliminar nenhum dos loops de repetição, para que a função retorne o array correto. O arquivo `myCounter.spec.js` contém os testes para `myCounter` já implementados. Implemente a função no arquivo `src/myCounter.js` de forma que ela atenda aos testes propostos.

</details>

---

### 9. Implemente os casos de teste para a função `getCharacter`

<details>

  <summary>A função `getCharacter` recebe uma string que representa o nome de uma personagem e retorna um objeto contendo o seu nome, a sua classe e as suas frases.</summary></br>

  ```javascript
  getCharacter('Arya');
  ```

  **Retorna:**

  ```javascript
  {
    name: 'Arya Stark',
    class: 'Rogue',
    phrases: ['Not today', 'A girl has no name.']
  }
  ```

  Essa função já está implementada no arquivo `src/getCharacter.js`. Escreva pelo menos seis testes para essa função no arquivo `tests/getCharacter.spec.js` para garantir que a implementação de `getCharacter` está correta.

</details>

---

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
