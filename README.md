# tibia001
Criando um servidor

Primeiro de tudo -> Baixe um Otserv que você irá usar no seu servidor.

Depois de ter baixado o Otserv -> Você irá ajeita-lo do seu gosto, editando\criando um mapa, editando\criando as spells, editando a aparência dos monsters, etc.

Após ter ajeitado o server -> Você irá salvar tudo no local certo ( mapa -> pasta World | Monsters -> pasta Monster | Spells -> pasta Spells | e assim vai ).

Depois de ter feito o procedimento anterior -> Pronto. Agora você irá colocar seu Servidor Online.

Colocando um Servidor Online

Primeiro de tudo -> Você irá desbloquear a porta 7171 ( Aconselhável está utilizando Windows XP, Internet individual & ServicePack 2).

Desbloqueando a porta 7171:

1º) Vá em Iniciar > Configurações > Painel de Controle.
2º) Abra ícone com nome de Firewall do Windows, vá em Exceções, Adicionar Porta. Em Nome você põe Open Tibia Server, em Número da Porta você põe 7171, deixe marcado TCP ( se nao tiver, marque ) e click OK. Pronto, porta 7171 desbloqueada.

*Obs: Não encontrou o Firewall do Windows no Painel de Controle? Tente assim:

1º) Vá em Iniciar > Configurações > Painel de Controle
2º) Abra o ícone com o nome de Opções da Internet, vá em Conexões, click na opção Configurações… ( que se encontra em baixo do botão Remover ).
3º) Após isso, click na opção Propriedades e na janela que se abrirá click em Avançado. No inferior do lado direito tem um botão chamado de Configurações…. Click. Vá em Adicionar Porta ( em alguns computadores tem somente Adicionar ). Em Número da Porta você põe 7171, deixe marcado TCP ( se nao tiver, marque ) e click OK. Pronto, porta 7171 desbloqueada.

Configurando o Ip:
1º) Acesse o site http://www.meuip.com.br e copie seu IP.
2º) Abra o seu config.lua e onde tiver QUOTEip = “127.0.0.1”edite o 127.0.0.1 ( ou qual quer outro ip que esteja no local ) pelo ip que você pegou no http://www.meuip.com.br.

3º) Pronto. Agora basta você tenta passar este mesmo ip pra seus amigos para que eles tentem entrar.

Configurando Ip fixo:
1º-Entre no site http://www.no-ip.com.

2º-Ai la em cima na direita terá uma coisa de entrar com sua conta.Se você ainda não tem um conta é só clicar em sign-up onde estará em baixo de Lost Password?.

3º-Lá você será obrigatório que você responda as questões sublinhadas em amarelo.

4º-Aceite o termo e de SIGN UP NOW!.logo apósd você ira receber um e-mail do no-ip.com.Abra o e-mail e confirme o cadastro.

5º-Vá no site e preenca onde esta para logar com sua conta, la estará assim:
E-mail:>>>>Coloque seu e-mail aqui<<<<
Password:>>>>Coloque seu password aqui<<<<
Preencha e de Login.

6º-Depois de ter entrado em sua conta estará um menu Escrito Hosts/Redirects que estará aberto.

7º-La você clicará em Add que será o primeiro da lista.

8º-Onde estiver Hostname ponha apenas o nome do seu serv.EX:
Loroteroserv.
OBS:Depois de ter escrito o nome do seu servidor não ponha (.) ou servegame.com. no-ip.info..

9º-Agora sim, em baixo você escolhera O resto do nome do Server.EX:
servegame.com, servercounterstrike.com, no-ip.info ou o proprio no-ip.com.

10º-Depois de ter feito isso não mecha em mais nada.

11º-Dessa la em baixo e clique em “Create Host”.

12º-Ficando assim:
Add a Host

The host loroteiroserv.no-ip.info resolving to 201.1.99.72 has successfuly been added to our system. New additions will take up to 5 minutes to become live on our DNS servers.

13º-Agora só copie o ip em numero ou seja em meu pc será 201.1.99.72 .

