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
3. ⚠ Depois de ter colocado essas configurações e não for tente

- CTRL + SHIFT + P
- Format Document (in pop-up bar)
- Select Format Document
- Select Configure Default Formatter... 
- Select Prettier - Code formatter

**[⬆ voltar ao topo](#Índice)**
