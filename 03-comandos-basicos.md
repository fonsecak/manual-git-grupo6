# 03 - Comandos Básicos

## Iniciar um Repositório

Para começar a usar o Git em um projeto, você precisa criar um repositório (pasta do projeto).

`Git init`

Isso cria uma pasta oculta .git que armazena o histórico de versões.

## Verificar o Status do Repositório

exibe informações importantes e o status de seus arquivos.

`Git status`

## Adicionar Arquivos para "Stage" (Preparação)

Antes de salvar as alterações, você precisa adicioná-las a uma área de preparação (staging area).

`git add nome_do_arquivo.txt`

Para adicionar um arquivo que ainda não esteja colocado.

`Git add .`

Para adicionar todos que ainda não estejam colocados.

## Salvar Alterações (Commit)

Cria um "snapshot" (registro) das mudanças com uma mensagem descritiva.

`Git commit -m "Adicionar comentário"`

Mensagens claras ajudam a equipe a entender as mudanças.

## Visualizar o Histórico de Commits

Lista todos os commits feitos no repositório.

`Git log`

Permite visualizar uma lista cronológica do histórico de commits.