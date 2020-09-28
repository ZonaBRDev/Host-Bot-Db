# Preparamento - DBD

Utilizaremos o aplicativo "DBD" Discord Bot Designer.

``
Tipo de Linguagem
``
BD Script - Estável/Instável | Java Script

```
Chaves principais de utilizações | BD Script
```
.
``
$onJoined[ID de Canal] - Gatilho - Faça um comando de entrada
``
- - - 

Maneira simples de criar um set join (BD Script)

**Gatilho:** (Prefixo)setjoin
**Bloco de texto:**
``$nomention
$title[Canal de Entrada Alterada]
$description[Novas Mensagens de Entrada Aparecera aqui!]
$footer[Comando executado por $username]
$setServerVar[IDCanal;$message]``

\\\ O comando funcionará assim: !setjoin <Cole a ID do Canal>
\\\ Agora para as mensagens aparecerem:


**Gatilho:** ``$onJoined[$getServerVar[IDCanal]]``
**Bloco de texto:**
``$title[Novo usuário!]
$description[Temos um novo usuário! $username, Bem vindo, leia as regras!]
$footer[Temos agora $membersCount membros no servidor]
``

\\\ Antes de executar os comandos é deixar tudo perfeito 
\\\ Crie uma variável: IDCanal > Value: 0

Este é uma simples configuração de entrada para o DBD


