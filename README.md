Material de estudos

blog diolinux
blog do edivaldo
viva o linux
guia foca linux

Descobrindo o Linux




################################# ATALHOS #################################

CTRL + SHIFT + T = Abre uma nova guia do terminal(uma janala do terminal já tem que eestar aberta)


=====================COMANDOS BASICOS PARA LINUX===================

ESTRUTURA DE DIRETÓRIOS


DIRETÓRIO /	= Diretório Raiz do sistema, então se o diretório / é o raiz todos os proximos diretórios estarão abaixo do direitório raiz

/sbin
/var      ----> /log e /spool
/boot
/dev      ----> /fd0
/etc
/home     ----> /ftp e /leo e /ivani (usuários)
/lib
/mnt
/root
/tmp
/usr      ----> /man e /lib e /bin
/bin




######################## O DIRETÓRIO RAIZ (/)###############################

Todos os arquivos e diretórios do sistema Linux instalados no computador partem de uma única origem: o diretório raiz. Mesmo que  estejam armazenados em outros dispositivos físicos, é a partir do diretório raiz - representado pela bala barra (/) - que você poderá acessá-los.
Também vale lembrar que o único usuário do sistema capaz de  criar ou mover arquivos do diretório raiz é o root, ou seja, o usuário-administrador. Isso evita que usuários comuns cometam erros e acabem comprometendo  a integridade de todo os sistema de arquivos.



Toda e qualquer alteração feita no diretório raiz, só pode ser feita ou executada pelo usuario root.

============================================================================

######################## BINÁRIO EXECUTÁVEIS: /bin  ########################

No diretório /bin estão localizados os binários executáveis que podem ser utilizados por qualquer usúario do sistema. São comandos essenciais, usados para trabalhar com arquivos, textos e alguns recursos básicos de rede, como o cp, mv, ping e grep.

---------------------------------------------------------------------------
---------------------- BINÁRIOS DO SISTEMA: /sbin --------------------------

Assim como o /bin, este diretório armazena executáveis, mas com um diferencial: são aplicativos utilizados por administradores de sistema com o propósito de realizar funções de manutenção e outras tarefas semelhantes. Entre os comandos disponíveis estão o ifconfig, para configurar e controlar interfaces de rede TCP/IP, e o fdisk, que permite particionar discos rígidos, por Exemplo.


####################### PROGRMAS DIVERSOS: /usr ############################

Se você não encontrar um comando no diretório /bin ou sbin, ele certamente está aqui.
O /usr reúne executáveis, bibliotecas e até documentação de softwares usados pelos usúarios ou administradores do sistema. Além disso, sempre que voc/çe compilar e instalar um prograa a partir do código-fonte, ele será instalado nesse diretório.

##################### CONFIGURAÇÃO DO SISTEMA: /etc #######################

No diretório /etc ficam arquivos de configiração que podem ser usados por todos os softwares, além de scripts especiais para iniciar ou interromper módulos e programas diversos. É no /etc que se encontra, por exemplo, o arquivo resolv.conf, com uma relação de servidores DNS que podem ser acessados pelo sistema, com os parâmetros necessários para isso.


########################## BIBLIOTECAS: /lib ###############################

Neste ponto do sistema de arquivos ficam localizadas as bibliotecas usadas pelos comandos presentes em /bin e /sbin. Normalmente, os arquivos de bibliotecas começam com os prefixos id ou lib e possuem "extensão" so.

############################ OPCIONAIS: /opt #############################

Aplicatvis adicionais, que não são essenciais para o sistema, terminam neste diretório.

########################### ARQUIVOS PESSOAIS: /home #####################

No diretório /home ficam os arquivos pessoais, como documentos e fotografias, sempre dentro de pastas que levam o nome de casa usuário. Vale notar que o diretório pessoal do administrador nao fica no mesmo local, e sim em /root.


############################ INICIALIZAÇÃO: /boot #########################

aRQUIVOS RELACIONADOS à inicialização do sistema, ou seja, o processo de boot do Linux, quando o computador é ligado, ficam em /boot.

(Também tem um programa chamado grub, que é o programa que controla todo o sistema de inicialização)

############################ SERVIÇOS: /srv ###############################

Dados de servidores e serviços em execução no computador ficam armazenados dentro desse direório.

########################### ARQUIVOS VARIÁVEIS: /var ######################

Todo arquivo que aumenta de tamanho ao longo do tempo está no diretório de arquivos variáveis. Um bom exemplo são os logs do sistema, ou seja, refistros de forma de texto de atividades realizadas no Linux, como os logins feitos ao longo dos meses.



