# Manipulando Branches

## O que é uma Branch?

Branch = ramificação do seu projeto.

- Ponteiro móvel para um commit no histórico do repositório 
- Criação de uma nova Branch a partir de outra existente, a nova se inicia apontando para o mesmo commit da Branch que estava quando foi criada
	- Possibilita o **trabalho independente**, que pode ser mesclado posteriormente

# Branch
> Comando utilizado para listar todas as branches de um projeto git

```bash
git branch 
```

## Criando uma nova Branch

```bash
git checkout -b <nome-branch>
```

Todo commit realizado dentro de uma nova branch, ocorre apenas dentro dessa nova branch.
Em caso de mudança para a branch main, por exemplo, todas as alterações feitas dentro da branch \<nome-branch> seriam "deletadas", visto que ainda não foram mescladas à branch principal.

## Removendo uma branch

```bash
git branch -d <nome-branch>
```
Parâmetro "delete", que deleta uma branch determinada.
## Mesclando Branches

```bash
git merge <nome-branch>
```
Mescla a branche atual com outra, de nome determinado.

## Conflitos de Merge
> Alterações concorrentes
- Duas pessoas, trabalhando no mesmo código, realizam alterações em uma mesma linha de código
- Conflito --> Git não entende qual alteração ele deve manter