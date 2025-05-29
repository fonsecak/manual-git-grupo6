## Instalação e Configuração do Git

Tópicos que serão abordados:

○ Onde baixar e instalar (Windows, Linux, macOS) ○ Comandos de configuração: ■ git config --global user.name ■ git config --global user.email ■ git config --list ○ Checagem da instalação

# 🔹1. Onde baixar e instalar o Git?

🔸 Windows Acesse o site oficial: https://git-scm.com

Baixe o instalador para Windows.

Execute o instalador e siga os passos clicando em “Next”.

Pode deixar as opções padrão, que já funcionam bem para a maioria.

Após a instalação, você terá o Git instalado e também o "Git Bash", que é o terminal para usar comandos Git.
🔸 Linux (Ubuntu/Debian) Abra o terminal e digite o comando:

bash sudo apt update sudo apt install git Depois de instalado, você pode usar o Git direto no terminal.

🔸 macOS Você pode instalar via Homebrew (se tiver instalado): bash brew install git Ou baixar direto do site https://git-scm.com e instalar como no Windows.

# 🔹2. Comandos de configuração Depois de instalar o Git, você precisa dizer para ele quem você é, porque o Git registra o nome e e-mail em cada alteração que você fizer (commit). Isso é importante para o histórico do projeto.

No terminal (Git Bash no Windows ou terminal no Linux/macOS), digite: Para configurar seu nome:

bash git config --global user.name "Seu Nome" Para configurar seu e-mail:

bash git config --global user.email "seu.email@example.com" Para ver todas as configurações feitas:

bash git config --list O --global significa que essa configuração vale para todos os seus projetos no computador. Se quiser configurar só para um projeto específico, pode tirar o --global.

# 🔹3. Como checar se o Git está instalado corretamente? 

Abra o terminal (Git Bash no Windows ou terminal no Linux/macOS) e digite:

bash git --version