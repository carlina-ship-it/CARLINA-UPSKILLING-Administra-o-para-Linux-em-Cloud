
# Superfície de Ataque - Tópico 04

## 1. Identificação do Serviço Web
* **Serviço Utilizado:** Nginx Web Server
* **Versão:** (nginx version: nginx/1.28.3 (Ubuntu)

## 2. Serviços Ativos e Portas Abertas
Com base na análise efetuada com o comando `sudo ss -tulnpx`, foram identificados os seguintes serviços em estado LISTEN:

| Serviço | Porta | Protocolo | Estado | Necessário? | Justificação |
| SSH (sshd) | 22 | TCP | LISTEN | Sim | Para administração remota do servidor. |
| Nginx | 80 | TCP | LISTEN | Sim | Para servir a página web configurada no Tópico 3. |

## 3. Análise de Portas Necessárias
As únicas portas que necessitam de estar expostas para o exterior são>
**80** (públicas para acesso ao site)
 **22** (restrita para administração). Quaisquer outras portas detetadas que não tenham utilidade direta devem ser fechadas para reduzir a superf>

## 4. Identificação de Riscos Iniciais
1. **Firewall Desativada (UFW Inactive):** Sem regras ativas, qualquer novo serviço ou porto aberto fica exposto imediatamente à rede.
2. **Exposição Global da Porta SSH (22):** Se o SSH aceitar ligações de qualquer endereço IP, o servidor fica vulnerável a ataques automatizados.
3. **Comunicação em Texto Limpo (HTTP / Porta 80):** Os dados trafegam sem cifrar, permitindo a interceção de informações


