# Realizando Alterações em um Diretório Git

## Status
> Verificar arquivos de um diretório.

```bash
git status 
```

O comando git status **realiza a verificação dos arquivos presentes** no diretório git atual, exibindo o **status dos seus arquivos**.

Obs: o Git **não reconhece** diretórios vazios. 
- Necessário adicionar arquivos dentro do diretório para que ele possa ser reconhecido
- Convenção --> arquivo .gitkeep utilizado para uma pasta vazia ser incluída em um commit

## Add
> Adicionar um arquivo ao próximo commit.

```bash
git add <nome-arquivo>
```

O arquivo em questão é adicionado à uma "área de preparação" antes de ser inserida em um commit.
## Commit
> Efetivar as alterações em um diretório Git
```bash
git commit -m"mensagem"
```

## O que é o arquivo .gitignore?

São arquivos a serem ignorados dentro de uma área de preparação, evitando que arquivos indesejados sejam inclusos dentro de um commit.

Adicionando arquivos ao .gitignore
```bash
echo <arquivo(s)> > .gitignore  
```