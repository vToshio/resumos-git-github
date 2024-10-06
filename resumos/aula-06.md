# Enviando Alterações para um Repositório Remoto

## Conectando ao Repositório Remoto

```bash
git remote add origin <url-diretorio>
git branch -M main
```
O comando adicional 'git branch' server para especificar qual branch do diretório receberá as alterações realizadas pelo usuário
## Push
> Empurra as alterações do respositório remoto para o repositório local

```bash
git push -u origin main
```

- Parâmetro -u: setupstream
	- Configurar a branch main do repositório remoto (especificada como origin) com a branch upstream main do repositório local
## Pull
> Puxa as alterações realizadas dentro de um repositório no Github para o repositório local, mantendo-os "sincronizados"

```bash
git pull
```