###################### VOLUMES E MÍDIAS: /mnt e /media ###################

Para acessar os arquivos de um Cd, pendrive ou disco rígido presente em outra máquina da rede, é necessário "montar" esse contéudo no sistema de arquivos local, isso é, torna-lo acessível como se fosse apenas mais um diretório no sistema.

Em /media ficam montadas todas as mídias removíveis, como dispositivos USB e DVD's de dados. Já o diretório /mnt fica reservado aos administradores que precisam montar temporariamente um sistema de arquivos externo.


###################### ARQUIVOS DE DISPOSITIVOS: /dev #####################

No Linux, tudo é apresentado na forma de arquivos. Ao plugar um pendrive no computador, por exemplo, um arquivo será criado dentro do diretório, você encontra caminhos semelhantes para acessar terminais e qualquer dispositivo conectado ao computador, como o mouse e até modems.


##################### PROCESSOS DO SISTEMA: /proc ##########################

Lembra da história de que tudo funciona como um arquivo no Linux? Pois o /proc é a prova disso. Nesse diretório são encontrados arquivos que revelam informações sobre os recursos e processos em execução no sistema. Quer um exemplo? Para saber há qanto tempo o Linux est[a sendo usado desde a última vez em que foi iniciado, basta ler o arquivo /proc/uptime.


#################### ARQUIVOS TEMPORÁRIOS: /tmp ############################

Arquivos e diretórios criados temporariamente tanto pelo sistema quanto pelos usuários devem ficar nesse diretório. Boa parte deles é apagada sempre que o computador é reiniciado.


########   PRATICA NOS COMANDOS   

todos os comandos podem ser complementados, por alguns comandos que são denomidos de flags, as flags fazem funções extras em seus comandos basicos


ls = lista o conteúdo do diretório atual

~

ls / Mostra todo o conteúdo do diretório /

~

ls -h mostra algumas opções

~

ls -l lista o conteúdo mostrando informações como, tamanho, data e permissões

ls -lh lista o conteúdo mostrando informações como, tamanho, data e permissões porém de uma forma mas simplês e facil de se entender por uma pessoa!

ls -lha mostra todos os arquivos, até mesmo os ocultos, se tiver algum (" Arquivos ocultos no linux são mostrado com um . no início do seu nome")

cd é o comando para entrar nos diretórios exemplo cd / vai te direcionar para o diretório /




mkdir -- cria um diretórios

cat -- mostra o conteúdo dos arquivos sem precisar abrir ele para editar

cp -- copia um arquivo

mv -- move ou renomeia um arquivo ou diretório

para mover um arquivo o comando deve seguir a seguinte forma

mv /diretório que você quer mover/arquivo que você quer mover

Para renomear voê deve seguir a seguinte forma

mv /arquivo_que_você_quer_renomear novo_nome_do_arquivo


########################### AJUDA NO LINUX #################################


man -- responval por imprimir na tela o manual do comando exemplo man ls ("Mostra o manual do comando ls, explicando funções e as flags que você pode utilizar")

apropos -- procura qualquer man baseado em uma palavra ou descrição

--help mostra o manual resumido de qualquer programa ou comando("Mostrando uma descrição rapida, e alguns dos principais comandos de saido do programa")

########################### MANIPULANDO ARQUIVOS ###########################






########################### PROGRAMAS NO LINUX #############################

Pata atualizar os pacotes de programas instalados no programa você deve colocar, o comando

apt-get update




####################### O PODER DA LINHA DE COMANDO ########################
========================================================================================================================================================



ARQUIVAR ARQUIVOS VIA LINHA DE COMANDO ------

COMPACTANDO COM TAR

tar um comando para compactação (um utilitario de compactação)

tar c (create - mostra o arquivo a ser criado) v (verbose - mostra o processo de compactação" Status) f(file - tipo de arquivo) x(extract - extrair arquivos)

tar cvf 'nome do arquivo'.tar + arquivos a serem compactados "Compacta os arquivos em formato .tar)

DESCOMPACTANDO COM TAR

tar xvf 'nome do arquivo'.tar extrai os arquivos desse arquivo .tar

gzip - mais rapido o processo de compatação
bzip - processo melhorado de compactação comprime melhor os arquivos porem demora mais


^^^^^^^^^^ 
COMPACTANDO COM GZIP

tar czvf compacto.tar.gz *.txt para utilizar o gzip para compactar todos os arquivos .txt do diretório, agora acrescentando o 'z' para indicarmos que estamos utilizando outro compactador 

DESCOMPACTANDO COM GZIP

tar xzvf 'nome do arquivo'.tar.gz

COMPACTANDO COM BZIP

tar cjvf compacto.tar.bz2 *.txt utilizando o bzip para compactar todos os arquivos .txt

utliziando o j para representar o bzip

DESCOMPATANDO COM BZIP

xjvf 'nome do arquivo'.tar.bz2


COMPACTNDO COM ZIP

zip 'nome do arquivo'.zip

DESCONPACTANDO COM ZIP

unzio 'nome do arquivo'.zip


========================================================================================================================================================

PESQUISAR E EXTRAIR DADOS DE ARQUIVOS 

	less - ler o conteudo dos arquivos
	wc - conta linhas, palavras e caracteres
	cat - ler conteudo de um arquivo, a diferença do cat pro less é que o less agt entra e permanece no arquivo o cat se le as ultimas linhas do arquivo
	tac - ler as primeiras linhas de um arquivo
	head - ler as 10 primeiras linhas de um arquivo, a não ser que você passe o aramentro n+numero de linhas que voce quer ler, ele vai mostrar o numero de linhas que vc quer ler
	tail - lê as ultimas linhas de um arquivo, caso queira seguir o restante das modificações em tempo real, utilize a flag f(follow) para serguir em tempo real
	sort - ordenar um arquivo em ordem alfabetca
	cut -d (delimitador) ';' -f 1,3(colunas que você quer que sejam lidas) 


======================================================================================================= REDIRECIONADORES ===============================
============================================================================


			
					  -----> STDOUT
			STDIN --> PROCESS 
					  -----> STDERR

ENTRADA PADRÃO: Teclado(Exemplo: Comando digitado "pwd", "ls", "outros")
SAÍDA PADRÃO: Tela (Exemplo: saída do comando pwd na tela)
SAÍDA DE ERRO: Comando desconhecido!

VALORES DOS DESCRITORES:| SINAIS DOS DESCRITORES
			| 
STDIN  = 0 		| >=1>   --> [Saída padrão] 
STDOUT = 1	        | >>=1>> --> [Saída com adição]
STDERR = 2		| 2>     --> [Saída de erro]

======================================================================================================== EXPRESSÕES REGULARES===========================
============================================================================


PRÁTICA

Regex = Regular Expression -> Conjuto de meta-caracteres
Principais expressões regulares:

^: Começo de linha.
$: Fim de linha
.: Qualquer caractere.
*: Qualquer sequência com tamanho igual ou superior a zero do caractere precedente.
?: Uma ou nenhuma ocorrência do caractere precedente.
[]: Qualquer caractere que esteja presente nos colchetes.




========================================================================================================================================================

				SHELLSCRIPT

========================================================================================================================================================

#! --> she bang --> exe /bin/bash ("mostra o inicio da pagina indicando que será um arquivo executavel")






========================================================================================================================================================

			
	     SEGURANÇA BÁSICA E IDENTIFICAÇÃO DE TIPOS DE USUÁRIOS


========================================================================================================================================================

ROOT -> Responsável por criar usuários no sistema local


		CONTAS -------> GRUPOS
		  |               |
	     /etc/passwd       /etc/group


UID / GID

ROOT -> id = a zero
Demais usuários -> +1000

Como saber quais ou qual usuario logou no sistema resentemente


lastlog - mostra os usuarios que logaram
last - quem esta logado no sistema
who - mostra os usuarios logados no momento


CRIAÇÃO DE USUARIOS


Comando useradd
-c  comentário: comentário (Geralmente o nome completo do usuário).
-d diretório caminho para o diretório pessoal do usuário.
-g grupo: grupo inicial (GID). Precis existir previamenten sistema.
-G grupol, grupo2: grupos adicionais, separados por vírgula.
-u UID: UID (User ID) do usuário.
-s shell: Shell padrão para o usuário.
-p senha: Senha (entre aspas).
-e data: data de validade da conta.
-k /etc/skel: copia o diretório modelo /etc/skel.
-m cria o diretório pessoal, se não existir.


useradd -c "Full name" -p "senha" 

cat /etc/passwd - informações dos usuarios
cat /etc/shadow - informações de senha
passwd - muda a senha do usuario
passwd nomedousuario - caso não informe o usuario que você quer trocar a senha, sera trocado a senha do root !!!!!TOMAR CUIDADO!!!!


COMANDO adduser melhor comando para criação de usuarios

passwd -l(lock) - trava o usuario
passwd -u(unlock) - destrava o usuario
vipw - editar senhas e grupos
chfn - changer information (troca de informações do usuarios)
userdel - deleta usuario
chage - define quando vai ser trocado uma senha(expirar, troca de senha etc.)

COMANDO groupadd

gpasswd grupo: cria uma senha para grupo.
gpasswd -r grupo: apaga a senha para grupo.
gpasswd -a usuário grupo: associa usuário ao grupo.
gpasswd -d usuário grupo: exclui usuário de grupo.
gpasswd -A usuário grupo: toma um usuário administrador do grupo.


========================================================================================================================================================

		GERENCIE PERMISSÕES E PROPRIEDADE DE ARQUIVOS

========================================================================================================================================================


COMANDO PARA TRADAR PERMISSÕES 

COMANDO chmod --> Permissões


Usuário dono do arquivo (u).                   r          w         x
Grupo dono do arquivo (g).                     2²         2¹        2
Demais usuários - outros - (o).		       4          2         1



r = read (leitura)
w = write (escrita)
x = execute (execução)



SUID SGID STICK r   w  x   r  w  x   r   w  x
  0   0    0    0   0  0   0  0  0   0   0  0
____________   __________ ________   _________
     |              |        |           |

		Usuário     Grupo     Outros


MODOS DE USAR O COMANDO CHMOD

1ºmodo informando as permissões correspondentes abaixo!

+ = adicionar uma permissão
- = remover uma permissão
= = equalizar uma permissão


	ALVO		   |	OPERAÇÃO       |        PERMISSÃO
u - user (Usuário)	   |	   +           |  r - read(leitura)
g - group (grupo) 	   |	   -           |  w - write (escrita)
o 0 others (outros)	   |	   =           |  x - execute (executção)
a - all (todos os acima)   |		       |



# chmod g-w arquivo.txt --> rw-r--r--
# chmod ugo+rwx arquivo.txt --> rwxrwxrwx
# chmod a-wx arquivo.txt --> -r--r--r--

2ºmodo, informando os valores numéricos (octal) para as permissões correspondentes abaixo!

	ALVO		   |	OPERAÇÃO       |        PERMISSÃO
u - user (Usuário)	   |	   +           |  r - read(leitura)
g - group (grupo) 	   |	   -           |  w - write (escrita)
o 0 others (outros)	   |	   =           |  x - execute (executção)
a - all (todos os acima)   |		       |



# chmod 744 arquivo.txt --> rwxr--r--
# chmod 777 arquivo.txt --> rwxrwxrwx
# chmod 711 arquivo.txt --> -rwx--x--x



chown - muda o dono do arquivo
chgrp - muda o grupo do arquivo



			DIRETÓRIOS E ARQUIVOS ESPECIAIS

PERMISSÕES ESPECIAIS

SUID bit
Set owner User ID Quando setado, permite que qualquer usuário execute determinado prgrama, como se fosse o usuário donmo.


Exemplo:

Comando passwd roda com sid configurado para que usuários possam alterar suas senhas
# chmod u+s arquivo.txt
# chmod 4750 arquivo.txt -->rwsr-x---


	SUID		SGID		STICK         r		w	 x
	 1		  0		  0	      2²	2¹ 	 2
	 <------------------------------------------  4	  	2	 1



STICKY BIT

Quando setada, impede que um usuário apague o arquivo ou diretório do outro, mesmo que o diretório pai tenha permissões que permitam a exclusão.

Somente o proprietário e o root podem excluir arquivos em uma pasta que tenha o Sticky bit ativado! Usa-se o comando ls -ls -> informações do próprio diretório.


# chmod 1750 arquivo.txt --> rwxr-x--T



	SUID		SGID		STICK         r		w	 x
	 0		  0		  1	      2²	2¹ 	 2
	 			          <---------  4	  	2	 1


	


========================================================================================================================================================

			LINKS SIMBÓLICOS E HARDLINKS

========================================================================================================================================================

Links simbólicos e hardlinks --> São atalhos, arquivos especiais!

--> Vários nomes que um inode do sistema de arquivos de ter


um inode é o elemento básico que identifica o arquivo no sistema de arquivos


# ls -i arquivo.txt -> A opção -i do comando ls mostra o número dos inodes dos arquivos:

1. Criando link hard

# In menu.sh adm.sh

2. Criando link soft

#In -s menu.sh atalho-adm

