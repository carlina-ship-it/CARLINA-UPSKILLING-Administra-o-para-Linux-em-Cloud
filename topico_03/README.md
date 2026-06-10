
# Atividade prática individual - Tópico 3

## Nível realizado
Nível 1 (Essencial)

## Objetivo
Criar e publicar um serviço na web em ambiente Linux, estruturando uma página HTML inicial para uma loja de produtos tradicionais de Cabo Verde e configurando o servidor HTTP para a disponibilizar localmente.

## Ambiente utilizado
VM local (Ubuntu Linux)

## Rota de publicação
Nginx

## Ficheiros criados
* `index.html` (Página principal da loja "Sodade - Sabores & Arte de Cabo Verde")
* `publicacao.md` (Documentação do processo de publicação)
* `validacao.md` (Documentação dos testes de validação do serviço)
* `TP04INDIVIDUAL.pdf` (Ficheiros do relatório unificado)

## URLs testados
* `http://localhost`
* `http://127.0.0.1
* Hostname -I
* 10.0.2.15 


## Evidências produzidas
* Cabeçalho de resposta HTTP obtido através do comando `curl -I http://localhost` devolvendo o estado `HTTP/1.1 200 OK`.
* Captura de ecrã (print screen) do navegador Firefox exibindo a página da loja online a funcionar corretamente através do endereço local.
* Ficheiro `relatorio_final.pdf` gerado via terminal através do Pandoc.

## Dificuldades encontradas
A principal limitação prendeu-se com a necessidade de gestão de permissões administrativas no ecossistema Linux, obrigando à utilização do comando `sudo` para conseguir transferir o ficheiro `index.html` para a diretoria protegida do sistema (`/var/www/html/`).

## Link do repositório GitHub
[Inserir o link do seu repositório aqui, ex: https://github.com]
