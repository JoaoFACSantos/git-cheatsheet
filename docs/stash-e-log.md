# Stash e histórico

## Stash: guardar trabalho a meio

Útil quando precisas de mudar de branch mas ainda não queres fazer commit.

```bash
git stash                       # guarda as alterações e limpa a pasta de trabalho
git stash push -m "descrição"   # igual, com nome
git stash list                  # lista os stashes
git stash pop                   # recupera o último e remove-o da lista
git stash apply                 # recupera o último e mantém-no na lista
git stash drop                  # apaga o último
```

## Ver o histórico

```bash
git log --oneline               # uma linha por commit
git log --oneline --graph --all # com o gráfico das branches
git log -p <ficheiro>           # alterações de um ficheiro ao longo do tempo
git show <hash>                 # detalhe de um commit
git diff                        # alterações ainda não preparadas
git diff --staged               # alterações já preparadas
git blame <ficheiro>            # quem alterou cada linha
```
