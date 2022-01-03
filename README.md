# :rocket: Iniciando o projeto

1 - Crie um diretório onde ficará o seu projeto (React)

```js
mkdir your-project 
```

2 - Entre no diretório e execute o seguinte comando

```js
yarn init -y
```

3 - Instale as dependências principais do projeto

```js
yarn add react react-dom
```

4 - Crie um diretório chamado `public` e outro `src` na raiz do projeto

> src: onde ficará todo o código do projeto
    
> public: onde ficará arquivos publicos do projeto. *Exemplo: index.html, robots.txt, favicon.png, assets/*

## Adicionando babel a aplicação

Ele será responsável por converter o código para algo que os browser entendam. [Leia mais](https://babeljs.io/docs/en/)

1 - Instale as dependências como desenvolvimento de projeto

```js
yarn add @babel/core @babel/cli @babel/preset-env @babel/preset-react -D
```

> @babel/core: é todo o núcleo do projeto, o coração do babel.
    
> @babel/cli: permite que você execute comandos via terminal. *Exemplo: yarn babel -h*

> @babel/preset-env: identifica qual ambiente você esta executando para que converta da melhor forma possível, seja `browser` ou `node`.

> @babel/preset-react: para que seja possível o entendimento do código `html` escrito dentro de arquivos `js`, ou seja, a sintaxe `jsx`

2 - Crie um arquivo na raiz do projeto `.babelrc` ou `babel.config.js` com o seguinte conteúdo

```js
module.exports = {
  presets: [
    '@babel/preset-env',
    '@babel/preset-react'
  ]
}
```
