Trabalho pratico 
Individual topico 02
Modulo linux e segurança cloud : Gestão de Identidades, Permissões e Acesso Remoto Seguro 
Ambiente de Trabalho: Utilização do hipervisor Oracle VM VirtualBox executado no Ubuntu Linux, acedida localmente via Terminal.

Comandos de Auditoria: 
Execução de comandos estruturais e de identificação como
cd, mkdir, touch, whoami (identificar utilizador ativo);
id  e groups (verificação de pertença ao grupo sudo) ;

Gestão de Permissões
(chmod): Criação de ficheiros de teste na pasta pasta_teste com atribuição de diferentes máscaras
publico.txt com 644 (rw-r--r--): Leitura/escrita para o dono, apenas leitura para grupo/outros 
restrito.txt com 640 (rw-r-----): Leitura/escrita para o dono, apenas leitura para o grupo, sem acesso para terceiros 
script.sh com u+x (-rwx------*): Execução restrita exclusivamente ao proprietário para cumprir o Princípio do Menor Privilégio.
Acesso Remoto (SSH): Revisão teórica do protocolo Secure Shell. 

Identificou uma limitação prática em que o teste de ligação externa falhou devido ao isolamento de rede padrão do VirtualBox (NAT sem port forwarding) e à falta do serviço openssh-server .