14º-Abra a pasta do seu ot e vai no config.lua e abra-o em bloco de notas.

15º-Procure um lugar que estará escrito:
— the ip the server should redirect too
ip = “”

16º-Onde está entre aspas você colocara o ip de numeros que você copiou la no no-ip.com quando você criou o ip.

17º-Salve e feche o config.lua .

18º-Pronto!!Ip fixo criado.

19º-Mas acalme-se ainda falta uma coisa importantissima.Toda vez que você reiniciar o computador você deverá ir no no-ip.com e ir na opção “Manage”.La estará seu ip fixo que você criou.clique em “Modify” Apenas dessa la em baixo e coloque dinovo Copie o ip
que estará em “Ip Adress” e de “Modify Host”.Faça o mesmo processo que expliquei no 14º e no 15º e cole la no config lua o novo ip que você pegou.Pronto espere 5 minutos e abra o server com o ip que você havia criado.No nosso exemplo que citei seria loroteiroserv.no-ip.info .

20º-Você deverá repetir esse processo toda vez que reiniciar o cmputador.

21º-Jogue e se divirta com seu ip fixo.

Parte 2 Ip fixo:

Você não consegue logar em seu server com o seu ip fixo que você criou depois qe reiniciou seu computador???Eis a solução:

1º-Você deverá ir no site http://www.no-ip.com onde você criou seu ip fixo.

2º-Depois de ter logado em sua conta la Nome menu escrito “Hosts/Redirects” vá na opção “Manage”.

3º-La estará o ip fixo do seu server apenas clique em “Modify”.

4º-Onde está “ip adress” estará outro ip.

5º-Copie-o e de “Modify Host”.

6º-Abra seu config.lua e substitua o ip que você avia pego pelo que você pegou agora ha um tempinho atrás.

7º-Depois disso salve e feche a pasta de arquivo.lua.

8º-Espere 5 minutos para usar o ip novamente aconselhavel esperar 10 minutos por precaução.

9º-Apenas toda vez que você reiniciar o computador repita o processo.

10º-Divirta-se.

Configurando o Config.Lua:

CODE
CODE– datadir
datadir = “data/”

S- Nome da pasta que está os componentes World, Spells, Monster, etc.

CODEmapfile = “data/world/guilcerapvp.otx”

S- Local ( data/world/ ) & Nome do mapa ( guilcerapvp.otx ) que o Server carregará.

CODEspawnfile = “data/world/guilcerapvp-spawn.xml”

S- Local ( data/world/ ) & nome do spawn ( guilcerapvp-spawn.xml ) que o Server carregará.

CODEloginmsg = “Guilcera Warmode!”

S-Mensagem que aparecerá quando alguem digitar a account pela primeira vez.

CODEallowsameips = “1”

S- Quantos players um ip só poderá abrir ( evitar mc ).

CODEhow long does the player has to stay out of fight to get un-skulled in ms (1000 = 1sec)
skulled = 1*45*1000

S- Quanto tempo o player ficará com battle após pegar Skull em milessegundos ( 1000 = 1seg ).

CODEhow many unjust kills to a red skull?
redskull = 3

S- Quantos players um jogador deverá matar injustamente pra obter uma Red Skull.

CODEport = “7171”

S- Port do seu Otserv ( aconselho não modificar, além dela ser a porta padrão, você deverá re-fazer o Tutorial de desbloquear a port 7171 modificando para a nova ).

CODEip = “”

S- Entre as aspas ( “” ) você colocará o IP obtido no site http://www.meuip.com.br

CODEmotdnum=”1″

S- Permanecendo “1”, a motd ficará Ligada. Colocando “0” ela será desligada.

CODEmotd = “PvP Server by Kevox”

S- Mensagem que aparecerá no default quando um player logar.

CODEdaycycle = 0

S- Permanecendo “0” o daycycke ( dia e noite ) ficará desligado. “1” ele ficará ligado.

CODEservername = “Guilcera”

