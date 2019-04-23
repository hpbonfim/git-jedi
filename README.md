# Git Guy - Guía de Comandos GIT

<h1 align="center">
	<br>
	<br>
	<img  src="https://i.imgur.com/BqtWixA.png" alt="git-hpbonfim">
	<br>
	<br>
	<br>
</h1>

> Git é um software de controle de versão projetado por _Linus Torvalds_, pensando na eficiência e confiabilidade de manter versões de aplicativos quando eles têm um grande número de arquivos de código.

## Vantagens:
	- ✔️ Melhor trabalho em equipe <br>
	- ✔️ Controle total sobre as alterações em projetos <br>
	- ✔️ Voltar às versões anteriores <br>
	- ✔️ Locais & Remotes Repositórios <br>
	- ▪️▪️▪️ E muito mais

> **Download** <br>
    Linux Debian: `$ sudo apt-get install git` <br>
    Linux Fedora: `$ sudo yum install git` <br>
    [Mac](http://git-scm.com/download/mac) <br>
    [Windows](http://git-scm.com/download/win) <br>
  **Você pode escrever os comandos no seu CMD ou no terminal do git bash**
  
## Sobre este guia:
	- 🔈 Tudo em negrito significa que o valor é relativo, muda de acordo com cada um.
	- 🔈 Não é uma versão finalizada.

# Comandos para virar o Mestre Jedi 🚀

___

### Versão do GIT: 🕵

```
git --version
```

### Definindo seu nome: ✋

<pre>
git config --global user.name <b>"hpbonfim"</b>
</pre>

### Definindo seu e-mail : ✉️

<pre>
git config — global user.email <b>“hp_bonfim@hotmail.com”</b>
</pre>

### Listar configurações: 🌍

<pre>
git config —-list
</pre>

### Listar configurações do usuário: 🌞

<pre>
git config --list --global
</pre>

### Precisa de ajuda? 🙏

```
git help  
```

### Precisa de ajuda com commits? 👏

<pre>
git help <b>commit</b>
</pre>

### Criando um Repositório 👊

<pre>
git init
</pre>

### Deletando um Repositório :boom:

<pre>
rm -rf .git
</pre>

### Add um arquivo 👉

<pre>
git add <b>index.html</b>
</pre>

### Add vários arquivos 🖖
<pre>
git add <b>index.html index.js</b>
</pre>

### Add todos os arquivos 💥

<pre>
git add .
</pre>

### Add todos os arquivos de um diretório específico pelo tipo: 🌕

<pre>
git add <b>*.txt</b>
</pre>

### Add todos os arquivos dentro de uma pasta: 📁

<pre>
git add <b>css/</b>
</pre>

### Add todos os arquivos que foram modificados: 〽️

<pre>
git add -u
</pre>

### Add todos os arquivos pelo tipo dentro de uma pasta específica: 📂

<pre>
git add <b>pdfs/*.pdf</b>
</pre>

### Ver todos os arquivos modificados 🔦

<pre>
git status
</pre>

### Ver todos os arquivos modificados de forma resumida: 🤐

<pre>
git status -s
</pre>

### Ver todos os arquivos modificados da branch atual: 🔆

<pre>
git status -sb
</pre>

### Excluir um arquivo que estava na área de teste  ⛔️

<pre>
git reset <b>index.js</b>
</pre>

### Excluir um arquivo que estava na área de teste por seu tipo ❌

<pre>
git reset <b>*.xml</b>
</pre>

### Commit e add mensagem 📝

<pre>
git commit -m <b>'navbar created'</b>
</pre>

### Ver todos os commits criados 👀

<pre>
git log
</pre>

### Ver todos os commits criados mais informativos 🌲

<pre>
git log --oneline --decorate --all --graph
</pre>

### Criando um Atalho(Aliase) Global 💧

<pre>
git config --global alias.<b>lg</b> "log --oneline --decorate --all --graph"
</pre>
*Agora digite: `git lg`  para usar o atalho criado para commits mais informativos* 👆

___

## Resumo dos comandos básicos e essênciais do GIT

- `$ git init` -> Inicializando um repositório local
- `$ git add <file>` -> Add arquívos que estão sendo trabalhados
- `$ git status` -> Verificar os estados dos arquivos modificados
- `$ git commit` -> Commitar mudanças
- `$ git push` -> Enviar para um repositório remoto

<h1 align="center">
<img src="https://i.imgur.com/heTewJo.png" alt="git-hpbonfim">
</h1>

### Veja todas as alterações que ocorreram entre o arquivo de trabalho e o arquivo de teste 📍

<pre>
git diff
</pre>

### Veja todas as alterações que ocorreram entre o arquivo da branch original e o arquivo commitado ⭕

<pre>
git diff --staged
</pre>

### Recuperando Arquivos 💞

<pre>
git checkout .
</pre>

### Deletando todas as mudanças feitas em um arquivo 📄

<pre>
git checkout -- <b>README.md</b>
</pre>

### Add arquivo e Add mensagem no mesmo comando: 🌟

<pre>
git commit -am <b>'README actualizado'</b>
</pre>

### Editar a mensagem de algum commit ✏️

<pre>
git commit --amend -m <b>'We edited the message!'</b>
</pre>

### Add ou Resetar o commit anterior ↶

<pre>
git reset --soft HEAD^
</pre>

### Retornar para um commit específico anterior de maneira fraca ↖️

<pre>
git reset --soft <b>39ae8e6</b>
</pre>

### Retornar para um commit específico anterior de maneira forte ⬅️🔄

<pre>
git reset --hard <b>39ae8e6</b>
</pre>

### Listar origem dos commits 📋

<pre>
git reflog
</pre>

### Renomear Arquivos ✍️

<pre>
git mv <b>index.js app.js</b>
</pre>

### Deletando um Arquivo ❌

<pre>
git rm <b>app.js</b>
</pre>

## Branches

> Uma Branch é basicamente uma nova linha de tempo que armazena os commits. Eles são usados para desenvolver funcionalidades independentes umas das outras. A ramificação principal é a ramificação padrão quando você cria um repositório. Crie novos ramos durante o desenvolvimento e junte-os ao ramo principal quando terminar.

<h1 align="center">
<img src="https://i.imgur.com/k7840Gk.png" alt="git-hpbonfim">
</h1>

### Criando uma branch: 🔱

<pre>
git branch <b>myBranch</b>
</pre>

### Veja todas as branchs do repositório: 🔅

<pre>
git branch
</pre>

### Trabalhando em uma branch específica 🌿

<pre>
git checkout <b>myBranch</b>
</pre>

### Criando e movendo uma branch em um único comando 🍀

<pre>
git checkout -b <b>myBranch</b>
</pre>

## Merge branches:

### Primeiro retornamos para a branch master: ❄️

<pre>
git checkout master
</pre>

### Agora fazemos o merge(substituição) da origin -> master 🌻

<pre>
git merge <b>myBranch</b>
</pre>

### Depois de realizado o merge, deletamos a branch antiga 🌹

<pre>
git branch -d <b>myBranch</b>
</pre>

## Tags

### Crie uma tag 💅🏼

<pre>
git tag -a <b>v1.0.0</b> -m <b>"Version 1.0.0"</b>
</pre>

### Insira uma tag em um commit específico 🔖

<pre>
git tag -a <b>v0.1.0 43809d4</b> -m <b>'Alpha Version'</b>
</pre>

### Veja todas as Tags 🎌

<pre>
git tag
</pre>

### Veja a mensagem da tag 👁‍🗨

<pre>
git show <b>v1.0.0</b>
</pre>

### Delete uma tag ✖️

<pre>
git tag -d <b>v0.1.0</b>
</pre>

## Stash

### Criando sua stash 📦

<pre>
git stash
</pre>

### Veja a lista 💼

<pre>
git stash list
</pre>


# Github

<h1 align="center">
	<br>
	<br>
	<img  src="https://i.imgur.com/cfJdgeP.png" alt="github-hpbonfim">
	<br>
	<br>
	<br>
</h1>

### Depois de criar o repositório local, precisamos adicionar um repositório server: 📮

<pre>
git remote add origin <b>yourRepo.git</b>
</pre>

### Veja os repositórios remotos: ⬛

<pre>
git remove -v
</pre>

Depois de dar os commits, e escolher um repositório, podemos mandar para o Github:

### Push: ✈️

<pre>
git push -u origin master
</pre>

<h1 align="center">
<img src="https://i.imgur.com/wFHA5k0.png" alt="git-hpbonfim">
</h1>

Mas, como você pode ver, as tags não são enviadas com o comando `git push`:

<h1 align="center">
<img src="https://i.imgur.com/wFHA5k0.png" alt="git-hpbonfim">
</h1>

### Push tags ▶️

<pre>
git push --tags
</pre>

### Ignore Files ❗️

<sub>Crie arquivos .gitignore para arquivos e pastas que você não quer subir para o git:</sub>

<pre>
node_modules
package-lock.json
</pre>

### Pull 🌌

<pre>
git pull
</pre>

<h1 align="center">
<img src="https://i.imgur.com/xMtw6uq.png" alt="git-hpbonfim">
</h1>

### Clonar um Repositorio ⌛

<pre>
git clone <b>repoUrl.git</b>
</pre>

### Clonar um repositório em uma pasta específica 📁

<pre>
git clone <b>repoUrl.git my-folder</b>
</pre>

___

