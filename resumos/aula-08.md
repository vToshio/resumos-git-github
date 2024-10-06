# Comandos Úteis no Dia a Dia

## Fetch
> Baixa as alterações de um repositório remoto sem realizar a mesclagem com o repositório local

- git pull = git fetch + git merge

```bash
git fetch origin 
```

## Diff
> Indica as diferenças entre duas branches

```bash
git diff main origin/main
```

Indica as diferenças entre a branch main local e a branch main da origem (origin/main)

## Clonando uma Branch especifica

```bash
git clone <url-projeto> --branch <nome-branch> --single-branch
```

## Stash
> Arquiva uma alteração de uma branch que pode revertida posteriormente

- Utilizada caso você queira trabalhar em uma branch antes de efetivar uma modificação
- Stash --> arquiva a modificação e volta ao estado antes da modificação

```bash
git stash

git stash pop #trazer as alterações de volta e excluir a alteração mais recente
git stash apply #aplica a modificação para um uso posterior
```

## Estudo próprio
- [Documentação do Git](https://git-scm.com/docs)
- [E-Book Git](https://git-scm.com/book/en/v2)