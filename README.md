# git-cheatsheet

Resumo pessoal dos comandos git que uso no dia a dia, organizado por tarefa.

## Configuração inicial

```bash
git config --global user.name "O teu nome"
git config --global user.email "o-teu-email@exemplo.com"
git config --global init.defaultBranch main
```

## Começar um repositório

```bash
git init                    # cria um repositório novo na pasta atual
git clone <url>             # copia um repositório remoto
```

## Ciclo básico

```bash
git status                  # estado dos ficheiros
git add <ficheiro>          # prepara um ficheiro para commit
git commit -m "mensagem"    # guarda as alterações preparadas
git push                    # envia os commits para o remoto
git pull                    # traz e junta as alterações do remoto
```

## Estrutura

- `README.md`: esta página, com o essencial
- Mais secções (branches, desfazer alterações, stash, etc.) vão sendo adicionadas por pull request
