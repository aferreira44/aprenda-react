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

### ES6 Classes



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

### State and Lifecycle

[State and Lifecycle](https://facebook.github.io/react/docs/state-and-lifecycle.html)

### React Events

[Handling Events](https://facebook.github.io/react/docs/handling-events.html)

### React Forms

[React Forms](https://facebook.github.io/react/docs/forms.html)

### Components and Props

#### this.props

[Components and Props](https://facebook.github.io/react/docs/components-and-props.html)

### Composition vs Inheritance

[Composition vs Inheritance](https://facebook.github.io/react/docs/composition-vs-inheritance.html)

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

Components: stateful and stateless (o ideal é que os componentes sejam stateless)

### Components and Props

[Components and Props](https://facebook.github.io/react/docs/components-and-props.html)

### Typechecking With PropTypes

[Typechecking With PropTypes](https://facebook.github.io/react/docs/typechecking-with-proptypes.html)

### React Styling

- [FormidableLabs/radium](https://github.com/FormidableLabs/radium)
- [Khan/aphrodite](https://github.com/Khan/aphrodite)
- [styled-components/styled-components](https://github.com/styled-components/styled-components)
- [css-modules/css-modules](https://github.com/css-modules/css-modules)

### Lifecycle Methods

- [React.Component](https://facebook.github.io/react/docs/react-component.html)
- [State and Lifecycle](https://facebook.github.io/react/docs/state-and-lifecycle.html)

### Conditional Rendering

- [All the Conditional Renderings in React](https://www.robinwieruch.de/conditional-rendering-react/)
- [Conditional Rendering](https://facebook.github.io/react/docs/conditional-rendering.html)

### Synthetic Event

[Synthetic Event](https://facebook.github.io/react/docs/events.html)

### Jest Testing Framework

- [Jest](https://facebook.github.io/jest/)
- [Testing React Apps](https://facebook.github.io/jest/docs/en/tutorial-react.html)
- [Snapshot Testing](https://facebook.github.io/jest/docs/en/snapshot-testing.html)

### Enzyme - Unit Tests

- [Enzyme](https://github.com/airbnb/enzyme)


### Ref Attribute

- [Refs and the DOM](https://facebook.github.io/react/docs/refs-and-the-dom.html)
- [When to use React's Ref on a DOM node in React](https://www.robinwieruch.de/react-ref-attribute-dom-node/)

## Referências

- [Introduction to React.js](https://www.youtube.com/watch?v=XxVg_s8xAms)
- [Livro - The Road to Learn React](https://leanpub.com/the-road-to-learn-react)
- [React Documentation](https://facebook.github.io/react/)
- [React Blog](https://facebook.github.io/react/blog/)
