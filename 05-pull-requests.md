GitHub e Pull Requests – Guia para Iniciantes

---

## 1. Criar conta no GitHub
Acesse o site: https://github.com

Clique em Sign up (ou Cadastre-se).

Preencha seu nome de usuário, e-mail e senha.

Confirme seu e-mail através do link que o GitHub enviará para você.

Pronto! Conta criada e já pode começar a usar.

## 2. Criar um repositório remoto no GitHub
Acesse seu GitHub e clique no botão verde “New” ou “Novo repositório”.

Dê um nome para seu repositório (ex.: meu-projeto).

Opcional: pode adicionar uma descrição.

Escolha se será público (qualquer um pode ver) ou privado (só você e quem você permitir).

Pode marcar a opção “Add a README file” se quiser começar com um arquivo inicial.

Clique em Create repository.

Pronto! Seu repositório remoto está criado na nuvem.

## 3. Clonar, Push e Pull
:arrow_down_small: Clonar (Clone) – Baixar o repositório para seu computador
No GitHub, clique no botão verde “Code”, copie o link (HTTPS ou SSH).
No terminal, digite:

bash

git clone https://github.com/seu-usuario/seu-repositorio.git

Isso cria uma cópia do repositório na sua máquina.

:arrow_up_small: Push – Enviar arquivos para o GitHub (subir mudanças)
Depois de fazer alterações, salvar e fazer commit, envie para o GitHub com:

bash

git push

O push envia as alterações do seu computador para o repositório remoto no GitHub.

:arrows_counterclockwise: Pull – Baixar as últimas atualizações do GitHub para seu computador
Se outra pessoa (ou até você mesmo de outro PC) fez alterações no GitHub, use:

bash

git pull

O pull baixa as atualizações do repositório remoto para seu repositório local.


## 4. Pull Requests e Revisão de Código

 O que é um Pull Request (PR)?

É uma solicitação para que suas alterações sejam adicionadas no código principal do projeto.

Serve para revisão, discussão e aprovação do código antes de juntá-lo na branch principal (geralmente main ou master).

 Como funciona na prática:

Crie uma nova branch no seu projeto para uma nova funcionalidade ou correção.

Faça commits normalmente nessa branch.

No GitHub, clique em “Compare & pull request” ou vá na aba Pull Requests e clique em New Pull Request.

Descreva o que você alterou.

Envie o PR para que outra pessoa revise (ou você mesmo, em projetos próprios).

Após aprovado, o código pode ser mesclado (merged) na branch principal.


Para que serve?

Revisar código antes de integrar.

Discutir melhorias, sugerir alterações e evitar erros.

Ótimo para projetos em equipe ou colaborativos.
