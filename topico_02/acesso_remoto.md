# Acesso remoto por SSH

## O que é SSH?
O SSH  é um protocolo de rede cifrado utilizado para aceder e gerir servidores Linux de forma remota e segura através do terminal.
## Informaçoes  necessários para aceder a um servidor por SSH
Para estabelecer uma ligação com sucesso a um servidor remoto, são necessários os seguintes dados:
- **Utilizador:** O nome da conta de sistema que vamos aceder no servidor (ex:ubuntu).
- **Endereço IP:** O endereço de rede único do servidor (ex: `192.168.1.50` ou um domínio público).
- **Porta:** Por padrão, o SSH utiliza a porta tcp **22**. Por motivos de segurança, esta porta é frequentemente alterada em servidores de produção.
- **Palavra-passe ou chave:** Um método de autenticação. 
## Exemplo de comando de ligação
ssh utilizador@endereco_ip -p 22
