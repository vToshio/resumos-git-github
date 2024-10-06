# O que é versionamento de Código?
- Controle de versão de um arquivo ao longo do tempo 
- Histórico detalhado de atualizações de um arquivo
	- Quem alterou, data, quantidade de alterações em comparação com a versão anterior, etc...

## Sistemas de Controle de Versão (VCS)
### CVCS (Centralized)
> Um servidor contém todos os arquivos responsáveis pelo sistema de controle de versão

- Todos os usuários conectados à um mesmo servidor VCS
- Área de trabalho compartilhada
- Desvantagem --> perca de dados
	- Não é possível salvar e recuperar arquivos caso o sistema esteja fora

### DVCS (Distributed)
> Contém uma cópia local dos arquivos do servidor de versionamento

- Clona o repositório completo --> clone = backup
- Evita a perda de dados, visto que as alterações realizadas localmente serão alteradas assim que o host estiver conectado novamente com a rede, e a mudança será permanente para todos os colaboradores
