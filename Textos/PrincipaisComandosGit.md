![Logo do Git](./../Imagens/icoGit.png) ![Logo do GitHub](./../Imagens/icoGitHub.png)

# Início e Navegação

Para começar a trabalhar com o git, devemos localizar o aplicativo git.bash (interface CLI para distribuições Linux) ou git.cmd (interface CLI para Windows).  
Através dos comandos de navegação entre pastas (sejam para distribuições linux ou windows) podemos navegar entre as estruturas de pastas e a partir daí criar o repositório local e utilizar os comandos git propriamente ditos, cujos principais estão descritos abaixo.

# Principais Comandos Git - Criação do Repositório  

1. **git config** - Comando que permite verificar ou atribuir algumas configurações relacionadas ao Git. Exemplos:  

	1. `git config username.email "seu e-mail aqui"` - Estamos atribuindo um novo valor para o e-mail do usuário.  
	2. `git config username.email` - Estamos verificando o valor atribuído para o e-mail do usuário.  
	3. `git config --list` - Lista todas as configurações e respectivos valores.

2. **git init** - Basicamente é o primeiro comando que vamos utilizar. Serve para inicializar um repositório local na pastinha em que vamos trabalhar. 

3. **git status** – traz o status do repositório atual. 

4. **git add** *<nomeArquivo.extensao>* - modifica o status do arquivo de untracked para unmodified, adicionando-o ao repositório. Para adicionar vários arquivos e pastas utilizamos `git add *`. Repare que ao invés de mencionarmos o nome do arquivo no comando, mencionamos apenas "*", que significa tudo.
 
5. **git commit -m** _<mensagem>_ - comando que permite ao git criar um *snapshot* (imagem) do repositório, passando uma mensagem que identifique as modificações realizadas. No local da mensagem, devemos informar o que de fato foi feito no código. Por exemplo: adição de determinada funcionalidade, resolução de determinado bug, etc..
A mensagem deve ser digitada entre aspas.

6. **git commit –am** _<mensagem>_ - permite adicionar todos os arquivos modificados ao *snapshot* (imagem) criado, além de uma breve mensagem informando o que foi feito na atualização, conforme item anterior. 
A mensagem deve ser digitada entre aspas.

Basicamente, sempre que modificarmos algo, precisaremos usar o comando **git add** e **git commit**. 

# Principais Comandos Git - Desfazer Ações Realizadas no Repositório  

1. **git checkout** *<nomeArquivo.extensão>* - Comando que permite trazer os arquivos/pastas do repositório ao estado anterior, ou seja, não modificado.  

2. **git reset** *<nomeArquivo.extensão>* - Comando que permite trazer os arquivos/pastas do repositório ao estado anterior APÓS a utilização do comando `git add`. Neste caso, os arquivos/pastas saem do status "Staged".

3. **git reset** *<opção>* *<nomeArquivo.extensão>* - Comando que permite trazer os arquivos/pastas do repositório ao estado anterior APÓS a utilização do comando `git commit`. Neste caso, os arquivos/pastas voltam para o status "Staged".
Em opção podemos utilizar os seguintes parâmetros:

	1. `--sotf` - Esta opção permite o arquivo/pasta retornar ao estado anterior a execução do comando `git commit`, ou seja, "staged".
	2. `--mixed` - Esta opção permite o arquivo/pasta retornar ao estado anterior a execução do comando `git add`, ou seja, para última modificação realizada.
	3. `--hard` - Esta opção permite o arquivo/pasta retornar ao estado anterior antes de sua criação, ou seja, o arquivo/pasta deixa de existir sem deixar rastros.
	Deve ser usado com bastante cuidado pois altera o histórico, em especial quando a mudança já está em repositório web compartilhado. 


[Voltar](./../README.md)
 


 