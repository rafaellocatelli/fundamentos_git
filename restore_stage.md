# Removendo mudanças do Stage



Caso tenha incluído um arquivo indesejado ao stage, você pode remove-lo (antes do commit) através do comando:   `git restore --staged [nome_do_arquivo]`



# Removendo arquivo do controle de versões sem deletar o arquivo do workspace

[Documentação Oficial](https://git-scm.com/docs/git-rm/pt_BR)

Mantém no workspace e remove do monitoramento e, se estiver no stage, remove do stage:    `git rm --cached [nome_do_arquivo]`


Para remover do workspace aleḿ de remover do controle de versão:    `git rm [nome_do_arquivo]`

