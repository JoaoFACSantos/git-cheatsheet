# Branches

Uma branch é uma linha de desenvolvimento independente. Permite trabalhar numa funcionalidade ou correção sem mexer na `main`.

## Comandos essenciais

```bash
git branch                      # lista as branches locais
git branch -a                   # lista locais e remotas
git switch -c nome-da-branch    # cria e muda para uma branch nova
git switch main                 # volta à main
git branch -d nome-da-branch    # apaga uma branch já integrada
git branch -D nome-da-branch    # apaga mesmo sem estar integrada (cuidado)
```

## Juntar o trabalho

```bash
git switch main
git merge nome-da-branch        # integra a branch na main
```

Se houver conflitos, o git marca os ficheiros afetados. Resolve-os à mão, depois:

```bash
git add <ficheiro>
git commit                      # conclui o merge
```

## Convenção de nomes

- `feature/<descrição>` para funcionalidades novas
- `fix/<descrição>` para correções
- `docs/<descrição>` para documentação
