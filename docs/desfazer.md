# Desfazer alterações

Qual comando usar depende de onde está a alteração.

## Ainda não fiz commit

```bash
git restore <ficheiro>          # descarta alterações no ficheiro
git restore --staged <ficheiro> # tira o ficheiro da área de preparação (mantém as alterações)
```

## Já fiz commit, mas ainda não fiz push

```bash
git commit --amend              # corrige a mensagem ou junta ficheiros ao último commit
git reset --soft HEAD~1         # desfaz o último commit, mantém as alterações preparadas
git reset --hard HEAD~1         # desfaz o último commit e apaga as alterações (cuidado)
```

## Já fiz push

Não reescrevas o histórico partilhado. Usa `revert`, que cria um commit novo a anular outro:

```bash
git revert <hash-do-commit>
```

## Encontrar algo perdido

```bash
git reflog                      # histórico de tudo o que o HEAD já apontou
git switch -c recuperada <hash> # recupera um estado antigo numa branch nova
```
