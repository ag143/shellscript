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
Linux 5.13.0-1022-azure (fv-az243-492) 	05/09/22 	_x86_64_	(2 CPU)

avg-cpu:  %user   %nice %system %iowait  %steal   %idle
           3.61    0.06    3.32    0.53    0.00   92.49

Device             tps    kB_read/s    kB_wrtn/s    kB_dscd/s    kB_read    kB_wrtn    kB_dscd
loop0             1.05         9.38         0.00         0.00       2250          0          0
loop1             0.28         4.59         0.00         0.00       1100          0          0
loop2             3.49       132.24         0.00         0.00      31714          0          0
loop3             0.05         0.06         0.00         0.00         14          0          0
sda             185.26      3303.30       657.88    125022.51     792229     157780   29984149
sdb               4.65        51.94      1249.45    103390.85      12457     299656   24796228


***************************************************************************************************************************************************************
- sar
***************************************************************************************************************************************************************
- vmstat
procs -----------memory---------- ---swap-- -----io---- -system-- ------cpu-----
 r  b   swpd   free   buff  cache   si   so    bi    bo   in   cs us sy id wa st
 1  0      0 5361924 209456 1035136    0    0  1761   959   87  510  4  3 92  1  0
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
/dev/root       87218124 55270576  31931164  64% /
devtmpfs         3552992        0   3552992   0% /dev
tmpfs            3556564        4   3556560   1% /dev/shm
tmpfs             711316     1072    710244   1% /run
tmpfs               5120        0      5120   0% /run/lock
tmpfs            3556564        0   3556564   0% /sys/fs/cgroup
/dev/loop0         63488    63488         0 100% /snap/core20/1405
/dev/loop1         69504    69504         0 100% /snap/lxd/22753
/dev/loop2         44800    44800         0 100% /snap/snapd/15177
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
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 5522
;; flags: qr rd ra; QUERY: 1, ANSWER: 13, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 65494
;; QUESTION SECTION:
;.				IN	NS

;; ANSWER SECTION:
.			517229	IN	NS	l.root-servers.net.
.			517229	IN	NS	k.root-servers.net.
.			517229	IN	NS	m.root-servers.net.
.			517229	IN	NS	d.root-servers.net.
.			517229	IN	NS	b.root-servers.net.
.			517229	IN	NS	e.root-servers.net.
.			517229	IN	NS	i.root-servers.net.
.			517229	IN	NS	f.root-servers.net.
.			517229	IN	NS	h.root-servers.net.
.			517229	IN	NS	c.root-servers.net.
.			517229	IN	NS	g.root-servers.net.
.			517229	IN	NS	a.root-servers.net.
.			517229	IN	NS	j.root-servers.net.

;; Query time: 0 msec
;; SERVER: 127.0.0.53#53(127.0.0.53)
;; WHEN: Mon May 09 12:26:03 UTC 2022
;; MSG SIZE  rcvd: 239

