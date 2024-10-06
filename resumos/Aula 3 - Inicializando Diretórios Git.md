# Como Inicializar e Clonar Repositórios 
## Inicializando um repositório
Criando um diretório e inicializando-o como um repositório GIT
```bash
mkdir nome_diretorio && cd ./nome_diretorio
git init
```

Relacionando o repositório GIT à um repositório remoto no Github
```bash
cd nome_diretorio
git remote add origin https://www.github.com/<nome_user>/<nome_repo>
```

## Clonando um repositório
### Clonando via Token
```bash 
git clone https://www.github.com/<nome_user>/<nome_repo> <nome_local_opcional>
```
### Clonando via SSH
```bash
git clone git@github.com/vToshio/<nome_diretorio>.git
```
### Clonando uma Branch específica
Caso não ache espeficicação, ele clona a branch main por padrão
```bash
git clone <URL> --branch <nome_branch> --single-branch
```
## Verificando as configurações de um repositório

```bash
cat ./<nome_diretorio>/.git/config
```