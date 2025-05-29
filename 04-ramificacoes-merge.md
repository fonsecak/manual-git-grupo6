# Branches e Merge no Git

## O que são Branches?

Branch (ramo) é uma linha separada de desenvolvimento dentro do mesmo projeto.

O branch principal geralmente se chama main ou master.

Você pode criar branches para desenvolver novas funcionalidades sem mexer no código principal.

Exemplo:

main → Código estável (versão que está funcionando).

feature/login → Branch para desenvolver um sistema de login.

## Criar, Mudar e Deletar Branches

Criar um novo branch

`git checkout -b nome-do-branch`  

Cria e muda para o branch

## Ver todos os branches

`git branch`

## Mudar de branch

`git checkout nome-do-branch`

## Deletar um branch

`git branch -d nome-do-branch`

# git merge e Conflitos

## O que é git merge?

Merge é o processo de juntar as alterações de um branch em outro (geralmente no main).

## Como fazer um merge?

Vá para o branch que receberá as alterações (ex.: main):

`git checkout main`

# Conflitos e como resolver

Conflito acontece quando o Git não consegue juntar automaticamente as mudanças (ex.: duas pessoas alteram a mesma linha).


## Passos para resolver:
O Git marca os conflitos no arquivo:

<<<<<<< HEAD  
Seu código atual  
=======  
Código do branch que está sendo mesclado  
>>>>>>> feature/login  
Edite o arquivo, removendo as marcações (<<<<<<<, =======, >>>>>>>) e deixando o código correto.

Salve e adicione as alterações:


`git add nome-do-arquivo`

Finalize o merge:

git commit

## Demonstração Passo a Passo

1. Criando um branch e fazendo alterações
bash

git checkout -b feature/login 

## Faça alterações nos arquivos...

git add .

`git commit -m "Adiciona sistema de login"`

2. Voltando para main e mesclando

git checkout main

git merge feature/login

3. Se houver conflito:

Abra o arquivo com conflito, corrija e salve.

Depois:

git add .

git commit -m "Resolve conflitos no merge"

# Resumo Visual
main: A -- B -- C  
            \  
feature/login: D -- E  
Depois do git merge:

main: A -- B -- C -- F (merge de E)  
feature/login: D -- E  