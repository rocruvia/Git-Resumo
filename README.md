

## Resumo Git
Esse repositório tem o obejetivo de ser uma fonte rápida de revisão dos principais comandos Git.
#### Configurações Iniciais Git
```git
$   git config -- global user.name <Seu nome>
$   git config --global user.email <Seu email>
$   git config user.name
$   git config user.email
```
#### Iniciando o repositório
```git
$   git init
```
#### Salvando e fazendo commit
```
$   git status

#Adiciona as modificações feitas no arquivo / move o arquivos para o staging
$   git add <Nome do arquivo>

#Adiciona as modificações feitas em todos os arquivo
$   git add .
$   git commit -m <Adicionar mensagem>
```
#### Logs
```
$   git log
$   git log --decorate
$   git log --author=<Nome do Autor>

# Versão resumida por autor
$   git shortlog 	

# Mostra de forma gráfica os commits
$   git log --graph

# Mostra as alterações daquele commit
$   git show <hash do commit>
```
#### Comparação de mudanças
``` git
$   git diff

# Mostra apenas os nomes dos arquivos modificados
$   git diff -name-only
```
#### Desfazendo mudanças
``` git
# Retorna a versão anterior (não pode estar no stage)
$   git checkout <Nome do arquivo>

# Retira o arquivo do stage
$   git reset <nome do arquivo>

# Retorna para o status stage
$   git reset --soft <Hash do commit>

# Retorna para o status antes do stage
$   git reset --mixed <Hash do commit>

# Desfaz TODAS as modificações
$   git reset --hard <Hash do commit>
```
#### Conectando o repositório local ao remoto
```git
$   git remote add origin <Link do repositório>

# Normalmente o repositório remoto será origin e a branch main/master
$   git push <repositório remoto> <Sua branch>
```
#### Clonando repositórios
```git
$   git clone <Link do repositório>
```
#### Branch
```git
# Criando uma branch
$   git checkout -b <Nome da branch>

# Visualizando as branchs existentes
$   git branch

# Mudando de banch
$   git  checkout <Nome da branch>

# Deletando uma banch
$   git banch -D <Nome da branch>
```

#### Merge e Rebase
```git
# Cria um commit extra e fecha o "ciclo"
$   git merge <Nome da branch com que será feito o merge>

# Não cria um commit extra e lineariza a junção
$   git rebase <Nome da branch com que será feito o merge>
```

#### Tags
```git
# Marca os realeases / versões do código
$   git tag -a <1.0.0(exemplo)> -m <Mensagem>

$   git push origin master --tags

# Visualização das tags
$   git tag

# Apagar tags
$   git tag -d <Nome da tag>
$   git push origin :<Nome da tag>
```

#### Revert
```git
# Desfaz as mudanças sem alter o histórico dos commits
$   git revert <Hash do commit>
```

