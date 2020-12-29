### Comando ESLint não encontra os erros ⤵

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

### Correção automática

Não são todas vezes, mas esse comando faz com que ele corrija automáticamente, exemplo:

```bash
npx eslint src --fix
```
