
# Monitorização do Sistema

## Tempo de atividade

Foi utilizado o comando:
uptime up 7:33, 1 user, load average: 0.01, 0.03, 0.02

## Memória
para ver a memoria foi utilizado o comando:

free -h : Total: 4.2Gi Usada: 1.4Gi Livre: 561Mi Disponível: 2.9gi

## Espaço em Disco
Foi utilizado o comando:df -h
Filesystem      Size  Used Avail Use% Mounted on
tmpfs           871M  3.3M  867M   1% /run
/dev/sda2        25G  7.0G   17G  31% /
tmpfs           2.2G     0  2.2G   0% /dev/shm
tmpfs           2.2G  7.6M  2.2G   1% /tmp
none            1.0M     0  1.0M   0% /run/credentials/systemd-journald.service
none            1.0M     0  1.0M   0% /run/credentials/systemd-resolved.service
tmpfs           436M   88K  435M   1% /run/user/1000

## Estado do Serviço Web
Foi utilizado o comando:systemctl status nginx

