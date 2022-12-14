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
