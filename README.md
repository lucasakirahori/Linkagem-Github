<details>
<summary>PRINCIPAIS COMANDOS</summary>
  
### CRIAR REPOSITÓRIO
1° Criar o repositório no GitHub; <br>
2° No terminal do VSCODE usar os comandos abaixo: <br>
`echo "# [nome-do-repositorio]" >> README.md` <br>
`git init` <br>
`git add .`  /Sobe todos os arquivos <br>
`git commit -m "[Mensagem de Commit]"` <br>
`git branch -M [nome-da-branch]` <br>
`git remote add origin [https://github.com/[usuario]/[nome-repositorio].git]` <br>
`git push -u origin [nome-da-branch]`

### INPUTAR EM REPOSITÓRIO EXISTENTE

`git add .` <br>
`git commit -m "[Mensagem de Commit]"` <br>
`git branch -M [nome-da-branch]` <br>
`git push -u origin [nome-da-branch]` <br>


### CLONAR DO GITHUB PARA O ARQUIVO LOCAL
`git clone ssh://git@github.com/[usuario]/[nome-repositorio].git`

### PARA ATUALIZAR DO GITHUB PARA O ARQUIVO LOCAL
`git pull origin [nome-da-branch]`

### ALTERNATIVOS
`git remote -v`  /verifica se houve a linkagem <br>
`git add README.md` <br>
`git config user.name "[nome]"` <br>
`git config user.email "[email.com]"`
</details>

<details>
<summary>OUTROS COMANDOS</summary>

### Criação de Projetos
| Comando | Descrição |
| --- | --- |
`git init` | Inicializa um repositório Git local
`git clone ssh://git@github.com/[usuario]/[nome-repositorio].git` | Cria uma cópia na máquina de um repositório remoto

### Básicos
| Comando | Descrição |
| --- | --- |
`git status` | Checa o status
`git add [nome-arquivo.txt]` | Adiciona um arquivo para área de stage
`git add .` | Adiciona todos os arquivos novos ou modificados para a área de stage
`git commit -m "[Mensagem de Commit]"` | Comita as alterações
`git rm -r [nome-arquivo.txt]` | Remove um arquivo (ou pasta)

### Branching & Merging
| Comando | Descrição |
| --- | --- |
`git branch` | Lista as branches (o asterisco denota a branch atual)
`git branch -a` | Lista todas as branches (local e remoto)
`git branch [nome da branch]`	| Cria uma nova branch
`git branch -d [nome da branch]`	| Deleta uma branch
`git push origin --delete [nome da branch]`	| Deleta uma branch remota
`git checkout -b [nome da branch]`	| Cria uma nova branch e muda para ela
`git checkout -b [nome da branch] origin/[nome da branch]`	| Clona uma branch remota e muda para ela
`git checkout [nome da branch]`	| Seleciona uma branch
`git checkout -`	| Muda para a última branch
`git checkout -- [nome-arquivo.txt]`	| Descarta modificações de um arquivo
`git merge [nome da branch]`	| Faz um merge de uma branch na branch atual
`git merge [source branch] [branch alvo]`	| Faz um merge de uma branch em outra branch
`git stash`	| Tirar o estado sujo do seu diretório de trabalho
`git stash clear`	| Remove todas as entradas 'stash'

### Sharing & Updating Projects
| Comando | Descrição |
| --- | --- |
`git push origin [nome da branch]`	| Enviar uma branch para seu repositório remoto
`git push -u origin [nome da branch]`	| Envia as alterações da branch informada para um repositório remoto (and selecionar a branch)
`git push`	| Envia as alterações para o repositório remoto (branch atual)
`git push origin --delete [nome da branch]`	| Deletar uma branch remota
`git pull`	| Atualiza o repositório da máquina com o último commit
`git pull origin [nome da branch]`	| Recebe alterações do repositório remoto
`git remote add origin ssh://git@github.com/[usuario]/[nome-repositorio].git`	| Adicionar um repositório remoto
`git remote set-url origin ssh://git@github.com/[usuario]/[nome-repositorio].git`	| Seta um repositório da origin branch para o SSH

### Inspeção & Comparação
| Comando | Descrição |
| --- | --- |
`git log`	| Ver modificações
`git log --summary`	| Ver modificações (detalhadas)
`git diff [branch original] [branch alvo]`	| Visualizar alterações antes de mesclar
</details>
