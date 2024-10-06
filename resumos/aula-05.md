# Desfazendo Alterações no Respositório Local

## Git log e Git reflog
> Acesso ao log de commits realizados

Git log --> commits efetuados e não alterados
Git reflog --> todos commits efetuados, inclusive os que sofreram reset
## Restore
> Restaurar um arquivo à última versão salva em um commit

```bash
git restore <nome-arquivo>
```

## Alterar Mensagem do último commit

```bash
git commit --ammend -m'nova mensagem'
```
Obs: esse comando altera somente a mensagem do último commit submetido, e caso seja passado sem o parâmetro -m, ele abrirá o editor de texto e possibilitará a alteração de todos os dados manualmente.
## Reset 
> Comando git utilizado para remover arquivos staging area ou para reverter commits
### Remover Arquivos da Staging Area

```bash
git reset <nome-arquivo>
```
### Remover Commits
Primeiramente, deve-se obter o hash do commit cujo o qual você queira realizar a alteração de mensagem, por meio do [git log]().

Com o endereço hash em do commit em mãos, utilizar o comando:

```bash
git reset --<tipo> [endereco-hash]
```
#### Soft
> Adicionar os arquivos posteriores ao commit específicado à staging area
#### Mixed
> Adiciona os arquivos posteriores ao commit especificado na árvore como "untracked files" (ainda não reconhecidos na staging area)
#### Hard
> Remove completamente o commit e desfaz todos os arquivos posteriores à ele