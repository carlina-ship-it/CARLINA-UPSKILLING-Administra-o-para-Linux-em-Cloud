# Validação do Serviço e Segurança - Tópico 04

## 1. Estado da Firewall
Após a aplicação das regras de segurança, a firewall (UFW) foi ativada com sucesso. O estado atual garante que apenas o tráfego estritamente nece>

* **Porta 22/TCP (SSH):** ALLOW IN (Permitido)
* **Porta 80/TCP (Nginx):** ALLOW IN (Permitido)
* **Todo o outro tráfego de entrada:** DENY IN (Bloqueado por padrão)

## 2. Validação do Serviço Web (Nginx)
Foi verificado que o servidor Nginx continua ativo e a responder corretamente na porta 80, confirmando que a ativação da firewall não interrompeu>

## 3. Lista de Evidências Disponíveis
As capturas de ecrã que comprovam a realização e validação desta atividade encontram-se na pasta `evidencias/`:
* `01-portas-ativas.png`: Output do comando `sudo ss -tulnpx` antes das alterações.
* `02-status-firewall.png`: Output do comando `sudo ufw status verbose` comprovando a proteção ativa.







