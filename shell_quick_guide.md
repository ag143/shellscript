## learn Bash scripting
## VIM/NANO/Poershell/Emacs
## Compiling apps from source(gcc,make)
###############################################################################################################################################################
## System performance(nmon,iostat,sar,vmstat)
- nmon
***************************************************************************************************************************************************************
- nmon
***************************************************************************************************************************************************************
- iostat
Linux 5.13.0-1022-azure (fv-az246-872) 	05/09/22 	_x86_64_	(2 CPU)

avg-cpu:  %user   %nice %system %iowait  %steal   %idle
          20.91    0.43   20.10    2.11    0.00   56.45

Device             tps    kB_read/s    kB_wrtn/s    kB_dscd/s    kB_read    kB_wrtn    kB_dscd
loop0            29.82      1130.35         0.00         0.00      34679          0          0
loop1             8.21        72.75         0.00         0.00       2232          0          0
loop2             2.22        35.85         0.00         0.00       1100          0          0
loop3             0.36         0.46         0.00         0.00         14          0          0
sda            1412.74     25799.27      3473.68    978002.38     791521     106572   30005113
sdb              36.86       424.02      9765.32    808221.25      13009     299600   24796228


***************************************************************************************************************************************************************
- sar
***************************************************************************************************************************************************************
- vmstat
procs -----------memory---------- ---swap-- -----io---- -system-- ------cpu-----
 r  b   swpd   free   buff  cache   si   so    bi    bo   in   cs us sy id wa st
 0  0      0 5359852 209272 1036044    0    0 14015  6753  699 3559 21 20 56  2  0
***************************************************************************************************************************************************************
###############################################################################################################################################################
## others(strace,dtrace,systemtap,uname,df,history)
- strace
***************************************************************************************************************************************************************
- dtrace
***************************************************************************************************************************************************************
- systemtap
***************************************************************************************************************************************************************
- uname
Linux
***************************************************************************************************************************************************************
- df
Filesystem     1K-blocks     Used Available Use% Mounted on
/dev/root       87218124 55270716  31931024  64% /
devtmpfs         3552992        0   3552992   0% /dev
tmpfs            3556564        4   3556560   1% /dev/shm
tmpfs             711316     1080    710236   1% /run
tmpfs               5120        0      5120   0% /run/lock
tmpfs            3556564        0   3556564   0% /sys/fs/cgroup
/dev/loop0         44800    44800         0 100% /snap/snapd/15177
/dev/loop1         63488    63488         0 100% /snap/core20/1405
/dev/loop2         69504    69504         0 100% /snap/lxd/22753
/dev/sda15        106858     5321    101537   5% /boot/efi
/dev/sdb1       14382088  4235296   9396508  32% /mnt
***************************************************************************************************************************************************************
- history
***************************************************************************************************************************************************************
###############################################################################################################################################################
## network(nmap,tcpdump,ping,mtr,traceroute,digariman,airodump,dig,iptables,netstat)
- nmap
***************************************************************************************************************************************************************
- tcpdump
***************************************************************************************************************************************************************
- ping
***************************************************************************************************************************************************************
- mtr
***************************************************************************************************************************************************************
- traceroute
***************************************************************************************************************************************************************
- digariman
***************************************************************************************************************************************************************
- airodump
***************************************************************************************************************************************************************
- dig

; <<>> DiG 9.16.1-Ubuntu <<>>
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 56829
;; flags: qr rd ra; QUERY: 1, ANSWER: 13, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 65494
;; QUESTION SECTION:
;.				IN	NS

;; ANSWER SECTION:
.			516921	IN	NS	d.root-servers.net.
.			516921	IN	NS	i.root-servers.net.
.			516921	IN	NS	b.root-servers.net.
.			516921	IN	NS	l.root-servers.net.
.			516921	IN	NS	g.root-servers.net.
.			516921	IN	NS	e.root-servers.net.
.			516921	IN	NS	j.root-servers.net.
.			516921	IN	NS	h.root-servers.net.
.			516921	IN	NS	m.root-servers.net.
.			516921	IN	NS	a.root-servers.net.
.			516921	IN	NS	k.root-servers.net.
.			516921	IN	NS	c.root-servers.net.
.			516921	IN	NS	f.root-servers.net.

;; Query time: 4 msec
;; SERVER: 127.0.0.53#53(127.0.0.53)
;; WHEN: Mon May 09 12:41:10 UTC 2022
;; MSG SIZE  rcvd: 239

