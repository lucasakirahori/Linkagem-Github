
> # PRINCIPAIS COMANDOS
## CRIAR REPOSITÓRIO
1° Criar o repositório no GitHub; <br>
2° No terminal do VSCODE usar os comandos abaixo: <br>
`echo "# [nome-do-repositorio]" >> README.md` <br>
`git init` <br>
`git add .`  /Sobe todos os arquivos <br>
`git commit -m "[Mensagem de Commit]"` <br>
`git branch -M [nome-da-branch]` <br>
`git remote add origin [https://github.com/[usuario]/[nome-repositorio].git]` <br>
`git push -u origin [nome-da-branch]`

## IMPUTAR EM REPOSITÓRIO EXISTENTE

`git add .` <br>
`git commit -m "[Mensagem de Commit]"` <br>
`git branch -M [nome-da-branch]` <br>
`git push -u origin [nome-da-branch]` <br>


## CLONAR DO GITHUB PARA O ARQUIVO LOCAL
`git clone ssh://git@github.com/[usuario]/[nome-repositorio].git`

## PARA ATUALIZAR DO GITHUB PARA A MÁQUINA
`git pull origin [nome-da-branch]`

ALTERNATIVO: git remote -v  /verifica se houve a linkagem <br>
ALTERNATIVO: git add README.md <br>
ALTERNATIVO: git config user.name "[nome]" <br>
ALTERNATIVO: git config user.email "[email.com]"


> # OUTROS COMANDOS

* ## Criação de Projetos
|---|---|
|`git init` | Inicializa um repositório Git local <br>
|`git clone ssh://git@github.com/[usuario]/[nome-repositorio].git` | Cria uma cópia na máquina de um repositório remoto

* ## Básicos

`git status` /Checa o status <br>
`git add [nome-arquivo.txt]` /Adiciona um arquivo para área de stage <br>
`git add .` /Adiciona todos os arquivos novos ou modificados para a área de stage <br>
`git commit -m "[Mensagem de Commit]"` /Comita as alterações <br>
`git rm -r [nome-arquivo.txt]` /Remove um arquivo (ou pasta)

* ## Branching & Merging

`git branch` /Lista as branches (o asterisco denota a branch atual) <br>
`git branch -a` /Lista todas as branches (local e remoto) <br>
`git branch [nome da branch]`	/Cria uma nova branch <br>
`git branch -d [nome da branch]`	/Deleta uma branch <br>
`git push origin --delete [nome da branch]`	/Deleta uma branch remota <br>
`git checkout -b [nome da branch]`	/Cria uma nova branch e muda para ela <br>
`git checkout -b [nome da branch] origin/[nome da branch]`	/Clona uma branch remota e muda para ela <br>
`git checkout [nome da branch]`	/Seleciona uma branch <br>
`git checkout -`	/Muda para a última branch <br>
`git checkout -- [nome-arquivo.txt]`	/Descarta modificações de um arquivo <br>
`git merge [nome da branch]`	/Faz um merge de uma branch na branch atual <br>
`git merge [source branch] [branch alvo]`	/Faz um merge de uma branch em outra branch <br>
`git stash`	/Tirar o estado sujo do seu diretório de trabalho <br>
`git stash clear`	/Remove todas as entradas 'stash'

* ## Sharing & Updating Projects

`git push origin [nome da branch]`	/Enviar uma branch para seu repositório remoto <br>
`git push -u origin [nome da branch]`	/Envia as alterações da branch informada para um repositório remoto (and selecionar a branch) <br>
`git push`	/Envia as alterações para o repositório remoto (branch atual) <br>
`git push origin --delete [nome da branch]`	/Deletar uma branch remota <br>
`git pull`	/Atualiza o repositório da máquina com o último commit <br>
`git pull origin [nome da branch]`	/Recebe alterações do repositório remoto <br>
`git remote add origin ssh://git@github.com/[usuario]/[nome-repositorio].git`	/Adicionar um repositório remoto <br>
`git remote set-url origin ssh://git@github.com/[usuario]/[nome-repositorio].git`	/Seta um repositório da origin branch para o SSH

* ## Inspeção & Comparação

`git log`	/Ver modificações <br>
`git log --summary`	/Ver modificações (detalhadas) <br>
`git diff [branch original] [branch alvo]`	/Visualizar alterações antes de mesclar
