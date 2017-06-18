# Aprenda React.js

## Introdução

[React.js - Website Oficial](https://facebook.github.io/react/)

[React.js - Documentação](https://facebook.github.io/react/docs/hello-world.html)

## Instalação



### npm packages

- Instala os package do React localmente no projeto

```shell
npm install --save react react-dom
```

- Instala o Babel.js (necessário para interpretar ES6 e JSX)

```shell
npm install --save-dev babel-cli babel-preset-env
```

### create-react-app

- Instala o pacote `create-react-app` globalmente

```shell
npm install -g create-react-app
```

- Exibe a versão do pacote `create-react-app` instalada

```shell
create-react-app --version
```

- Cria um projeto chamado `projeto-react`

```shell
create-react-app projeto-react
cd projeto-react
```

- Executa a aplicação em `http://localhost:3000`

```shell
npm start
```

- Executa os testes

```shell
npm test
```

- Compila a aplicação para produção

```shell
npm run build
```

## Exercício

1. Executar `npm start` na aplicação e visitar a página no navegador
1. Executar o script interativo `npm test`
1. Explore e conheça melhor a estrutura criada na pasta do projeto
1. Explore e conheça melhor o código dos arquivos criados
1. Leia mais sobre o pacote [`create-react-app no Github`](https://github.com/facebookincubator/create-react-app)

## Introdução a JSX

- [DOM Elements](https://facebook.github.io/react/docs/dom-elements.html)
- [Introducing JSX](https://facebook.github.io/react/docs/introducing-jsx.html)
- [React Components, Elements, and Instances](https://facebook.github.io/react/blog/2015/12/18/react-components-elements-and-instances.html)

### ES6 `const` e `let`

- Ver referência no repositório [Aprenda ES6 (JavaScript)](https://github.com/aferreira44/aprenda-es6-javascript)

### Immutable Data Structures

- Por quê elas fazem sentido em React e no seu eco-sistema?

### ReactDOM

- `ReactDOM.render()` espera 2 argumentos:
    - um JSX que será renderizado.
    - o lugar onde o React renderizá dentro do HTML.

Exemplo:

```js
ReactDOM.render(<App />, document.getElementById('root'));
```

- [Rendering Elements](https://facebook.github.io/react/docs/rendering-elements.html)

### Hot Module Reloading

- Evitar carregamento da página quando realiza alteração no código.
- Mantém o log no developer console.
- Mantém o estado da aplicação.

- Inserir código abaixo no final do entry-point `index.js`

```js
if (module.hot){
    module.hot.accept()
}
```

- [Dan Abramov - Live React: Hot Reloading with Time Travel](https://www.youtube.com/watch?v=xsSnOQynTHs)

### Key attribute `<div key={item.objectID}>`

- [Lists and Keys](https://facebook.github.io/react/docs/lists-and-keys.html)

- **Conceitos de Javascript por trás do React**

Object.assign()
Object.freeze()
spread operator (...this.state.object)

Component and PureComponent

setState()

Arrays são Objects

Evitar métodos mutáveis de arrays: push, pop, shift, unshift, splice, sort, reverse

Usar métodos imutáveis de array que retornam um novo array ou novo objeto: map, filter, reduce, every, some, slice

key field para renderizar arrays no DOM

Evitar efeitos colaterais com operadores: ++, -- e delete

Pure functions - render() method and functional components

Nome de Componente começa com maiúscula

Expressões ternárias

Short circuit && e ||

!! transforma para o equivalete booleano

Context(this) bind methods

## Referências

- [Introduction to React.js](https://www.youtube.com/watch?v=XxVg_s8xAms)
- [Livro - The Road to Learn React](https://leanpub.com/the-road-to-learn-react)