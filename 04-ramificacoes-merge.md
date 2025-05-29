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

---

# git merge e Conflitos

 O que é git merge?

Merge é o processo de juntar as alterações de um branch em outro (geralmente no main).

---

##  Como fazer um merge?

Vá para o branch que receberá as alterações (ex.: main):

`git checkout main`

---

## Conflitos no Merge
Ocorrem quando há mudanças conflitantes no mesmo arquivo ou linha entre os branches.



---
 
## Como resolver:

Edite o arquivo, escolha o código correto e remova as marcações.

Salve o arquivo.

Adicione as alterações:
git add nome-do-arquivo

Finalize o merge com um commit:
git commit -m "Resolve conflitos no merge"

---

## Demonstração Passo a Passo
Criar um branch e fazer alterações:

git checkout -b feature/login                  

git add .

git commit -m "Adiciona batata"

---

## Voltar para main e fazer o merge:

git checkout main
git merge feature/login

---

## Se houver conflito:

Abra o arquivo com conflito.

Corrija o código, salve e depois execute:

 git add .
 git commit -m "Resolve conflitos no merge"

---
## Resumo Visual do Processo

 main:          A -- B -- C
                         \
feature/login:            D -- E

Após o merge:

main:          A -- B -- C -- F (merge das alterações de E)
feature/login:            D -- E



 








