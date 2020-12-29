## Comando ESLint não encontra os erros ⤵

```bash
eslint [nomeDaPasta]
```

Se caso retorna algum error igual da print a baixo:

<p align="left">
  <img src="/help/img/print-01.png">
</p>

Você pode usar o comando usando o `npx` no começo, exemplo:

```bash
npx eslint src
```

<p align="left">
  <img src="/help/img/print-02.png">
</p>

Agora sim podemos ver que já foi avisado do error.

## Correção automática

Não são todas vezes, mas esse comando faz com que ele corrija automáticamente, exemplo:

```bash
npx eslint src --fix
```
caso não corrija, uma mensagem igual da `print` a cima vai aparecer.


## Adicionando atalho

Caso queria rodar isso de fomar mais rápida, basta adicionarmos ao nosso `package,json`.

```json
"scripts": {
  "lint": "eslint src"
},
```

Feito isso, basta rodar no terminal `yarn eslint` que ele vai verificar da mesma forma, só mudamos o jeito de rodar esse comando.
