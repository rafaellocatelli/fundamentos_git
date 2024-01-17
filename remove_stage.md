# Removendo arquivo do controle de versões sem deletar o arquivo do workspace

[Documentação Oficial](https://git-scm.com/docs/git-rm/pt_BR)


Remove arquivo do Stage (se estiver) e Work Directory:  `git rm [nome_do_arquivo]`

Porém, não funciona sem argumento.

`git rm --cached [nome_do_arquivo]`     - Remove do Stage e do Monitoramento
`git rm -f [nome_do_arquivo]`           - Remove do Stage, do Work Directory e do Monitoramento

Remove arquivo do Stage: `git rm --cached [nome_do_arquivo]`