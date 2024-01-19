# Arquitetura Git


## Banco de dados de Objetos

Todos os objetos são armazenados em     `.git/objects`

Para visualizar a estrutura:

```bash
$ find .git/objects
```


## Formato Objeto Git

`{tipo_do_objeto} {tamanho_do_conteudo}\o{conteudo}`

Exemplo:
```bash
$ echo "rafael locatelli" | git hash-object --stdin
4738ce74d04f0aa4236a0ab7f403d2b771e0b478
$ echo -e "blob 17\0rafael locatelli" | sha1sum
4738ce74d04f0aa4236a0ab7f403d2b771e0b478
```

Para ler o objeto:
```bash
$ git cat-file -p 4738ce74d04f0aa4236a0ab7f403d2b771e0b478
rafael locatelli
```

## Adicionando objeto ao stage

Para adicionar um objeto que não consta no diretório:
`git update-index --add --cacheinfo 100644 {hash-object} [nome_do_arquivo]` 

Para adicionar um objeto que consta no diretório:
`git update-index {hash-object} [nome_do_arquivo]`


Após adicionar todos os objetos desejados, o Git agrupa tudo em um objeto árvore usando o comando   `git write-tree`

