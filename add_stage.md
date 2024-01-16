# Adicionando as mudanças ao Stage

Para adicionar todas as mudanças:   `git add .`

Para adicionar as mudanças de um arquivo específico:    `git add [nome_do_arquivo]`

Para adicionar as mudanças de arquivos com determinada extensão:    `git add *.[extensão]`

Exemplo: 
```bash
$ git add *.html
```

Para adicionar as mudanças de forma interativa:     `git add -i`

Exemplo:

Ao digitar `git add -i`, o git listará todas as mudanças e um menu de comandos:
```bash
# lista das mudanças ocultado
*** Commands ***
  1: status       2: update       3: revert       4: add untracked
  5: patch        6: diff         7: quit         8: help
```

Você poderá selecionar as opções digitando o seu número ou primeira letra correspondente.

```bash
# para acessar add untracked
$ a
```

As opções *update*, *revert* e *add untracked* exibirão a lista numérica de arquivos que sofreram suas mudanças e você poderá selecionar qual arquivo fará parte do Stage selecionando o número (ex: "1") ou uma sequência de número (ex: "1-3 7,9") 
