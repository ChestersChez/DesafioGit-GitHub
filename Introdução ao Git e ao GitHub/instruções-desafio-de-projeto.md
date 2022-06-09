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

Iremos criar uma pasta chamada:  dentro do nosso diretório DesafioGit-GitHub com um arquivo markdown com as instruções para o seu primeiro commit.

Agora verificaremos o status de nosso arquivo.

$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        "Introdu\303\247\303\243o ao Git e ao GitHub/"

nothing added to commit but untracked files present (use "git add" to track)

Como o arquivo está Untrack e escrito em vermelho nós teremos que o adicionar para poder o enviar.

Beto@Chesters MINGW64 /c/MyWorkSpace/DesafioGit-GitHub (main)
$ git add .

Após adicionar iremos verificar novamento o status do arquivo, o nome do arquivo escrito em verde indica que ele está pronto.

Beto@Chesters MINGW64 /c/MyWorkSpace/DesafioGit-GitHub (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   "Introdu\303\247\303\243o ao Git e ao GitHub/instru\303\247\
303\265es-desafio-de-projeto.md"

Agora vamos dar um commit desse arquivo em nossa máquina para o repositório no git.

Beto@Chesters MINGW64 /c/MyWorkSpace/DesafioGit-GitHub (main)
$ git commit -m "Inclusão das instruções do curso git/GitHub"
[main f8f888f] Inclusão das instruções do curso git/GitHub
 1 file changed, 204 insertions(+)
 create mode 100644 "Introdu\303\247\303\243o ao Git e ao GitHub/instru\303\247\
303\265es-desafio-de-projeto.md"

Verificaremos novamente o seu status e como podemos observar há um commit por se realizar.

Beto@Chesters MINGW64 /c/MyWorkSpace/DesafioGit-GitHub (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

Iremos usar o comando push para empurrar o nosso arquivo enviando-o para o git/github.

Beto@Chesters MINGW64 /c/MyWorkSpace/DesafioGit-GitHub (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 2.16 KiB | 369.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:ChestersChez/DesafioGit-GitHub.git
   8998463..f8f888f  main -> main

E pronto dessa forma os arquivos já foram enviados para o site do Git/GitHub.



































