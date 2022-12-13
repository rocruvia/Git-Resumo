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
$	git add 		#Adiciona as modificações feitas no arquivo
$	git commit -m "Adicionar mensagem"
```
#### Logs
```
$		git log
$		git log --decorate
$		git log --author="Nome do Autor"
$		git shortlog 			     	#Versão resumida por autor
$		git log --graph			    #Mostra de forma gráfica os commits
$		git show hash_do_commit 	#Mostra as alterações daquele commit
```
