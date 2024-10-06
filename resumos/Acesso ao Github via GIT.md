# Acessando o Github via Git

## Token
- Gerar token
- Salvar o token (não solicitar acesso quando utilizá-lo novamente)
	- git config --global credential.helper store
	- local armazenado:
		- git config --global --show-origin \<nome-da-variavel-buscada>
- Fazer login com o Token

## SSH (Secure Shell)
- Protocolo de rede que possibilita que um host se conecte a outro de forma segura e criptografada por meio da internet
- Chave pública e chave privada
	- Chave privada = senha
	- Chave pública --> inserida no github

## Criando novas chaves SSH


```bash
$ ssh-keygen -t ed25519 -C "seu_email@email.com"

$ eval "$(ssh-agent -s)"

$ ssh-add ~/.ssh/id_ed25519
```