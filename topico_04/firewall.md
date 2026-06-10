                                                         
configuração da Firewall (UFW) - Tópico 04

## 1. Estratégia de Firewall
A estratégia adotada segue o princípio do privilégio mínimo: bloquear todo o tráfego de entrada por padrão (Default Deny) e permitir apenas os se>

## 2. Regras a Aplicar
Para garantir o funcionamento seguro do servidor Web, foram planeadas as seguintes regras no UFW:

* **Bloquear entradas por padrão:** `sudo ufw default deny incoming`
* **Permitir saídas por padrão:** `sudo ufw default allow outgoing`
* **Permitir SSH (Porta 22):** `sudo ufw allow 22/tcp` (Acesso para administração)
* **Permitir Nginx (Porta 80):** `sudo ufw allow 80/tcp` (Acesso público ao site)

## 3. Comandos de Ativação
```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw allow 22/tcp
sudo ufw allow 80/tcp
sudo ufw enable