S- Nome do mundo que ficará do lado direito do player na Player List.

CODEmaxplayers = “25”

S- Capacidade máxima de players em seu servidor.

CODEexhausted = 1*1500

S- Modificando o 1500 do 1*1500, mais exausted terá no server.

CODEpzlocked = 60*1000

S- Tempo em segundos que o player ficará com battle ( neste caso se encontra 1min ).

CODEallowclones = 1

S- Quantidades de pessoas que poderão entrar num mesmo char.

Como colocar server on em net compartilhada:
1º modo:
-1º Passo ———- Baixando o programa

Baixe o programa Hamachi ……. no site http://www.hamachi.cc/download

-2º Passo ———– Instalando

Instale-o no seu computador

-3º Passo ———– Iniciando o Programa

Abra o programa …………. No canto inferior esquerdo tem um botãosinho chamado Power On …. aperte e então eli ira pedir para voce se cadastrar com um nome de usuário e senha ……. coloque o que voce quiser como por exemplo:
EX: nome: exemplo …… senha: 1234

-4º Passo ———- Colocando o Server Online
Feito o usuário e estando conectado …… voce vai no canto inferior direito no Botãosinho chamado “Create or Join Networks” e em seguida cloque em “Create New Network” ———– Crie o nome do seu server e a senha que voce desejar–
Depois clique em OK e pronto voce verá que aparecerá um linha na tela inicial com o nome do seu server e o IP …… (no caso o ip tmb pode ser encontrado na barra do programa la em cima bem grande^^)

-5º Passo ————– Estamos Quase Lá
Agora só falta entra no config.lua no seu otserv e mudar o ip para o ip do Hamachi e abrir o servidor ………. e pronto estará online

Duvidas:

OS OUTROS NÃO ENTRAM NO MEU OTSERV POR QUE? APARECE QUE O SERVER ESTÁ OFF ME AJUDE!!!!

RE: Para que outras pessoas entrem no seu server elas também prescisam do programa Hamachi ………………… passe para seus amigos o programa e peça para eles se cadastrarem e clicar em “Create or Join Netowks” e depois em “Join Netwok” ….. ai pessa para ele colokar o nome do server (o que voce colocou quando criou) e a senha (que voce tmb colocou quando criou) e ai ele e voce verá que ele entrou na sua lista do server (no programa) ai sim ele poderá entrar no seu otserv…..

2º Modo:
Tutorial Internet Compartilhada por roteador
(feito com um roteador D-Link versão Dl-604, marca muito usada nos routers)

Obtendo o Gatway Padrão e entrando no menu de configuração do routeador
Primeiramente, você precisa do número do seu gateway padrão. Para conseguí-lo basta ir em Iniciar > Executar e digitar “cmd” (sem as aspas) aparecendo assim uma tela preta.

Nessa tela preta, digite “ipconfig” (sem aspas) e pegue o número do Gateway Padrão.

Agora abra o Internet Explorer e digite: http://”nº do Gateway Padrão” (sem as aspas) daí abrirá uma tela exigindo um nome de usuário e senha (esses dados foram fornecidos quando você configurou o routeador).
obs. Se não foi você que configurou o routeador, tente entrar com o nome de usuário “admin” (sem aspas) e deixe a senha em branco. Se mesmo assim não conseguir entrar, entre em contato com a pessoa que configurou o routeador.

Se fizer tudo certo, abrirá o menu do seu roteador com várias opções. No caso do routeador Dl-604, vá na guia advanced, localizado no topo, e depois clique na opção Firewall, localizada na barra da esquerda. É no firewall que você adcionará regras ao seu roteador para ele permitir ou não o acesso ao seu otserv.