***************************************************************************************************************************************************************
- iptables
***************************************************************************************************************************************************************
- netstat
Active Internet connections (w/o servers)
Proto Recv-Q Send-Q Local Address           Foreign Address         State      
tcp        0      0 fv-az246-872.py5d:34894 lb-140-82-113-4-i:https TIME_WAIT  
tcp        0      0 fv-az246-872.py5d:34472 168.63.129.16:http      TIME_WAIT  
tcp        0      0 fv-az246-872.py5d:34470 168.63.129.16:http      TIME_WAIT  
tcp        0      0 fv-az246-872.py5d:58460 169.254.169.254:http    TIME_WAIT  
tcp6       0      0 fv-az246-872.py5d:46792 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az246-872.py5d:46802 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az246-872.py5d:46800 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az246-872.py5d:46788 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az246-872.py5d:46798 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az246-872.py5d:58682 lb-140-82-112-5-i:https TIME_WAIT  
tcp6       0      0 fv-az246-872.py5d:46790 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az246-872.py5d:46794 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az246-872.py5d:46796 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az246-872.py5d:40854 lb-140-82-114-10-:https TIME_WAIT  
Active UNIX domain sockets (w/o servers)
Proto RefCnt Flags       Type       State         I-Node   Path
unix  3      [ ]         DGRAM                    14173    /run/systemd/notify
unix  2      [ ]         DGRAM                    14190    /run/systemd/journal/syslog
unix  8      [ ]         DGRAM                    14200    /run/systemd/journal/dev-log
unix  10     [ ]         DGRAM                    14204    /run/systemd/journal/socket
unix  2      [ ]         DGRAM                    24266    /run/chrony/chronyd.sock
unix  2      [ ]         DGRAM                    27915    @00014
unix  3      [ ]         STREAM     CONNECTED     14879    
unix  2      [ ]         DGRAM                    21474    
unix  3      [ ]         STREAM     CONNECTED     25332    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     24507    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     26772    
unix  2      [ ]         DGRAM                    14496    
unix  3      [ ]         STREAM     CONNECTED     31452    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     24508    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM                    24257    
unix  3      [ ]         STREAM     CONNECTED     16752    
unix  3      [ ]         STREAM     CONNECTED     22735    
unix  3      [ ]         STREAM     CONNECTED     20173    
unix  3      [ ]         STREAM     CONNECTED     27346    
unix  2      [ ]         DGRAM                    25324    
unix  3      [ ]         STREAM     CONNECTED     23671    
unix  3      [ ]         STREAM     CONNECTED     20712    
unix  3      [ ]         STREAM     CONNECTED     24480    
unix  3      [ ]         STREAM     CONNECTED     21389    
unix  2      [ ]         DGRAM                    14888    
unix  3      [ ]         STREAM     CONNECTED     28463    
unix  3      [ ]         STREAM     CONNECTED     21041    
unix  3      [ ]         STREAM     CONNECTED     25647    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22307    
unix  2      [ ]         DGRAM                    943      
unix  3      [ ]         STREAM     CONNECTED     21478    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     26057    
unix  3      [ ]         STREAM     CONNECTED     22895    
unix  3      [ ]         STREAM     CONNECTED     27935    /run/containerd/containerd.sock
unix  3      [ ]         STREAM     CONNECTED     27009    
unix  3      [ ]         STREAM     CONNECTED     26757    
unix  2      [ ]         DGRAM                    20083    
unix  3      [ ]         STREAM     CONNECTED     24235    
unix  3      [ ]         STREAM     CONNECTED     27937    
unix  3      [ ]         STREAM     CONNECTED     15098    /run/systemd/journal/stdout
unix  3      [ ]         DGRAM                    14174    
unix  3      [ ]         STREAM     CONNECTED     26056    
unix  3      [ ]         STREAM     CONNECTED     941      
unix  3      [ ]         STREAM     CONNECTED     21044    
unix  3      [ ]         STREAM     CONNECTED     19046    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     24259    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     22385    
unix  3      [ ]         STREAM     CONNECTED     20960    
unix  3      [ ]         DGRAM                    20088    
unix  2      [ ]         DGRAM                    24261    
unix  2      [ ]         DGRAM                    16296    
unix  3      [ ]         STREAM     CONNECTED     25695    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     25664    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     25638    /run/systemd/journal/stdout
unix  3      [ ]         DGRAM                    20087    
unix  3      [ ]         STREAM     CONNECTED     26722    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     17304    /run/systemd/journal/stdout
unix  3      [ ]         SEQPACKET  CONNECTED     24267    
unix  3      [ ]         STREAM     CONNECTED     16290    
unix  3      [ ]         DGRAM                    14890    
unix  3      [ ]         STREAM     CONNECTED     21475    
unix  3      [ ]         STREAM     CONNECTED     31441    
unix  3      [ ]         STREAM     CONNECTED     28464    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     24564    /run/systemd/journal/stdout
unix  3      [ ]         SEQPACKET  CONNECTED     24268    
unix  3      [ ]         STREAM     CONNECTED     20885    
unix  3      [ ]         DGRAM                    14891    
unix  3      [ ]         STREAM     CONNECTED     24574    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     28367    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     25644    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     21477    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     21913    
unix  3      [ ]         DGRAM                    14175    
unix  3      [ ]         STREAM     CONNECTED     24258    
unix  3      [ ]         STREAM     CONNECTED     19128    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     21479    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     942      /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     31451    
unix  3      [ ]         STREAM     CONNECTED     30719    /run/containerd/containerd.sock
unix  3      [ ]         STREAM     CONNECTED     17432    /run/systemd/journal/stdout
unix  3      [ ]         DGRAM                    20089    
unix  3      [ ]         STREAM     CONNECTED     27934    
unix  3      [ ]         STREAM     CONNECTED     26756    
unix  3      [ ]         STREAM     CONNECTED     23672    /run/dbus/system_bus_socket
unix  2      [ ]         DGRAM                    735      
unix  3      [ ]         STREAM     CONNECTED     26721    
unix  3      [ ]         STREAM     CONNECTED     18321    
unix  3      [ ]         DGRAM                    17300    
unix  2      [ ]         DGRAM                    30682    
unix  3      [ ]         STREAM     CONNECTED     23210    
unix  3      [ ]         STREAM     CONNECTED     27008    
unix  2      [ ]         DGRAM                    24153    
unix  3      [ ]         STREAM     CONNECTED     21994    
unix  3      [ ]         DGRAM                    20090    
unix  3      [ ]         STREAM     CONNECTED     22736    
unix  3      [ ]         STREAM     CONNECTED     25697    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     24482    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM                    31727    
unix  3      [ ]         DGRAM                    17299    
unix  3      [ ]         STREAM     CONNECTED     27348    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM                    23667    
unix  2      [ ]         DGRAM                    20178    
unix  3      [ ]         STREAM     CONNECTED     20081    
unix  3      [ ]         STREAM     CONNECTED     22153    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     26773    
unix  3      [ ]         STREAM     CONNECTED     25331    
unix  3      [ ]         STREAM     CONNECTED     23665    
unix  3      [ ]         STREAM     CONNECTED     21480    /run/dbus/system_bus_socket
unix  2      [ ]         DGRAM                    31449    
unix  3      [ ]         STREAM     CONNECTED     21476    
unix  3      [ ]         STREAM     CONNECTED     15522    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM                    21916    
unix  3      [ ]         STREAM     CONNECTED     25641    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     25646    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     20713    
***************************************************************************************************************************************************************
###############################################################################################################################################################
## process Monitoring(ps,top,htop,atop,lsof)
- ps
    PID TTY          TIME CMD
   1440 ?        00:00:01 Runner.Listener
   1456 ?        00:00:02 Runner.Worker
   1563 ?        00:00:00 bash
   1590 ?        00:00:00 sh
   1614 ?        00:00:00 ps
***************************************************************************************************************************************************************
- top
***************************************************************************************************************************************************************
- htop
***************************************************************************************************************************************************************
- atop
***************************************************************************************************************************************************************
- lsof
***************************************************************************************************************************************************************
###############################################################################################################################################################
## Text Manipulation TOols(awk,sed,grep,sort,uniq,cat,cut,echo,frmt,tr,nl,egrep,fgrep,wc)
- awk
***************************************************************************************************************************************************************
- sed
***************************************************************************************************************************************************************
- grep
***************************************************************************************************************************************************************
- sort
***************************************************************************************************************************************************************
- uniq
***************************************************************************************************************************************************************
- cat
***************************************************************************************************************************************************************
- cut
***************************************************************************************************************************************************************
- echo

***************************************************************************************************************************************************************
- frmt
***************************************************************************************************************************************************************
- tr
***************************************************************************************************************************************************************
- nl
***************************************************************************************************************************************************************
- egrep
***************************************************************************************************************************************************************
- fgrep
***************************************************************************************************************************************************************
- wc
      0       0       0
***************************************************************************************************************************************************************
