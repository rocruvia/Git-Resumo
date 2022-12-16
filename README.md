## Resumo Git
Esse repositório tem o obejetivo de ser uma fonte rápida de revisão dos principais comandos Git.
#### Configurações Iniciais Git
```git
$	git config -- global user.name "Meu Nome"
$	git config --global user.email "Meu Email"
$	git config user.name
$	git config user.email
```
#### Iniciando o repositório
```git
$	git init
```
#### Salvando e fazendo commit
```
$	git status
#Adiciona as modificações feitas no arquivo
$	git add nomed_do_arquivo		
#Adiciona as modificações feitas em todos os arquivo
$	git add .
$	git commit -m "Adicionar mensagem"
```
#### Logs
```
$	git log
$	git log --decorate
$	git log --author="Nome do Autor"
# Versão resumida por autor
$	git shortlog 	
# Mostra de forma gráfica os commits
$	git log --graph
# Mostra as alterações daquele commit
$	git show hash_do_commit 	
```
#### Comparação de mudanças
``` git
$	git diff
# Mostra apenas os nomes dos arquivos modificados
$	git diff -name-only
```
#### Desfazendo mudanças
``` git
# Retorna a versão anterior (não pode estar no stage)
$	git checkout nome_do_arquivo
# Retira o arquivo do stage
$ 	git reset nome_do_arquivo
# Retorna para o status stage
$	git reset --soft hash_do_commit
# Retorna para o status antes do stage
$	git reset --mixed hash_do_commit
# Desfaz TODAS as modificações
$	git reset --hard hash_do_commit
```
#### Conectando o repositório local ao remoto
```git
$	git remote add origin link_do_repositório
# Normalmente o repositório remoto será origin e a branch main/master
$	git push <repositório_remoto> <sua_branch>
```