Configurando o routeador
Feito isso, aparecerá várias opções para preencher. Irei indicar o que serve cada coisa aqui:
Name: nome da regra que irá ser adcionado à lista do Firewall
Action (allow/deny): é a ordem que você dará ao firewall em relação à regra, allow para permitir que outros conectem ao seu computador, e deny, para bloquear.
Source/Destination Interface (WAN/LAN): Interface WAN se refere aos computadores, fora de sua rede, que usarão o otserv. Interface LAN se refere ao computador que hospedará o otserv.
Schedule: aqui você indicará quando deixará valendo a regra. Poderá escolher em certos períodos do dia ou sempre.

Configure deste modo (coloque enabled na primeira linha):
Name: Open Tibia Server
Action: Allow
Source: Em interface, coloque WAN. Logo em seguida, em IP Start, coloque “*” (sem aspas), significando que qualquer pessoa poderá entrar em seu otserv. Deixe IP End em branco.
Destination: Em interface, coloque LAN. Em IP Start coloque seu IP Global (que pode ser conseguido em clicando aqui)! Deixe IP End em branco e marque, em Protocol, TCP. Em Port Range, escreva “7171” (sem aspas) na primeira lacuna e deixe a da direita em branco.
Schedule: Always

Pronto! Basta clicar em Apply e reiniciar o router (no caso do Dl-604, ele reinicirá sozinho ao clicar em apply)!

Vá ao config.lua do seu otserv e coloque seu IP Global em the IP the server should redirect too.

Site:
Bom, há uns programinhas necessários pra rodar um site…

Programas:
-EasyPHP- ftp://download.revolutionhosting.net/rh/easyphp1-7_setup.exe
-Scripts em PHP- http://rapidshare.de/files/18617488/www.rar.html

-EasyPHP-
*Instale-o em qualquer lugar, a sua escolha.
*Na pasta EasyPHP 1-7, vai ter uma pasta chamada Apache.
*Entre nela, depois vá na pasta conf e abra com Bloco de Notas/WordPad o arquivo httpd.conf .
*Dê Ctrl + F e procure por Port 80.
*Em Port 80, adicione 90 no final, ficando assim: Port 8090

-Configurando o PHP-
*Baixe os Scripts.
*Descompacte o .rar na pasta do EasyPHP, se ele perguntar se pode substituir, escolha Sim para Todos.
*Agora, abra o config.php com algum editor de texto.

*Terá o seguinte:

QUOTE//————————–Diretorios—————————//
= \’D:\Otserv\data\accounts/\’; //Diretório das accounts.
= \’D:\Otserv\data\players/\’;//Diretório dos players.
//—————————————————————//

*= É o diretório de Accounts do OTServer. Coloque o diretório separando cada pasta com uma barra assim \, e quando terminar coloque /.
*= É o diretório de Players do OTServer. O mesmo de cima só que de players.

QUOTE//—————————-Ranks——————————//
= “10”; //Quantos irao aparecer no rank
//—————————————————————//

*= O número de pessoas que aparecerão no ranking.

QUOTE//———————-Informaçoes do Server——————–//
= “Rikera OTServer”;
= “rikeserver.servegame.com”;
= “7171”;
//—————————————————————//

*= Nome do seu OTServer.
*= IP do seu OTServer.
*= Port do seu OTServer(Recomendado não alterar).

