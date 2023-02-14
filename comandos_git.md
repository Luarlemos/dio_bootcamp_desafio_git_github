# Comandos Git

## WorkFlow

1. Criar um arquivo
2. Salvar o arquivo
3. Editar o arquivo
4. Salvar de novo

Precisa escolher a pasta que quer atualizar as versões

## Comandos

- Esse comando faz com que o git tenha um repositório dentro da pasta e esse repositório vai ser responsável por controlar as versões da pasta

git init

- Mostra se os arquivos adicionados estão preparados ou não ou se já foram preparados para serem comitados.
 
git status

- Prepara o arquivo específico pra ser salvo dentro do git

git add nome_do_arquivo

- Prepara todos os arquivos para serem salvos

git add .

- Esses comandos permitem realizar o commit dos arquivos.

git commit --message "pq o arquivo foi alterado? Iniciando o versionamento de alguns arquivos"
 
ou

git commit -m ""

ou

git commit --message "iniciando o versionamento dos outros arquivos"

- Remove a pasta git, sendo deixada de ser controlada

rm -r .git 

- Mostra qual e a diferenca entre o repositório remoto no github e o local na minha máquina

git diff nome_do_arquivo
    
- Verifica o nome e o email da pessoa q fez aquela versão 

git log

- Configurar nome e email:

git config --global user.name "Nome do usuário"

git config --global user.email "email@gmail.com"

- Criar novo arquivo no terminal

touch

- Criar nova branch

git branch nome_da_branch

ou 

git checkout -b nome_da_branch

- Voltar para a branch main

git checkout main

- Troca de branch

git checkout

- Lista todas as branchs inclusive a main

git branch

- Consegue ver quais as diferencas entre a branch atual e a main

git diff main..nome_da_branch    

- Comando para no final do projeto transferir o arquivo atualizado da branch para a main

git merge --no-ff nome_da_branch

- Deleta a branch

git branch -d nome_da_branch_vazia

## GITHUB
No site clicar em:
* New repository
* Nome do repositório
* Criar repositório

- Clonar um repositório já existente no github

git clone https://github.com/repositorio 

- Como conectar pasta do git com repositório remoto do github

git remote add origin link_do_repositorio

- Comando q vê os repositorios remotos linkados com esse git no pc

git remote -v

- Enviar o código para o repositório remoto

git push origin nome_da_branch

- Desconecta do git remoto

git remote remove origin

ou

git remote -v

- Reverter commit

git reset

- Pega as atualizacoes feitas no github que no meu pc não tem

git pull origin main

- Checa as diferenças entre a main no pc e a main remota no github

git diff main..origin/main
