- [Índice](#índice)
  - [Comando ESLint não encontra os erros](#comando-eslint-não-encontra-os-erros)
  - [Meu prettier não está formatando o código](#meu-prettier-não-está-formatando-o-código)

### Comando ESLint não encontra os erros

```bash
eslint [nomeDaPasta]
```

Se caso retorna algum error igual da print a baixo:

  <p align="left">
    <img src="/help/img/eslint-print-01.png">
  </p>

Você pode usar o comando usando o `npx` no começo, exemplo:

```bash
npx eslint src
```

<p align="left">
  <img src="/help/img/eslint-print-02.png">
</p>

Agora sim podemos ver que já foi avisado do error.

## Correção automática

Não são todas vezes, mas esse comando faz com que ele corrija automáticamente, exemplo:

```bash
npx eslint src --fix
```
caso não corrija, uma mensagem igual da `print` a cima vai aparecer.


## Adicionando atalho

Caso queria rodar isso de fomar mais rápida, basta adicionarmos ao nosso `package.json`

```json
"scripts": {
  "lint": "eslint src"
},
```

Feito isso, basta rodar no terminal `yarn eslint` que ele vai verificar da mesma forma, só mudamos o jeito de rodar esse comando.

## Meu prettier não está formatando o código

1. Caso não tenha, instale com `yarn add -D prettier`, reinicie o editor e tente novamente.

2. Verifique se o teu VS Code está configurado para formatar ao salvar. Você precisa ter um arquivo _na raiz do projeto_como `.vscode/settings.json` ou salvar diretamento no `settings.json`, segue abaixo o código:

```json
{
  "editor.formatOnSave": false,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  }
}
```

## ⚠ Depois de ter colocado essas configurações e não for tente ⤵

- CTRL + SHIFT + P
- Format Document (in pop-up bar)
- Select Format Document
- Select Configure Default Formatter... 
- Select Prettier - Code formatter
