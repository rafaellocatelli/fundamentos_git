# Obtendo um repositório Git

Para inicializar um repositório em um diretório existente, basta utilizar:  `git init`

Exemplo:
```bash
$ mkdir nome_do_projeto
$ cd nome_do_projeto
$ git init
```

Para criar um novo repositório local com um nome especificado, use:  `git init [nome-do-projeto]`

Exemplo:
```bash
$ git init nome_do_projeto
$ cd nome_do_projeto
```

Para clonar um repositório existente, use:  `git clone [url]`

Exemplo clonando de um diretório na máquina local:
```bash
$ git clone ~/Documentos/nome_do_projeto
$ cd nome_do_projeto
```

Exemplo clonando do GitHub:
```bash
$ git clone https://github.com/rafaellocatelli/fundamentos_git
$ cd fundamentos_git
```