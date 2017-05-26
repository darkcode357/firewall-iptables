# firewall-iptables
## firewall para hackers e trackes que querem deixar o seu sistema mais seguro e com regras de portas 
```
[darkcode distro]# bash firewall-arch 
    
       .__                              ___.          .__   
  ____ |  |__   ___________  ____   ____\_ |__ ___.__.|  |  
_/ ___\|  |  \_/ __ \_  __ \/    \ /  _ \| __ <   |  ||  |  
\  \___|   Y  \  ___/|  | \/   |  (  <_> ) \_\ \___  ||  |__
 \___  >___|  /\___  >__|  |___|  /\____/|___  / ____||____/
     \/     \/     \/           \/           \/\/           
  _____.__                      .__  .__                    
_/ ____\__|______   ____ _____  |  | |  |                   
\   __\|  \_  __ \_/ __ \\__  \ |  | |  |                   
 |  |  |  ||  | \/\  ___/ / __ \|  |_|  |__                 
 |__|  |__||__|    \___  >____  /____/____/                 
                      \/     \/                            

Opções disponíveis são: start|stop|restart|status|panic|install
firewall  ch-os

[darkcode distro]# bash firewall-arch start 
    
       .__                              ___.          .__   
  ____ |  |__   ___________  ____   ____\_ |__ ___.__.|  |  
_/ ___\|  |  \_/ __ \_  __ \/    \ /  _ \| __ <   |  ||  |  
\  \___|   Y  \  ___/|  | \/   |  (  <_> ) \_\ \___  ||  |__
 \___  >___|  /\___  >__|  |___|  /\____/|___  / ____||____/
     \/     \/     \/           \/           \/\/           
  _____.__                      .__  .__                    
_/ ____\__|______   ____ _____  |  | |  |                   
\   __\|  \_  __ \_/ __ \\__  \ |  | |  |                   
 |  |  |  ||  | \/\  ___/ / __ \|  |_|  |__                 
 |__|  |__||__|    \___  >____  /____/____/                 
                      \/     \/                            

-------------------------------------
Firewall!
criador darkcode
proteção para o sistema operacional blackarch
-------------------------------------
Loading modules...
Cleaning up firewall...
OK -> difinindo politicas padrão...
OK -> liberandom o Loopback ...
OK -> proteção contra DOS
OK -> abilitar comunicação com outras interfaces...
====>Bloquear pacotes com estado novo/invalido que saiam pela placa  de rede (eno1/wlan0wlo1/outras)<====
modificar como a sua placa de rede para ter a proteção
====>Bloqueando conexão brute force via SSH:<====
OK -> Conexão SSH aceita (fail2ban abilitado)...
====>PROTEÇÃO CONTRA ATAQUES<====
OK -> bloqueando  attacks...
====>PROTEGE CONTRA PACOTES QUE PODEM PROCURAR E OBTER INFORMAÇÕES INTERNAS<====
OK -> proteção Spy-packages ...
====>BLOQUEANDO TRACEROUTE<====
OK -> bloqueando traceroute...
====>REGRAS DE SEGURANÇA NA INTERNET<====
OK -> regras de segurança na internet...
====>PROTECOES DE KERNEL<====
OK -> proteção para o Kernel ...
====>Portas do user do CH-OS<====
------> Abrindo Portas do Apache
open port tcp 80
open port tcp 443
open port tcp 8080 
-------> Abrindo Portas para DNS
open port udp 53
-------> abrindo porta para o postgresql
open port tcp 5432
-------> Abrindo Portas para MYSQL
open port tcp 3306
open port udp 3306
-------> Abrindo Portas para SSH
open port tcp 2222
open port udp 2222
----------------------
tunelamento ssh ataque
open port tcp 3212
open port tcp 1232
====>PORTAS PARA ATAQUE<====
====>BEEF-XSS<====
open port tcp 3000
open port udp 3000
------->teamserver armitage/cobalt
port open tcp 555554
port open tcp 419
port open tcp 5419
port open udp 5419
port open tcp 519
port open udp 519
------->metasploit<--------
open port 4444
open port 4455
open port 3322
open port 2233
open port 3322
open port 5301
-------> abrindo porta  para beef-xss
====>Proteções Adicionais<====
====>Proteção contra ping da morte<====
====>Proteção contra trinoo<====
OK -> proteção Trinoo ...
====> Proteção contra trojans<====
OK -> proteção contra Trojan ...
====>Proteção contra worms<====
OK -> proteção contra Worm ...
====>Proteção contra port scanners<====
OK -> proteção contra Port Scanner ...
====>BLOQUEANDO PORT SCANNERS OCULTOS<====
OK -> proteção contra porte scanner oculto...
====>BackOrifice<====
OK -> proteção BackOrifice ...
====>NetBus<====
OK -> proteção NetBus ...
====>Ativa mascaramento de saída<====
OK -> mascarando Packages de saida ...

[darkcode distro]# bash firewall-arch stop
    
       .__                              ___.          .__   
  ____ |  |__   ___________  ____   ____\_ |__ ___.__.|  |  
_/ ___\|  |  \_/ __ \_  __ \/    \ /  _ \| __ <   |  ||  |  
\  \___|   Y  \  ___/|  | \/   |  (  <_> ) \_\ \___  ||  |__
 \___  >___|  /\___  >__|  |___|  /\____/|___  / ____||____/
     \/     \/     \/           \/           \/\/           
  _____.__                      .__  .__                    
_/ ____\__|______   ____ _____  |  | |  |                   
\   __\|  \_  __ \_/ __ \\__  \ |  | |  |                   
 |  |  |  ||  | \/\  ___/ / __ \|  |_|  |__                 
 |__|  |__||__|    \___  >____  /____/____/                 
                      \/     \/                            

parandom o firewall!
OK -> Limpando todas as  chains
OK ->removendo as chains do user 
OK -> Cadeias internas redefinidas para a diretiva ACCEPT padrão
OK



[darkcode distro]# bash firewall-arch restart
    
       .__                              ___.          .__   
  ____ |  |__   ___________  ____   ____\_ |__ ___.__.|  |  
_/ ___\|  |  \_/ __ \_  __ \/    \ /  _ \| __ <   |  ||  |  
\  \___|   Y  \  ___/|  | \/   |  (  <_> ) \_\ \___  ||  |__
 \___  >___|  /\___  >__|  |___|  /\____/|___  / ____||____/
     \/     \/     \/           \/           \/\/           
  _____.__                      .__  .__                    
_/ ____\__|______   ____ _____  |  | |  |                   
\   __\|  \_  __ \_/ __ \\__  \ |  | |  |                   
 |  |  |  ||  | \/\  ___/ / __ \|  |_|  |__                 
 |__|  |__||__|    \___  >____  /____/____/                 
                      \/     \/                            

-------------------------------------
Firewall!
criador darkcode
proteção para o sistema operacional blackarch
-------------------------------------
Loading modules...
Cleaning up firewall...
OK -> difinindo politicas padrão...
OK -> liberandom o Loopback ...
OK -> proteção contra DOS
OK -> abilitar comunicação com outras interfaces...
====>Bloquear pacotes com estado novo/invalido que saiam pela placa  de rede (eno1/wlan0wlo1/outras)<====
modificar como a sua placa de rede para ter a proteção
====>Bloqueando conexão brute force via SSH:<====
OK -> Conexão SSH aceita (fail2ban abilitado)...
====>PROTEÇÃO CONTRA ATAQUES<====
OK -> bloqueando  attacks...
====>PROTEGE CONTRA PACOTES QUE PODEM PROCURAR E OBTER INFORMAÇÕES INTERNAS<====
OK -> proteção Spy-packages ...
====>BLOQUEANDO TRACEROUTE<====
OK -> bloqueando traceroute...
====>REGRAS DE SEGURANÇA NA INTERNET<====
OK -> regras de segurança na internet...
====>PROTECOES DE KERNEL<====
OK -> proteção para o Kernel ...
====>Portas do user do CH-OS<====
------> Abrindo Portas do Apache
open port tcp 80
open port tcp 443
open port tcp 8080 
-------> Abrindo Portas para DNS
open port udp 53
-------> abrindo porta para o postgresql
open port tcp 5432
-------> Abrindo Portas para MYSQL
open port tcp 3306
open port udp 3306
-------> Abrindo Portas para SSH
open port tcp 2222
open port udp 2222
----------------------
tunelamento ssh ataque
open port tcp 3212
open port tcp 1232
====>PORTAS PARA ATAQUE<====
====>BEEF-XSS<====
open port tcp 3000
open port udp 3000
------->teamserver armitage/cobalt
port open tcp 555554
port open tcp 419
port open tcp 5419
port open udp 5419
port open tcp 519
port open udp 519
------->metasploit<--------
open port 4444
open port 4455
open port 3322
open port 2233
open port 3322
open port 5301
-------> abrindo porta  para beef-xss
====>Proteções Adicionais<====
====>Proteção contra ping da morte<====
====>Proteção contra trinoo<====
OK -> proteção Trinoo ...
====> Proteção contra trojans<====
OK -> proteção contra Trojan ...
====>Proteção contra worms<====
OK -> proteção contra Worm ...
====>Proteção contra port scanners<====
OK -> proteção contra Port Scanner ...
====>BLOQUEANDO PORT SCANNERS OCULTOS<====
OK -> proteção contra porte scanner oculto...
====>BackOrifice<====
OK -> proteção BackOrifice ...
====>NetBus<====
OK -> proteção NetBus ...
====>Ativa mascaramento de saída<====
OK -> mascarando Packages de saida ...

[darkcode distro]# bash firewall-arch status 
    
       .__                              ___.          .__   
  ____ |  |__   ___________  ____   ____\_ |__ ___.__.|  |  
_/ ___\|  |  \_/ __ \_  __ \/    \ /  _ \| __ <   |  ||  |  
\  \___|   Y  \  ___/|  | \/   |  (  <_> ) \_\ \___  ||  |__
 \___  >___|  /\___  >__|  |___|  /\____/|___  / ____||____/
     \/     \/     \/           \/           \/\/           
  _____.__                      .__  .__                    
_/ ____\__|______   ____ _____  |  | |  |                   
\   __\|  \_  __ \_/ __ \\__  \ |  | |  |                   
 |  |  |  ||  | \/\  ___/ / __ \|  |_|  |__                 
 |__|  |__||__|    \___  >____  /____/____/                 
                      \/     \/                            

Chain INPUT (policy DROP)
target     prot opt source               destination         
ACCEPT     all  --  anywhere             anywhere            
ACCEPT     tcp  --  anywhere             anywhere             tcp dpt:EtherNet-IP-1 flags:FIN,SYN,RST,ACK/SYN
DROP       all  --  anywhere             anywhere             state INVALID
DROP       udp  --  anywhere             anywhere             udp dpts:33435:33525
ACCEPT     all  --  anywhere             anywhere             state RELATED,ESTABLISHED
ACCEPT     tcp  --  anywhere             anywhere             tcp dpt:http
ACCEPT     tcp  --  anywhere             anywhere             tcp dpt:https
ACCEPT     tcp  --  anywhere             anywhere             tcp dpt:http-alt
ACCEPT     udp  --  anywhere             anywhere             udp dpt:domain
ACCEPT     tcp  --  anywhere             anywhere             tcp dpt:postgresql
ACCEPT     tcp  --  anywhere             anywhere             tcp dpt:mysql
ACCEPT     udp  --  anywhere             anywhere             udp dpt:mysql
ACCEPT     tcp  --  anywhere             anywhere             tcp dpt:EtherNet-IP-1
ACCEPT     udp  --  anywhere             anywhere             udp dpt:EtherNet-IP-1
ACCEPT     tcp  --  anywhere             anywhere             tcp dpt:surveyinst
ACCEPT     tcp  --  anywhere             anywhere             tcp dpt:first-defense
ACCEPT     tcp  --  anywhere             anywhere             tcp dpt:hbci
ACCEPT     udp  --  anywhere             anywhere             udp dpt:hbci
ACCEPT     tcp  --  anywhere             anywhere             tcp dpt:55554
ACCEPT     tcp  --  anywhere             anywhere             tcp dpt:ariel1
ACCEPT     tcp  --  anywhere             anywhere             tcp dpt:dj-ice
ACCEPT     udp  --  anywhere             anywhere             udp dpt:dj-ice
ACCEPT     tcp  --  anywhere             anywhere             tcp dpt:utime
ACCEPT     udp  --  anywhere             anywhere             udp dpt:utime
ACCEPT     tcp  --  anywhere             anywhere             tcp dpt:krb524
ACCEPT     tcp  --  anywhere             anywhere             tcp dpt:prchat-user
ACCEPT     tcp  --  anywhere             anywhere             tcp dpt:3322
ACCEPT     tcp  --  anywhere             anywhere             tcp dpt:infocrypt
ACCEPT     tcp  --  anywhere             anywhere             tcp dpt:emcads
ACCEPT     tcp  --  anywhere             anywhere             tcp dpt:hacl-gs
ACCEPT     tcp  --  anywhere             anywhere             tcp dpt:hbci
DROP       tcp  --  anywhere             anywhere             tcp dpt:rfb
DROP       tcp  --  anywhere             anywhere             tcp dpt:domain
TRINOO     tcp  --  anywhere             anywhere             tcp dpt:27444
TRINOO     tcp  --  anywhere             anywhere             tcp dpt:27665
TRINOO     tcp  --  anywhere             anywhere             tcp dpt:31335
TRINOO     tcp  --  anywhere             anywhere             tcp dpt:34555
TRINOO     tcp  --  anywhere             anywhere             tcp dpt:35555
TROJAN     tcp  --  anywhere             anywhere             tcp dpt:mdqs
TROJAN     tcp  --  anywhere             anywhere             tcp dpt:terabase
TROJAN     tcp  --  anywhere             anywhere             tcp dpt:x11
TROJAN     tcp  --  anywhere             anywhere             tcp dpt:6006
TROJAN     tcp  --  anywhere             anywhere             tcp dpt:16660
SCANNER    tcp  --  anywhere             anywhere             tcp flags:FIN,SYN,RST,PSH,ACK,URG/FIN,PSH,URG
SCANNER    tcp  --  anywhere             anywhere             tcp flags:FIN,SYN,RST,PSH,ACK,URG/NONE
SCANNER    tcp  --  anywhere             anywhere             tcp flags:FIN,SYN,RST,PSH,ACK,URG/FIN,SYN,RST,PSH,ACK,URG
SCANNER    tcp  --  anywhere             anywhere             tcp flags:FIN,SYN,RST,PSH,ACK,URG/FIN,SYN
SCANNER    tcp  --  anywhere             anywhere             tcp flags:FIN,SYN,RST,PSH,ACK,URG/FIN,SYN,RST,ACK,URG
SCANNER    tcp  --  anywhere             anywhere             tcp flags:SYN,RST/SYN,RST
SCANNER    tcp  --  anywhere             anywhere             tcp flags:FIN,SYN/FIN,SYN
DROP       tcp  --  anywhere             anywhere             tcp dpt:31337
DROP       udp  --  anywhere             anywhere             udp dpt:31337
DROP       tcp  --  anywhere             anywhere             tcp dpts:italk:12346
DROP       udp  --  anywhere             anywhere             udp dpts:italk:12346

Chain FORWARD (policy DROP)
target     prot opt source               destination         
ACCEPT     tcp  --  anywhere             anywhere             tcp flags:FIN,SYN,RST,ACK/SYN limit: avg 1/sec burst 5
DROP       all  --  anywhere             anywhere             state INVALID,NEW
DROP       all  --  anywhere             anywhere             state INVALID,NEW
DROP       tcp  --  anywhere             anywhere             tcp flags:FIN,SYN,RST,PSH,ACK,URG/SYN,ACK
ACCEPT     all  --  anywhere             anywhere             state RELATED,ESTABLISHED
ACCEPT     icmp --  anywhere             anywhere             icmp echo-request limit: avg 1/sec burst 5
REJECT     tcp  --  anywhere             anywhere             tcp dpt:epmap reject-with icmp-port-unreachable
ACCEPT     tcp  --  anywhere             anywhere             tcp flags:FIN,SYN,RST,ACK/RST limit: avg 1/sec burst 5

Chain OUTPUT (policy ACCEPT)
target     prot opt source               destination         

Chain SCANNER (7 references)
target     prot opt source               destination         
LOG        all  --  anywhere             anywhere             limit: avg 15/min burst 5 LOG level info prefix "FIREWALL: port scanner: "
DROP       all  --  anywhere             anywhere            

Chain TRINOO (5 references)
target     prot opt source               destination         
LOG        all  --  anywhere             anywhere             limit: avg 15/min burst 5 LOG level info prefix "FIREWALL: trinoo: "
DROP       all  --  anywhere             anywhere            

Chain TROJAN (5 references)
target     prot opt source               destination         
LOG        all  --  anywhere             anywhere             limit: avg 15/min burst 5 LOG level info prefix "FIREWALL: trojan: "
DROP       all  --  anywhere             anywhere            

[darkcode distro]# bash firewall-arch panic
    
       .__                              ___.          .__   
  ____ |  |__   ___________  ____   ____\_ |__ ___.__.|  |  
_/ ___\|  |  \_/ __ \_  __ \/    \ /  _ \| __ <   |  ||  |  
\  \___|   Y  \  ___/|  | \/   |  (  <_> ) \_\ \___  ||  |__
 \___  >___|  /\___  >__|  |___|  /\____/|___  / ____||____/
     \/     \/     \/           \/           \/\/           
  _____.__                      .__  .__                    
_/ ____\__|______   ____ _____  |  | |  |                   
\   __\|  \_  __ \_/ __ \\__  \ |  | |  |                   
 |  |  |  ||  | \/\  ___/ / __ \|  |_|  |__                 
 |__|  |__||__|    \___  >____  /____/____/                 
                      \/     \/                            

OK -> Mudou as políticas de destino para DROP

OK -> limpando todas as  chains
OK -> removendo todas as chains do user 
OK ->Extremamente modo paranóico [ON] (sim, você pode ser mais paranóico do que a função de início padrão)

[darkcode distro]# bash firewall-arch status 
    
       .__                              ___.          .__   
  ____ |  |__   ___________  ____   ____\_ |__ ___.__.|  |  
_/ ___\|  |  \_/ __ \_  __ \/    \ /  _ \| __ <   |  ||  |  
\  \___|   Y  \  ___/|  | \/   |  (  <_> ) \_\ \___  ||  |__
 \___  >___|  /\___  >__|  |___|  /\____/|___  / ____||____/
     \/     \/     \/           \/           \/\/           
  _____.__                      .__  .__                    
_/ ____\__|______   ____ _____  |  | |  |                   
\   __\|  \_  __ \_/ __ \\__  \ |  | |  |                   
 |  |  |  ||  | \/\  ___/ / __ \|  |_|  |__                 
 |__|  |__||__|    \___  >____  /____/____/                 
                      \/     \/                            

Chain INPUT (policy DROP)
target     prot opt source               destination         

Chain FORWARD (policy DROP)
target     prot opt source               destination         

Chain OUTPUT (policy DROP)
target     prot opt source               destination         

Chain SCANNER (0 references)
target     prot opt source               destination         
LOG        all  --  anywhere             anywhere             limit: avg 15/min burst 5 LOG level info prefix "FIREWALL: port scanner: "
DROP       all  --  anywhere             anywhere            

Chain TRINOO (0 references)
target     prot opt source               destination         
LOG        all  --  anywhere             anywhere             limit: avg 15/min burst 5 LOG level info prefix "FIREWALL: trinoo: "
DROP       all  --  anywhere             anywhere            

Chain TROJAN (0 references)
target     prot opt source               destination         
LOG        all  --  anywhere             anywhere             limit: avg 15/min burst 5 LOG level info prefix "FIREWALL: trojan: "
DROP       all  --  anywhere             anywhere            

[darkcode distro]# bash firewall-arch install 
    
       .__                              ___.          .__   
  ____ |  |__   ___________  ____   ____\_ |__ ___.__.|  |  
_/ ___\|  |  \_/ __ \_  __ \/    \ /  _ \| __ <   |  ||  |  
\  \___|   Y  \  ___/|  | \/   |  (  <_> ) \_\ \___  ||  |__
 \___  >___|  /\___  >__|  |___|  /\____/|___  / ____||____/
     \/     \/     \/           \/           \/\/           
  _____.__                      .__  .__                    
_/ ____\__|______   ____ _____  |  | |  |                   
\   __\|  \_  __ \_/ __ \\__  \ |  | |  |                   
 |  |  |  ||  | \/\  ___/ / __ \|  |_|  |__                 
 |__|  |__||__|    \___  >____  /____/____/                 
                      \/     \/                            

# Generated by iptables-save v1.6.1 on Sun Apr 30 03:40:41 2017
*mangle
:PREROUTING ACCEPT [1150:180583]
:INPUT ACCEPT [950:125538]
:FORWARD ACCEPT [0:0]
:OUTPUT ACCEPT [2063:147577]
:POSTROUTING ACCEPT [936:65090]
COMMIT
# Completed on Sun Apr 30 03:40:41 2017
# Generated by iptables-save v1.6.1 on Sun Apr 30 03:40:41 2017
*nat
:PREROUTING ACCEPT [205:55319]
:INPUT ACCEPT [0:0]
:OUTPUT ACCEPT [1907:138499]
:POSTROUTING ACCEPT [819:59166]
-A POSTROUTING -o wlan0wlo1 -j MASQUERADE
COMMIT
# Completed on Sun Apr 30 03:40:41 2017
# Generated by iptables-save v1.6.1 on Sun Apr 30 03:40:41 2017
*filter
:INPUT DROP [12:9119]
:FORWARD DROP [0:0]
:OUTPUT DROP [1127:82487]
:SCANNER - [0:0]
:TRINOO - [0:0]
:TROJAN - [0:0]
-A SCANNER -m limit --limit 15/min -j LOG --log-prefix "FIREWALL: port scanner: " --log-level 6
-A SCANNER -j DROP
-A TRINOO -m limit --limit 15/min -j LOG --log-prefix "FIREWALL: trinoo: " --log-level 6
-A TRINOO -j DROP
-A TROJAN -m limit --limit 15/min -j LOG --log-prefix "FIREWALL: trojan: " --log-level 6
-A TROJAN -j DROP
COMMIT
# Completed on Sun Apr 30 03:40:41 2017
```

