# Tutorial-Comandos-Staff

<h2> Primeira Etapa: Colocar o Resource no seu servidor</h2>

Coloque o resource RSC_Comandos_Staff no seu servidor logo após certificar que o mesmo esta aparecendo no Painel P
<img src='https://i.imgur.com/Xj3jjdz.png'>

Abra o F8 e de o comando 'debugscript 3' dessa forma:

<img src='https://i.imgur.com/ZFMvEio.png'>

Tem que aparecer no proprio F8 essa Mensagem:

<img src='https://i.imgur.com/lkLO88I.png'>

Irá Aparecer Algumas Mensagem de erros e avisos de scripts do seu servidor no centro de baixo da tela, ignore por enquanto

Após isso Devemos logar com nosso acesso na proteção, então inicie o script RSC_Loader e Logue com Seu Login e Senha da proteção:

<img src='https://i.imgur.com/zxuvWrM.png'>

Efetue o login e espere a mensagem de "Logado com Sucesso", Após isso devemos iniciar o Resource 'RSC_Comandos_Staff'

Espere o sistema verificar se tem alguma atualização, Caso essa Mensagem Apareça:

<img src='https://i.imgur.com/zWg3jkp.png'>

chat:
<img src='https://i.imgur.com/w07Y8Sq.png'>


Não se preocupe o nosso sistema de loader identifica e baixa atualizações mais recentes dos arquivos Server e Client, deixando seu resource sempre atualizado.

Espere o sistema atualiza.

<img src='https://i.imgur.com/t2x9UzX.png'>

Perceba que ele atualizou o Client dps o Server e automaticamente ja reiniciou o script que denovo buscou atualizações e nao achou e ai então iniciou o resource.

Devemos nos Atentar que após iniciar o script, tem que aparecer as mensagens na seguinte ordem, sem acusar nenhum erro.

<img src='https://i.imgur.com/ew8J9Y8.png'>

Pronto seu script esta iniciado.

<h2> Segunda Etapa: Configuração </h2>

Localiza a Pasta do RSC_Comandos_Staff o Arquivo RSC_Config.lua 

<img src='https://i.imgur.com/F93ul6S.png'>

Ao abri você vai colocar uma area que vai esta com o nome 'CargosComando = {'

<img src='https://i.imgur.com/nYRaM2b.png'>

Aqui você vai colocar todas os Groups Staff que entraram em horario.

obs: eles não precisam esta em nenhuma acl para conseguir entra, o objetivo desse script é justamente evitar que staff utilizem painel durante o RP normal e usar somente em horario

Após adicionar todas dessa forma:

Exemplo:
<img src='https://i.imgur.com/ntzXXDU.png'>

o Proximo que vai encontrar vai ser a area onde vai esta escrito 'CargosComandoVoar = {' Nessa Parte igual a de cima você vai colocar todos os groups que você quer que possa utilizar o comando voar

Exemplo:
<img src='https://i.imgur.com/RZCgMXU.png'>
Obs: isso é igual para todas as outras:
'CargosDarVida = {'
'ArrumarVeiculos = {'
'DestruirVeiculos = {'
'SetarColetes = {'
'SanarFomeESede = {'
'TeleportaAtePlayers = {'
'PuxarPlayers = {'
'FicarInvisivel = {'
'SetarGasolina = {'
'SetarSkins = {'

Após configurar todas temos a parte de chamados staff

<img src='https://i.imgur.com/XiQ3uMG.png'>

Nessa você coloca também todas as acls que receberam chamados de pedido de ajuda staff de player.

Nosso resource tem um sistema de comandos para identificar comandos de possiveis 'mod menu':

<img src='https://i.imgur.com/KPUOXv2.png'>

Nessa Parte temos o primiero local que é a mensagem que o jogador vai receber ao ser kikado do servidor

<img src='https://i.imgur.com/0ncTtff.png'>

Não são todos os comandos que daram kick nos jogadores você vai configurar mais pra frente

Aqui são os comandos padrão que o script vai ignora e não ira fazer nada caso alguem de esse comando (ele so nao vai da kick, manda log no dc, etc o comando ainda ira funcionar)

<img src='https://i.imgur.com/PROCHXG.png'>

Agora Temos os comandos que são proibidos digamos assim, aqui vamos coloca da seguinte forma:

<img src='https://i.imgur.com/svPE7n1.png'>

sendo: {"Comando",sim ou nao} - caso coloque sim o jogador ao dar esse comando ira ser kikado, caso coloque nao o jogador nao sera kikado do servidor.

aconselho que nessa parte deixe os comandos que ja vem no script e so adicione mais, os comandos ja existentes nele são de mods menus que ja existem evitando assim que burlem o sistema do seu servidor

Terminando essa Parte entramos no Config do script em geral

a Primeira parte é o comando de entrar e sair de horario

<img src='https://i.imgur.com/604iiUN.png'>

o comando é o mesmo pra todos, sendo o primeiro o de entrar e o segundo de Sair, você pode mudar.

logo apos temos a configuração do painel Staff

<img src='https://i.imgur.com/EtzAXQ6.png'>

Aqui você configura o comando para abrir o painel e a Acl que poderá abrir e gerenciar

ao dar esse comando ira abrir esse painel:

<img src='https://i.imgur.com/vmQ4m4u.png'>

é nele que você vai dar permissão para o jogador da o comando de entrar e sair selecionando o jogador do lado esquerdo e o Group do lado direito que ele vai entra.

continuando logo a baixo temos a configuração do painel comandos:

<img src='https://i.imgur.com/YzH5hut.png'>

o sendo {"Comando Abrir Painel","ACL que vai poder Abrir"},

ao dar esse comando vai abrir o painel de comandos:

<img src='https://i.imgur.com/s8SdnGP.png'>

Esse painel irá mostrar todos os scripts que tem comandos neles e qual comandos tem, Obs: esse painel foi criado pelo simples fato de ja ter encontrado mais de 70 comandos dentro de uma skin de personagem
essa skin contia um mod menu dentro dela!

Então utilizem ele vale muito a pena

Logo em seguida temos a configuração de logs:

<img src='https://i.imgur.com/YzH5hut.png'>

Logo no mesmo temos essa area onde voce vai colocar sim para os que você quer que envie logs no servidor discord configurado a cima e nao para os que você nao quer que envie

<img src='https://i.imgur.com/aiSZjsK.png'>

As Logs apareceram assim no discord:

<img src='https://i.imgur.com/w1UdQMP.png'>

Logo abaixo temos a configuração do Element Data do ID, se seu servidor utiliza Custom Personagem, e A Sigla nome do servidor que vai aparecer quando o staff entra em horario

<img src='https://i.imgur.com/GnV0AQv.png'>

Caso seu servidor não utilize Custom basta colocar '["CustomSkin"] = {nao, 1},' caso possuia deixe sim e coloque do lado o id principal da custom

Lodo depois temos a parte de cobrança por alguns comando (essa parte foi pedida por alguns clientes):

<img src='https://i.imgur.com/N1TA19y.png'>

Aqui é basicamente:
["vida"] = {CAso queira que o comando cobre coloque sim caso nao coloque nao, Valor cobrado},

na parte '["AclInsentas"] = {' você coloca as acls que mesmo com o sim na parte acima não serão cobradas o valor.

<img src='https://i.imgur.com/g3L6aRw.png'>

E Por ultimo temos os comandos:

<img src='https://i.imgur.com/816Mw3Q.png'>

Aqui você Poderá mudar os comandos do jeito que preferir

e é isso com isso basta utilizar o resource e pronto esta tudo configurado ^^


