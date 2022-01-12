![Logo do Git](./../Imagens/icoGit.png) ![Logo do GitHub](./../Imagens/icoGitHub.png)

# Início e Navegação

Para começar a trabalhar com o git, devemos localizar o aplicativo git.bash (interface CLI para distribuições Linux) ou git.cmd (interface CLI para Windows).  
Através dos comandos de navegação entre pastas (sejam para distribuições linux ou windows) podemos navegar entre as estruturas de pastas e a partir daí criar o repositório local e utilizar os comandos git propriamente ditos, cujos principais estão descritos abaixo.

# Principais Comandos Git

1. **git init** - Basicamente é o primeiro comando que vamos utilizar. Serve para inicializar um repositório local na pastinha em que vamos trabalhar. 

2. **git status** – traz o status do repositório atual. 

3. **git add** *<nomeArquivo.extensao>* - modifica o status do arquivo de untracked para unmodified, adicionando-o ao repositório. Para adicionar vários arquivos e pastas utilizamos `git add *`. Repare que ao invés de mencionarmos o nome do arquivo no comando, mencionamos apenas "*", que significa tudo.
 
4. **git commit -m** *"breve mensagem que informa o que de fato foi feito no código. Por exemplo: adição de determinada funcionalidade, resolução de determinado bug, etc.."* - comando que permite ao git criar um *snapshot* (imagem) do repositório, passando uma mensagem que identifique as modificações realizadas. 

5. **git commit –am** *"breve mensagem"* - permite adicionar todos os arquivos modificados ao *snapshot* (imagem) criado, além de uma breve mensagem informando o que foi feito na atualização. 

Basicamente, sempre que modificarmos algo, precisaremos usar o comando **git add** e **git commit**. 

[Voltar](./../README.md)
 


 