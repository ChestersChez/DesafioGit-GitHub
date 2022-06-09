*Reforce seu conhecimento em Git com um desafio de projeto totalmente prático, onde você executará todos os passos para a criação, atualização e sincronização de um repositório no GitHub. Para isso, tenha em mente todas as dicas e direcionamentos apresentados pelo expert nas aulas. Dessa forma, você poderá compartilhar suas anotações e exercícios em seu próprio repositório. Criando assim, o primeiro (de muitos) projetos do seu portfólio ;)*

# Desafio repositório no GitHub.

*Criando um Repositório.*

- Vamos criar um novo repositório no site do github clicando em repositórios e clicando em New e vamos chama-lo de:  DesafioGit-GitHub.

- Agora nós vamos baixar esse repositório clonando-o para trabalhar em nossa máquina. clicando em code e copiando a chave ssh.

Beto@Chesters MINGW64 /c/MyWorkSpace
$ git clone git@github.com:ChestersChez/DesafioGit-GitHub.git

Beto@Chesters MINGW64 /c/MyWorkSpace
$ git clone git@github.com:ChestersChez/DesafioGit-GitHub.git
Cloning into 'DesafioGit-GitHub'...
remote: Enumerating objects: 6, done.
remote: Counting objects: 100% (6/6), done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 6 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (6/6), done.

- Entraremos em nosso diretório DesafioGit-GitHub. 

Beto@Chesters MINGW64 /c/MyWorkSpace
$ cd DesafioGit-GitHub/

Beto@Chesters MINGW64 /c/MyWorkSpace/DesafioGit-GitHub (main)
$









Vamos criar uma pasta de arquivos no diretório C:  para ser o nosso repositório e vamos chama-lá de: DesafioGitHub.

Beto@Chesters MINGW64 /c
$ mkdir DesafioGitHub

 Beto@Chesters MINGW64 /c
 $ cd/c/DesafioGitHub/

E logo a seguir usaremos o comando git init para inicializar o nosso novo      diretório no Git.

Beto@Chesters MINGW64 /c/DesafioGitHub
$ git init
 Initialized empty Git repository in C:/DesafioGitHub/.git/

Já na pasta do nosso diretório DesafioGitHub nós vamos criar um arquivo   markdown chamado: instruções-desafio-de-projeto.

Beto@Chesters MINGW64 /c/DesafioGitHub (master)
$ git add *

Beto@Chesters MINGW64 /c/DesafioGitHub (master)
$ git commit -m "commit inicial"
[master (root-commit) 184837c] commit inicial
1 file changed, 99 insertions(+)
create mode 100644 "instru\303\247\303\265es-desafio-de-projeto.md" 

Agora nós vamos criar lá no site git um novo repositório e a seguir vamos clicar em code e copiar uma chave ssh para clonar o nosso repositório em nossa máquina.

Beto@Chesters MINGW64 /c/DesafioGitHub (master)
$ git clone git@github.com:ChestersChez/DesafioGitHub.git
Cloning into 'DesafioGitHub'...
remote: Enumerating objects: 15, done.
remote: Counting objects: 100% (15/15), done.
remote: Compressing objects: 100% (9/9), done.
remote: Total 15 (delta 1), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (15/15), done.
Resolving deltas: 100% (1/1), done.

Vamos listar e verificar se o nosso arquivo está em nosso repositório.

Beto@Chesters MINGW64 /c/DesafioGitHub (master)
$ ls
DesafioGitHub/  instruções-desafio-de-projeto.md

Agora vamos verificar o status de nosso arquivo, caso houver a mensagem untracked como o nome do arquivo em vermelho nós deveremos o adicionar.

Beto@Chesters MINGW64 /c/DesafioGitHub (master)
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)

Precisaremos adicionar o nosso para que o mesmo esteja pronto para subir.

Beto@Chesters MINGW64 /c/DesafioGitHub (master)
$ git add .

Vamos verificar o status novamente e ver se o nosso arquivo está pronto , o nome do arquivo preparado estará verde.

Beto@Chesters MINGW64 /c/DesafioGitHub (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   DesafioGitHub

Agora com o nosso arquivo pronto iremos dar um commit.

Beto@Chesters MINGW64 /c/DesafioGitHub (master)
$ git commit -m "Instruções para o desafio de projeto"
[master 74729e0] Instruções para o desafio de projeto
 1 file changed, 99 deletions(-)
 delete mode 100644 "instru\303\247\303\265es-desafio-de-projeto.md"

Vamos verificar o status novamente.

Beto@Chesters MINGW64 /c/DesafioGitHub (master)
$ git status
On branch master
nothing to commit, working tree clean

E agora vamos empurrar o nosso arquivo para o git usando o comando push.



















Beto@Chesters MINGW64 /c/workspace (master)
$ mkdir  desafio-de-projeto.

$ cd /c/workspace/desafio-de-projeto/

Agora iremos iniciar o repositório no git.

Beto@Chesters MINGW64 /c/workspace/desafio-de-projeto (master)
$ git init
Initialized empty Git repository in C:/workspace/desafio-de-projeto/.git/

Entrando na pasta de desafio de projeto nós iremos criar esse arquivo de instruções com o Typora no formato markdown onde iremos executar todos os passos para a criação, atualização e sincronização de um repositório no GitHub.

Mas se verificarmos o status do arquivo veremos que ele ainda não está pronto, sendo necessário o adicionar ao Git.

Beto@Chesters MINGW64 /c/workspace/desafio-de-projeto (master)
$ git add .

Ao adicionar podemos verificar o status do arquivo para saber se o arquivo está pronto para o commit.

Beto@Chesters MINGW64 /c/workspace/desafio-de-projeto (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   "instru\303\247\303\265es-desafio-de-projeto.md"

Com o arquivo pronto nós vamos usar o comando -m para iniciar o commit.

Beto@Chesters MINGW64 /c/workspace/desafio-de-projeto (master)
$ git commit -m "commit inicial"

[master (root-commit) 08abfc6] commit inicial
 1 file changed, 65 insertions(+)
 create mode 100644 "instru\303\247\303\265es-desafio-de-projeto.md"

E assim com o arquivo em criptografia nós vamos prosseguir usando o comando?

$ git push oringin main

Beto@Chesters MINGW64 /c/workspace/desafio-de-projeto (master)
$ cd desafio-github

Beto@Chesters MINGW64 /c/workspace/desafio-de-projeto/desafio-github (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

