***************************************************************************************************************************************************************
- iptables
***************************************************************************************************************************************************************
- netstat
Active Internet connections (w/o servers)
Proto Recv-Q Send-Q Local Address           Foreign Address         State      
tcp        0      0 fv-az243-492.eyhn:40600 lb-140-82-112-4-i:https TIME_WAIT  
tcp6       0      0 fv-az243-492.eyhn:44780 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az243-492.eyhn:44794 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az243-492.eyhn:60386 lb-140-82-113-5-i:https TIME_WAIT  
tcp6       0      0 fv-az243-492.eyhn:44786 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az243-492.eyhn:44792 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az243-492.eyhn:44790 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az243-492.eyhn:44782 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az243-492.eyhn:48012 lb-140-82-113-10-:https TIME_WAIT  
tcp6       0      0 fv-az243-492.eyhn:44784 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az243-492.eyhn:44778 13.107.42.16:https      ESTABLISHED
Active UNIX domain sockets (w/o servers)
Proto RefCnt Flags       Type       State         I-Node   Path
unix  3      [ ]         DGRAM                    14245    /run/systemd/notify
unix  2      [ ]         DGRAM                    14262    /run/systemd/journal/syslog
unix  8      [ ]         DGRAM                    14272    /run/systemd/journal/dev-log
unix  8      [ ]         DGRAM                    14276    /run/systemd/journal/socket
unix  2      [ ]         DGRAM                    24168    /run/chrony/chronyd.sock
unix  2      [ ]         DGRAM                    30231    @00014
unix  3      [ ]         STREAM     CONNECTED     22887    /run/dbus/system_bus_socket
unix  2      [ ]         DGRAM                    23277    
unix  3      [ ]         STREAM     CONNECTED     19243    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     21141    
unix  3      [ ]         STREAM     CONNECTED     26804    
unix  3      [ ]         STREAM     CONNECTED     25634    
unix  3      [ ]         SEQPACKET  CONNECTED     24169    
unix  2      [ ]         DGRAM                    611      
unix  3      [ ]         STREAM     CONNECTED     26379    
unix  2      [ ]         DGRAM                    32850    
unix  3      [ ]         STREAM     CONNECTED     26805    
unix  3      [ ]         DGRAM                    14247    
unix  3      [ ]         STREAM     CONNECTED     26387    
unix  2      [ ]         DGRAM                    15569    
unix  3      [ ]         STREAM     CONNECTED     24409    
unix  3      [ ]         STREAM     CONNECTED     24443    /run/dbus/system_bus_socket
unix  3      [ ]         DGRAM                    19863    
unix  3      [ ]         STREAM     CONNECTED     32290    
unix  3      [ ]         DGRAM                    18487    
unix  3      [ ]         DGRAM                    14246    
unix  3      [ ]         STREAM     CONNECTED     21194    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22299    
unix  2      [ ]         DGRAM                    30240    
unix  3      [ ]         STREAM     CONNECTED     931      
unix  3      [ ]         STREAM     CONNECTED     22883    
unix  3      [ ]         DGRAM                    19864    
unix  3      [ ]         STREAM     CONNECTED     19267    
unix  3      [ ]         STREAM     CONNECTED     23558    
unix  3      [ ]         STREAM     CONNECTED     22885    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     24411    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22565    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     21195    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22882    
unix  3      [ ]         DGRAM                    19865    
unix  3      [ ]         STREAM     CONNECTED     22875    
unix  3      [ ]         STREAM     CONNECTED     21903    
unix  3      [ ]         STREAM     CONNECTED     24229    /run/systemd/journal/stdout
unix  3      [ ]         DGRAM                    15121    
unix  3      [ ]         STREAM     CONNECTED     24299    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22795    
unix  3      [ ]         STREAM     CONNECTED     18119    
unix  3      [ ]         STREAM     CONNECTED     30256    /run/containerd/containerd.sock
unix  2      [ ]         DGRAM                    19272    
unix  3      [ ]         STREAM     CONNECTED     22886    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     20376    
unix  3      [ ]         STREAM     CONNECTED     21551    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     23724    
unix  3      [ ]         STREAM     CONNECTED     21192    
unix  3      [ ]         STREAM     CONNECTED     26194    /run/dbus/system_bus_socket
unix  3      [ ]         SEQPACKET  CONNECTED     24170    
unix  3      [ ]         STREAM     CONNECTED     24244    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     21379    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     26388    
unix  3      [ ]         STREAM     CONNECTED     22884    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     26771    
unix  3      [ ]         STREAM     CONNECTED     24184    
unix  3      [ ]         STREAM     CONNECTED     21293    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     20377    
unix  3      [ ]         STREAM     CONNECTED     22888    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     15561    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM                    14547    
unix  2      [ ]         DGRAM                    25627    
unix  3      [ ]         STREAM     CONNECTED     30253    /run/containerd/containerd.sock
unix  3      [ ]         STREAM     CONNECTED     24240    /run/systemd/journal/stdout
unix  3      [ ]         DGRAM                    19862    
unix  3      [ ]         STREAM     CONNECTED     24641    
unix  3      [ ]         STREAM     CONNECTED     16621    
unix  2      [ ]         DGRAM                    21142    
unix  3      [ ]         STREAM     CONNECTED     25635    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     30255    
unix  3      [ ]         STREAM     CONNECTED     22060    
unix  2      [ ]         DGRAM                    940      
unix  2      [ ]         DGRAM                    24433    
unix  3      [ ]         STREAM     CONNECTED     26243    
unix  3      [ ]         DGRAM                    15120    
unix  3      [ ]         STREAM     CONNECTED     32291    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     17080    
unix  2      [ ]         DGRAM                    22881    
unix  2      [ ]         DGRAM                    19858    
unix  3      [ ]         STREAM     CONNECTED     22793    
unix  3      [ ]         STREAM     CONNECTED     21550    
unix  3      [ ]         STREAM     CONNECTED     30252    
unix  3      [ ]         STREAM     CONNECTED     26921    
unix  3      [ ]         DGRAM                    18488    
unix  2      [ ]         DGRAM                    23181    
unix  3      [ ]         STREAM     CONNECTED     24442    
unix  3      [ ]         STREAM     CONNECTED     15127    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     26378    
unix  2      [ ]         DGRAM                    24143    
unix  3      [ ]         STREAM     CONNECTED     24020    
unix  3      [ ]         STREAM     CONNECTED     20007    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     21068    
unix  3      [ ]         STREAM     CONNECTED     26242    
unix  3      [ ]         STREAM     CONNECTED     19856    
unix  3      [ ]         STREAM     CONNECTED     21745    
unix  3      [ ]         STREAM     CONNECTED     23374    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     24242    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     26923    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     16066    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     24243    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     18139    /run/systemd/journal/stdout
***************************************************************************************************************************************************************
###############################################################################################################################################################
## process Monitoring(ps,top,htop,atop,lsof)
- ps
    PID TTY          TIME CMD
   1512 ?        00:00:02 Runner.Listener
   1527 ?        00:00:03 Runner.Worker
   1634 ?        00:00:00 bash
   1659 ?        00:00:00 sh
   1681 ?        00:00:00 ps
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