QUOTE//—————————Visual——————————//
= “Rikera OTServer”;
= “6”;
= “Rikera foi reformulada. (:”;
//—————————————————————//

*= Titúlo que aparecerá no topo da página.
*= Número máximo de caracteres para a account.
*= Notícia curta e rápida que aparecerá na página principal do site.

QUOTE//—————————Dados OT——————————//
= “10x”;
= “10x”;
= “10x”;
= “1x”;
= “500 Gps”;
= “Non-PvP”;
= “1 K 100x”;
//—————————————————————//

*= Quantos X é a EXP.
*= Quantos X é o Magic Level.
*= Quantos X é as Skills.
*= Quantos X é o Loot(1x= Loot normal).
*= Preço por SQM de uma casa.
*= Modo do OTServer(PvP, Non-PvP, etc).
*= Preço médio das runas.

QUOTE//—————————Contadores————————–//
= TRUE;
= “count.txt”;
= “ips”;
//—————————————————————//

*= Coloque TRUE se quiser que apareça um contador de accounts já feitas no servidor, ou coloque FALSE se não quiser.
*= Nome do arquivo que guardará o número de pessoas que fizeram cadastro.
*= Pasta onde estará guardado os ips de quem se cadastra.

OBS: Para mudar os equips iniciais, configure no Criarplayer.php, na pasta accounts, lá no finalzinho.

-Protegendo seu OTServer-
*Para proteger seu server, abra o Bloco de Notas e nele escreva:
QUOTEDeny For All
*Salve-o na pasta do seu ot como .htaccess .
*Crie uma cópia do .htaccess e coloque esta cópia na pasta Ips, que fica na pasta account do PHP.
*OBS: COLOQUE APENAS NA PASTA DO SEU OT E NA PASTA IPS, SENÃO O PHP VAI BUGAR E NÃO VAI DAR PRA CRIAR CHAR!!!

-Colocando o site no ar com IP fixo-
*Entre em http://www.no-ip.com .
*Clique em Sign-Up Now!
*Preencha todos os dados(Coloque e-mail certo, será necessário depois).
*Se cadastre e espere o e-mail chegar.
*Entre no e-mail, confirme sua conta do No-IP e entre com seu login no No-Ip.
*No menu Hosts/Redirects, vá em Add.
*No Hostname, escolha um nome a sua escolha.
*Irá ter um “no-ip.info” embaixo, clique nele pra escolher um outro tipo de domínio… Exemplo: servegame.com .
*Deixe tudo como está e clique em Create Host.
*Como todo mundo sabe, ao reiniciar o computador ou a Internet, o IP irá mudar, então no site do No-IP, para facilitar, no canto superior esquerdo há um Current IP: <IP>, copie o <IP> lá no site e no config.lua do OT altere o IP.
*No seu Host do No-IP também é necessário fazer isto, portanto copie o IP que aparece no site, vá em Manage no Menu, e no seu Host clique em Modify.
*Na caixa IP Address altere o IP pelo que você copiou.
*Lembrando: SEMPRE QUE REINICIAR A NET OU O PC REPITA ESTE PROCESSO DE ALTERAÇÃO DO IP!

-Testando a segurança do seu site-
*Rode os programas EasyPHP, apache e entre em seu site…(http://seuip:8090)
*Após o “8090”, digite /account .
*Ele vai acessar uma pasta, mas agora tente entrar na pasta IPS. Se não aparecer nada, muito bem, sua pasta de IPS(Onde ficam as accounts e senhas) está protegida!
*Agora, tente acessar a pasta do seu OT da mesma forma como você acessou a pasta account…(Coloque /Nome da pasta do ot depois do 8090)
*Não apareceu nada? Então parabéns!
*Seu site está bem protegido e seu OT não sofrerá hackings…

-Finalizando-
*Abra o programa EasyPHP, na pasta EasyPHP 1-7, o ícone é um “e”.
*Na pasta apache, abra o programa apache.
*Rode seu OT e pronto!!!
*Site ON, OT ON!
*Seu site poderá ser acessado por:
QUOTEhttp://Seu IP fixo(Ou móvel, tanto faz):8090
*Exemplo:
QUOTEhttp://rikeserver.servegame.com:8090

OBS: Caso o PHP seja outro, o processo fundamental do config.php não vai mudar muito.Faça do seu jeito, fuce tudo, procure bastante pelos erros, seja persistente!

Outra opção para ver seu IP é o site http://www.whatip.com , e o site http://www.meuip.com.br .

Extras:

LISTA DE ESPERA?
Isso acontece porque o Spawn do Player (a posição que ele está), ESTÀ EM CIMA DE ALGUMA COISA (paredes, portas..).
SOLUÇÃO: Mudar o Spawn do Player! Abra (No bloco de Notas) o NOME DO PLAYER.XML, NA PASTA PLAYERS, PRECIONE CTRL+F, PROCURE POR: spawn ,e MODIFIQUE…
QUOTEEXPLICANDO:

PONHA EM: x=”CORDENADAX”, EM y=”CORDENADAY”, EM z=”CORDENADAZ” (PONHA AS CORDENADAS DO TEMPLO DO MAP EM <TEMPLE> , E PODE POR IGUAL NO SPAWN)

EXEMPLO:
<spawn x=”504″ y=”504″ z=”6″/><temple x=”504″ y=”504″ z=”6″/>

MUITAS VEZES as pessoas acham que é problema do site… é mais ou menos, pois a maioria das pessoas esquecem de por o templo e o spawn certo no config.php!
ENTÂO VOCE ABRE O SEU CONFIG.PHP (na pasta www) e coloca as coordenadas do templo certo.. e no spawn coloca as mesmas coordenadas do templo. ESSA SERIA A SOLUçÂO.

Abre char na list world mas não entra?
ABRE A CHAR LIST, MAIS NÂO ENTRA?
=p VOCE TEM QUE FAZER O SEGUINTE:

1- VER SE SEU IP ESTÀ CORRETO NO CONFIG.LUA
ACHE IP = “” , NO CONFIG.LUA
QUOTE– ip
— the ip the server should redirect too
ip = “”

COLOQUE SEU IP ENTRE AS TAGS ” “.
EXEMPLO:
QUOTEip = “201.13.218.8”

Não sabe seu IP? Clique Aqui! (Somente os Números, NÃO É O REVERSO!)

DEPOIS de ter feito isso, ache o icone do seu otserv.exe, CLIQUE COM O BOTÃO DIREITO E >CRIAR ATALHO.

DEPOIS QUE VOCE CRIOU O ATALHO, CLIQUE COM O BOTÃO DIREITO NELE(NO ATALHO), VÁ EM PROPRIEDADES.
NO DESTINO, DE UM ESPAçO DEPOIS DA ” e COLOQUE O SEU IP

NO LUGAR DE 201.13.218.8, PONHA O SEU IP.
Não sabe seu IP? Clique Aqui! (Somente os Números, NÃO É O REVERSO!)

PRONTO… AGORA DE APLICAR, e OK!

QUANDO VOCÊ VAI ABRIR O SERVER

OS 2 IPS IGUAIS!

SEMPRE ABRA SEU OTSERV PELO ATALHO!

Esta cansado de ver seu server sendo invadido por hackers ??

Seus problemas acabaram ..

Primeiramente :

*Como eles invadem meu pc ?
-Eles entram pelo site de accounts. (Sem detalhes se não vão descobrir como hackeia)

*Tah bom .. mas como impedir que eles entram ?
-Você coloca o nome da pasta que esta seu ot bem dificil por exemplo : LKMs RoX oT

*Mas porque tem que por um nome assim ?
-Porque os hackers invadem o server pelo nome da pasta.

Galera o tuto acaba por aki espero ter ajudado .. demorei pra fazer esse tutorial pq soh hj q vi uns kras entrando em um server.

Não existe essa maneira mas existem VÁRIAS maneiras de se hackear um server, vamos dizer maneira noob e maneira inteligente de se hackear um server.

Edit : (Mais informaçoes para o topico) > By Iguinho

A maneira noob de se hackear é entrando pelo site de account como ele disse mas SEM DETALHES.

A maneira inteligente de se hackear é com um keylogger, por exemplo, você baixa um otserver contaminado de keylogger mas não sabe que tem keylogger, ai vamos dizer que voce abra seu server e entre com sua account de gm o keylogger, ele rouba a sua senha e manda para o hacker, logo depois o hacker tem acesso a sua conta de gm como tambem a sua conta de e-mail e etc…

MAS ISSO TEM UMA SOLUÇÃO!

Na hora que você for criar o seu otserver você simplesmente não ponha a pasta do otserver na pasta www, ponha em algum outro diretorio na pasta C:\ e etc… mas isso não quer dizer que você esta 100% seguro de nao ser hackeado, existem 1001 maneiras de se hackear que eu nao vou postar aqui.

Sobre o keylogger eu sugiro baixar um antivirus bom de empresa boa como o norton ou outros ai, que ele cata o keylogger mas é sempre necessário que ele fique atualizado que se não ele não cata nada xis dê.

Criando char Gm:
—EM DATA/PLAYERS—
-Vá em data/players. (vamos supor que existe um char chamado Ajuda)
-Copie o char “Ajuda” e cole-o na mesma pasta.
-Renomeie este char para o nome do GM desejado (vamos supor que o nome do seu GM seja, GM Ok)
-Agora com o botão direito clicke em editar… edite para isso:
*Em name=”Ajuda” mude para name=”GM Ok”
*Em account=”159″ para account=”acc 1111″(vamos supor que seja “1111, se voce quiser 1414 tem que ficar assim; account=”1414″)
*Em access=”0″ mude para access=”3″
*Em <look type=”128″> mude para <look type=”75″>
Salve !

—EM DATA/ACCOUNTS—
-Copie a account que estiver nesta pasta.
-Renomiei para account colocada no seu GM (que era a 1111).
-Agora com o botão direito clicke em editar.
*Em <account pass=”lala” mude para senha desejada ex: <account pass=”senhaaqui”
*Em characters:
Exemplo;
<characters>
<character name=”Ajuda” />
</characters>
Mude para o nome do GM colocado em data/players:
<characters>
<character name=”GM Ok” />
</characters>
Salve!

Como deixar server On 24:00 horas on:

Mesmo que voce tenha um reestarter sempre da akele errozinho que trava seu OTServ, para tirar akele errinho que enche o sako aki vai a resposta:
Entre no painel de controles/sistema/avançados/relatorio de erros/escolher programa/adicionar/procurar
Agora ache seu OTServ.exe e ponha lá e de OK
Pronto
Nao inviara + ralatorio de erros
Mas ainda tera a possibilidade de aparecer erros criticos
ai seja mais radical
Mande desativar o relatorio de erros e dismarque o “notificar-me quando ocorrerem erros criticos” na pagina do ralatorio de erros

Esse tutorial creio que vai ajudar mta gente

~Agora crie seu Auto-restarter~

aew pessoal… vo ensina a faze seu proprio Auto-Restarter.. isso mesmo.. akele q qndo seu server fecha ele volta sozinho x)~

Vamos começar 😆

Vow da um exemplo aki do MEU Auto-restarter.bat:

CODE@echo off
title OTserv Auto-restarter
echo :: =========================================
echo :: — OTserv Restarter —
echo :: — Por: Fvox —
echo :: =========================================
echo ::
:begin
OTserv.exe
echo ::
echo :: =========================================
echo :: — O Sever caiu, volta ja ja —
echo :: =========================================
echo ::
goto begin
:goto begin

Agora faça o seu:

1°)Abra um bloco de notas
2°) escreva nele (Naum esqueça de tirar o “CODE” se vc for Copiar e colar):
CODE@echo off
title OTserv Auto-restarter
echo :: =========================================
echo :: — OTserv Auto-Restarter —
echo :: — Por: Seu nick aki —
echo :: =========================================
echo ::
:begin
Nome do Executavel.exe
echo ::
echo :: =========================================
echo :: — Mensagem de quando o server cai—
echo :: =========================================
echo ::
goto begin
:goto begin

Agora eh soh renomeia as coisas q eu colokei la tpw:

Por: Seu nick aki
Nome do executavel.exe (Exemplo: OTserv.exe)
Mensagem de quando o server cai (Exemplo: o Server caiu.. volta ja)

3°) depois de ter feito salve o seu bloco de notas o arquivo.bat (Exemplo: Auto-Restarter.bat)

4°)Abra seu server e divirta-se pq ja acabo xDDDD
– – – – – – – – – – – – – – – – – – – – – – – – – – – –

Agora sempre q seu server cair ele vai cair direto… e o Auto-Restarter o abrirá normalmente!!!
