# Como configurar o Git?

## Escopos de configuração
- Global
	- Escopo que abrange todos os repositórios do usuário atual
- System
	- Escopo que abrange todos os usuários de sistema
- Local
	- Escopo referente às configurações do diretório local

## Config
> Variáveis de configurações do git

#### Obtendo o valor de uma variável
```bash
git config <nome_variavel>
git config --escopo --list
```
#### Configurando Variáveis básicas
```bash
git config --escopo user.name 'nome usuario'
git config --escopo user.email ''
git config --escopo init.defaultBranch main
```