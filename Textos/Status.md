![Logo do Git](./../Imagens/icoGit.png) ![Logo do GitHub](./../Imagens/icoGitHub.png)
# Ciclo de Vida do Repositório  

Os arquivos e pastas de um repositório local podem se encontrar em um dos seguintes status:  

1. **Untracked** – quando o arquivo/pasta ainda não foi conhecido pelo Git, ou seja, não faz parte do repositório. Neste caso, o arquivo foi criado ou modificado, mas ainda não foi adicionado ao controle de versionamento. Fazemos isto com o comando `git add`.  

2. **Tracked** – quando o arquivo/pasta já é conhecido pelo Git. Nesta situação, ele pode possuir três status:  

1. **Unmodified** - assim que o arquivo/pasta é adicionado no Git ele passa a este status, ou seja, após ser adicionado ao controle de versão ele assume o status de *não modificado*. Como o arquivo/pasta não possui modificação, ele imediatamente é colocado em uma área denominada Staged, que é uma espécie de área onde o Git armazena tudo aquilo que aguarda confirmação das ações realizadas.

2. **Modified** – ocorre quando um arquivo/pasta for editado. Neste momento, o arquivo/pasta sai da área Staged comentada anteriormente. Para voltar a ela, usa-se o comando `git add`.

3. **Staged** – status do arquivo/pasta após ser modificado e atualizado com o comando `git add`. Após ser adicionado a este status, as modificações podem ser confirmadas utilizando o comando `git commit` , passando via comando uma mensagem que deixe claro quais foram as modificações atualizadas (vide Principais Commandos).  
Após o uso do comando git-commit, o arquivo/pasta passa de fato a fazer parte do repositório.

Importante destacar que para verificar a situação de um repositório, podemos utilizar o comando git status.

[Voltar](./../README.md)
 


 