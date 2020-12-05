# git_workflow
Repositório com conteúdo básico sobre o Git

### Objetivo:
Este repositório contém comandos básicos do Git que podem ajudar a todos que estão iniciando o uso desta ferramenta.
Através do Git você poderá versionar seus projetos e integra-lo com esta "rede social" de desenvolvedores que é o Github, dando visibilidade e agilidade ao seu trabalho.

### Configuração do Ambiente:
Estes são os passos iniciais para configurar o Git no seu computador e iniciar o seu uso:

1. Abrir uma conta do Github.
2. Instalar o Git no seu computador.
3. Configurar o Git (local) com as informações de usuário/e-mail do Github, isto permitirá que no futuro você possa enviar seus projetos e arquivos para o repositório no Github.

```
git config --global user.name "Nome do usuário"
git config --global user.email "E-mail do usuário"
```
_Utilizar o nome de usuário e e-mail utilizados para criação da conta no Github_

### Comandos Básicos:
Estes são comandos básicos utilizados para trabalhar no repositório local:

1. Iniciar/Habilitar o Git para fazer o *tracking* de um diretório e seus arquivos:

```
git init
```

2. Verificar o status do seu repositório, identificar se possuem arquivos que precisam ser adicionados na *stage area* para que o Git possa fazer o *tracking*:
```
git status
```

3. Adicionar arquivos na *stage area*:
```
git add "nome do arquivo"

ou 

git add * (para adicionar todos os arquivos)
```

4. Efetuar *commit* dos arquivos que estão na *stage area*:
```
git commit -m "mensagem (ex. Commit inicial do projeto)"
```

5. Verificar o log do Git, onde são registrados todos os commits efetuados no repositório:
```
git log
```

### Comandos Adicionais:

Configurar arquivo *gitignore*, este arquivos deve conter o nome de arquivos e diretórios que estão no repositório mas *não serão trackeados/versionados* pelo Git:
1. Na raiz do repositório, criar um arquivo com o nome *.gitignore*.
2. Adicionar no arquivo os nomes de arquivos ou diretórios que não serão versionados e salvar o arquivo.
3. Executar o *git add* e *git commit* para o arquivo.

Pronto, o git irá ignorar todos os arquivos/diretórios listados neste arquivos.

### Sincronização com repositório remoto:

1. Criar o repositório remoto no Git (preciso já ter criado um usuário na plataforma) e copiar a URL do seu repositório criado no Git

2. No diretório local do seu computador executar:

```
git add remote origin <url-do-seu-repositorio-no-git>
```
**ex.: git add remote origin https://github.com/isasouza-com/git_workflow.git**

3. Para sincronizar conteúdo do diretório remoto com o diretório local do seu computador:

```
git pull origin main
```
