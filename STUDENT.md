student@programming-lab:~$ pwd
/home/student
student@programming-lab:~$ man ifconfig
student@programming-lab:~$ man ifconfig
student@programming-lab:~$ 
student@programming-lab:~$ man ifconfig
student@programming-lab:~$ man ifconfig
student@programming-lab:~$ man ifconfig -a
No manual entry for -a
student@programming-lab:~$ ifconfig -a
enp1s0: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500
        ether d0:ad:08:55:8d:a6  txqueuelen 1000  (Ethernet)
        RX packets 18840  bytes 4134960 (4.1 MB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 440  bytes 78534 (78.5 KB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

lo: flags=73<UP,LOOPBACK,RUNNING>  mtu 65536
        inet 127.0.0.1  netmask 255.0.0.0
        inet6 ::1  prefixlen 128  scopeid 0x10<host>
        loop  txqueuelen 1000  (Local Loopback)
        RX packets 34496  bytes 2671213 (2.6 MB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 34496  bytes 2671213 (2.6 MB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

student@programming-lab:~$ ifconfig -s
Iface      MTU    RX-OK RX-ERR RX-DRP RX-OVR    TX-OK TX-ERR TX-DRP TX-OVR Flg
enp1s0           1500    18850      0      0 0           440      0      0      0 BMRU
lo              65536    34496      0      0 0         34496      0      0      0 LRU
student@programming-lab:~$ ifconfig -v
enp1s0: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500
        ether d0:ad:08:55:8d:a6  txqueuelen 1000  (Ethernet)
        RX packets 18861  bytes 4140331 (4.1 MB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 440  bytes 78534 (78.5 KB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

lo: flags=73<UP,LOOPBACK,RUNNING>  mtu 65536
        inet 127.0.0.1  netmask 255.0.0.0
        inet6 ::1  prefixlen 128  scopeid 0x10<host>
        loop  txqueuelen 1000  (Local Loopback)
        RX packets 34496  bytes 2671213 (2.6 MB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 34496  bytes 2671213 (2.6 MB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

student@programming-lab:~$ top

top - 13:48:13 up 42 min,  1 user,  load average: 0.09, 0.16, 0.29
Tasks: 276 total,   1 running, 275 sleeping,   0 stopped,   0 zombie
%Cpu(s):  0.3 us,  0.2 sy,  0.0 ni, 99.4 id,  0.1 wa,  0.0 hi,  0.0 si,  0.0 st 
MiB Mem : 63.8/3604.5   [||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||                                    ] 
MiB Swap:  0.0/3604.0   [                                                                                                    ] 
Maximum tasks = 0, change to (0 is unlimited) 
    PID USER      PR  NI    VIRT    RES    SHR S  %CPU  %MEM     TIME+ COMMAND                                                                          
    496 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker/R-ttm                                                                    
    497 root     -51   0       0      0      0 S   0.0   0.0   0:00.00 card1-crtc0                                                                      
    498 root     -51   0       0      0      0 S   0.0   0.0   0:00.00 card1-crtc1                                                                      
    499 root     -51   0       0      0      0 S   0.0   0.0   0:00.00 card1-crtc2                                                                      
    500 root     -51   0       0      0      0 S   0.0   0.0   0:00.00 card1-crtc3                                                                      
    560 root      20   0       0      0      0 I   0.0   0.0   0:00.38 kworker/u32:12-kvfree_rcu_reclaim                                                
    565 root       0 -20       0      0      0 I   0.0   0.0   0:00.00 kworker/R-cryptd                                                                 
    890 systemd+  20   0   21592  13260  10956 S   0.0   0.4   0:00.71 systemd-resolve                                                                  
    891 systemd+  20   0   91052   7856   6880 S   0.0   0.2   0:00.25 systemd-timesyn                                                                  
   1060 message+  20   0   12188   7316   4628 S   0.0   0.2   0:00.89 dbus-daemon                                                                      
   1065 gnome-r+  20   0  439216  16640  14120 S   0.0   0.5   0:00.04 gnome-remote-de                                                                  
   1069 polkitd   20   0  384904  11424   7800 S   0.0   0.3   0:00.55 polkitd                                                                          
   1070 root      20   0  313508   7992   7168 S   0.0   0.2   0:00.03 power-profiles-                                                                  
   1074 root      20   0 2292640  40112  25140 S   0.0   1.1   0:01.07 snapd                                                                            
   1075 root      20   0  313556   8060   6952 S   0.0   0.2   0:00.19 accounts-daemon                                                                  
   1076 root      20   0    9424   2896   2652 S   0.0   0.1   0:00.00 cron                                                                             
   1077 root      20   0  309720   6808   6256 S   0.0   0.2   0:00.03 switcheroo-cont                                                                  
   1079 root      20   0   18132   9244   7960 S   0.0   0.3   0:00.17 systemd-logind                                                                   
   1080 root      20   0  424868  11324  10304 S   0.0   0.3   0:00.17 thermald                                                                         
   1081 root      20   0  469840  15176  11464 S   0.0   0.4   0:00.30 udisksd                                                                          
   1085 avahi     20   0    8480   1520   1152 S   0.0   0.0   0:00.00 avahi-daemon                                                                     
   1103 syslog    20   0  222564   6552   4612 S   0.0   0.2   0:00.19 rsyslogd                                                                         
   1269 root      20   0  336236  18748  15912 S   0.0   0.5   0:00.32 NetworkManager                                                                   
   1270 root      20   0   17384   6496   5620 S   0.0   0.2   0:00.02 wpa_supplicant                                                                   
   1307 root      20   0  318356  12872  10808 S   0.0   0.3   0:00.05 ModemManager                                                                     
   1447 root      20   0   38348  12076   9824 S   0.0   0.3   0:00.02 cupsd                                                                            
   1451 root      20   0  118032  25108  15192 S   0.0   0.7   0:00.06 unattended-upgr                                                                  
   1465 root      20   0  314808   9440   8324 S   0.0   0.3   0:00.02 gdm3                                                                             
   1483 root      -2   0       0      0      0 S   0.0   0.0   0:00.00 psimon                                                                           
   1534 rtkit     21   1   22940   3552   3248 S   0.0   0.1   0:00.05 rtkit-daemon                                                                     
[1]+  Stopped                 top
student@programming-lab:~$ man top
student@programming-lab:~$ man ifconfig
student@programming-lab:~$ man ip
student@programming-lab:~$ ip -a s a up
Error: argument "a" is wrong: unknown
student@programming-lab:~$ ip -a s -a up
Error: argument "-a" is wrong: unknown
student@programming-lab:~$ ip -s a s up
1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN group default qlen 1000
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
    inet 127.0.0.1/8 scope host lo
       valid_lft forever preferred_lft forever
    inet6 ::1/128 scope host noprefixroute 
       valid_lft forever preferred_lft forever
    RX:  bytes packets errors dropped  missed   mcast           
       3120073   40427      0       0       0       0 
    TX:  bytes packets errors dropped carrier collsns           
       3120073   40427      0       0       0       0 
2: enp1s0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc pfifo_fast state UP group default qlen 1000
    link/ether d0:ad:08:55:8d:a6 brd ff:ff:ff:ff:ff:ff
    inet 10.10.1.87/16 brd 10.10.255.255 scope global dynamic noprefixroute enp1s0
       valid_lft 27743sec preferred_lft 27743sec
    inet6 fe80::76ee:77e2:368a:580b/64 scope link noprefixroute 
       valid_lft forever preferred_lft forever
    RX:  bytes packets errors dropped  missed   mcast           
      20012210   45261      0      18       0    6024 
    TX:  bytes packets errors dropped carrier collsns           
       1305907    6090      0       0       0       0 
student@programming-lab:~$ who is
student@programming-lab:~$ who is www.google.com
student@programming-lab:~$ who is googe.com
student@programming-lab:~$ whois www.google.com
Command 'whois' not found, but can be installed with:
apt install whois
Please ask your administrator.
student@programming-lab:~$ apt install whois
E: Could not open lock file /var/lib/dpkg/lock-frontend - open (13: Permission denied)
E: Unable to acquire the dpkg frontend lock (/var/lib/dpkg/lock-frontend), are you root?

