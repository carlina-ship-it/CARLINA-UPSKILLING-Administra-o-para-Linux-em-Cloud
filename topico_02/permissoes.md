# Permissões aplicadas

## Ambiente utilizado
Máquina Virtual (VM) local configurada VM VirtualBox com o sistema operativo Ubuntu Linux.

## Utilizador e grupos
O utilizador pertence ao grupo principal do sistema e possui privilégios administrativos através do grupo 'sudo'.

## Ficheiros criados
- **publico.txt**: Ficheiro destinado ao acesso geral de leitura para utilizadores externos ou outros serviços.
- **restrito.txt**: Ficheiro com dados sensíveis que devem ser protegidos contra acessos não autorizados.
- **script.sh**: Script de automatização que necessita de privilégios de execução na consola.

## Permissões aplicadas

| Ficheiro | Permissão | Justificação |
|---|---:|---|
| publico.txt | 644 | O dono pode ler e escrever (6). O grupo e os outros utilizadores do sistema podem apenas ler (4), garantindo a integridade do ficheiro público. |
| restrito.txt | 640 | O dono pode ler e escrever (6) e o grupo pode apenas ler (4). Os outros utilizadores do sistema não têm qualquer acesso (0), protegendo a informação confidencial. |
| script.sh | u+x | Adiciona o bit de execução (+x) apenas para o utilizador dono (u). Evita que outros utilizadores corram o script sem autorização. |

## Relação com o princípio do menor privilégio
As permissões aplicadas cumprem rigorosamente o **Princípio do Menor Privilégio**. Em vez de atribuir permissões totais (como `777`), cada ficheiro recebeu apenas o acesso estritamente necessário para cumprir a sua função:
1. O ficheiro público não pode ser modificado por terceiros.
2. O ficheiro restrito fica completamente invisível para quem não pertence ao grupo de segurança.
3. O script só pode ser executado por quem o criou
