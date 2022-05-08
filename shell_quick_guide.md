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
Linux 5.13.0-1022-azure (fv-az252-768) 	05/08/22 	_x86_64_	(2 CPU)

avg-cpu:  %user   %nice %system %iowait  %steal   %idle
           4.01    0.07    3.48    0.75    0.00   91.69

Device             tps    kB_read/s    kB_wrtn/s    kB_dscd/s    kB_read    kB_wrtn    kB_dscd
loop0             0.41         6.64         0.00         0.00       1100          0          0
loop1             4.99       189.37         0.00         0.00      31364          0          0
loop2             1.52        13.14         0.00         0.00       2176          0          0
loop3             0.07         0.08         0.00         0.00         14          0          0
sda               6.23        72.27      1809.35     88624.66      11969     299664   14678016
sdb             260.02      4781.88       946.68        46.83     791974     156788       7756


***************************************************************************************************************************************************************
- sar
***************************************************************************************************************************************************************
- vmstat
procs -----------memory---------- ---swap-- -----io---- -system-- ------cpu-----
 r  b   swpd   free   buff  cache   si   so    bi    bo   in   cs us sy id wa st
 1  0      0 5375820 207832 1024032    0    0  2546  1385  125  739  4  3 92  1  0
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
/dev/root       87218124 55263008  31938732  64% /
devtmpfs         3552992        0   3552992   0% /dev
tmpfs            3556564        4   3556560   1% /dev/shm
tmpfs             711316     1072    710244   1% /run
tmpfs               5120        0      5120   0% /run/lock
tmpfs            3556564        0   3556564   0% /sys/fs/cgroup
/dev/loop0         69504    69504         0 100% /snap/lxd/22753
/dev/loop1         44800    44800         0 100% /snap/snapd/15177
/dev/loop2         63488    63488         0 100% /snap/core20/1405
/dev/sdb15        106858     5321    101537   5% /boot/efi
/dev/sda1       14382088  4235296   9396508  32% /mnt
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
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 33545
;; flags: qr rd ra; QUERY: 1, ANSWER: 13, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 65494
;; QUESTION SECTION:
;.				IN	NS

;; ANSWER SECTION:
.			518280	IN	NS	b.root-servers.net.
.			518280	IN	NS	d.root-servers.net.
.			518280	IN	NS	e.root-servers.net.
.			518280	IN	NS	l.root-servers.net.
.			518280	IN	NS	a.root-servers.net.
.			518280	IN	NS	c.root-servers.net.
.			518280	IN	NS	g.root-servers.net.
.			518280	IN	NS	f.root-servers.net.
.			518280	IN	NS	i.root-servers.net.
.			518280	IN	NS	m.root-servers.net.
.			518280	IN	NS	k.root-servers.net.
.			518280	IN	NS	h.root-servers.net.
.			518280	IN	NS	j.root-servers.net.

;; Query time: 4 msec
;; SERVER: 127.0.0.53#53(127.0.0.53)
;; WHEN: Sun May 08 09:56:34 UTC 2022
;; MSG SIZE  rcvd: 239

***************************************************************************************************************************************************************
- iptables
***************************************************************************************************************************************************************
- netstat
Active Internet connections (w/o servers)
Proto Recv-Q Send-Q Local Address           Foreign Address         State      
tcp        0      0 fv-az252-768.0oqg:32874 lb-140-82-112-3-i:https TIME_WAIT  
tcp6       0      0 fv-az252-768.0oqg:52374 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az252-768.0oqg:52378 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az252-768.0oqg:52370 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az252-768.0oqg:52382 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az252-768.0oqg:52380 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az252-768.0oqg:36004 lb-140-82-114-9-i:https TIME_WAIT  
tcp6       0      0 fv-az252-768.0oqg:52372 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az252-768.0oqg:52368 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az252-768.0oqg:48462 lb-140-82-113-5-i:https TIME_WAIT  
Active UNIX domain sockets (w/o servers)
Proto RefCnt Flags       Type       State         I-Node   Path
unix  3      [ ]         DGRAM                    1382     /run/systemd/notify
unix  2      [ ]         DGRAM                    1399     /run/systemd/journal/syslog
unix  8      [ ]         DGRAM                    1409     /run/systemd/journal/dev-log
unix  8      [ ]         DGRAM                    1413     /run/systemd/journal/socket
unix  2      [ ]         DGRAM                    22646    /run/chrony/chronyd.sock
unix  2      [ ]         DGRAM                    30909    @00014
unix  3      [ ]         STREAM     CONNECTED     18526    
unix  3      [ ]         STREAM     CONNECTED     22288    /run/dbus/system_bus_socket
unix  3      [ ]         DGRAM                    15081    
unix  3      [ ]         DGRAM                    18097    
unix  3      [ ]         STREAM     CONNECTED     25740    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     26896    
unix  3      [ ]         STREAM     CONNECTED     21003    
unix  3      [ ]         STREAM     CONNECTED     23385    
unix  3      [ ]         STREAM     CONNECTED     15985    
unix  3      [ ]         STREAM     CONNECTED     22623    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     21004    /run/systemd/journal/stdout
unix  3      [ ]         DGRAM                    19235    
unix  3      [ ]         STREAM     CONNECTED     25970    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     22440    
unix  3      [ ]         STREAM     CONNECTED     2027     /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     25504    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22638    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     26895    
unix  3      [ ]         STREAM     CONNECTED     23000    
unix  2      [ ]         DGRAM                    19229    
unix  3      [ ]         DGRAM                    1383     
unix  3      [ ]         STREAM     CONNECTED     22636    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     26885    
unix  2      [ ]         DGRAM                    25741    
unix  3      [ ]         STREAM     CONNECTED     30940    
unix  3      [ ]         STREAM     CONNECTED     21881    
unix  2      [ ]         DGRAM                    14473    
unix  3      [ ]         STREAM     CONNECTED     23140    
unix  2      [ ]         DGRAM                    22610    
unix  3      [ ]         STREAM     CONNECTED     26884    
unix  3      [ ]         STREAM     CONNECTED     19899    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     21556    
unix  3      [ ]         SEQPACKET  CONNECTED     22647    
unix  3      [ ]         STREAM     CONNECTED     2016     
unix  3      [ ]         STREAM     CONNECTED     26842    
unix  3      [ ]         DGRAM                    19233    
unix  2      [ ]         DGRAM                    32294    
unix  3      [ ]         STREAM     CONNECTED     24838    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM                    16456    
unix  3      [ ]         STREAM     CONNECTED     19884    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     23141    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     19387    
unix  3      [ ]         STREAM     CONNECTED     26905    
unix  3      [ ]         STREAM     CONNECTED     22639    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     24054    /run/systemd/journal/stdout
unix  3      [ ]         DGRAM                    18098    
unix  2      [ ]         DGRAM                    1643     
unix  2      [ ]         DGRAM                    23363    
unix  3      [ ]         STREAM     CONNECTED     21555    
unix  3      [ ]         STREAM     CONNECTED     21381    
unix  3      [ ]         STREAM     CONNECTED     24821    
unix  3      [ ]         STREAM     CONNECTED     25085    
unix  3      [ ]         STREAM     CONNECTED     18548    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM                    23112    
unix  3      [ ]         STREAM     CONNECTED     30938    /run/containerd/containerd.sock
unix  3      [ ]         STREAM     CONNECTED     21647    
unix  3      [ ]         SEQPACKET  CONNECTED     22648    
unix  3      [ ]         STREAM     CONNECTED     23706    
unix  3      [ ]         STREAM     CONNECTED     30937    
unix  2      [ ]         DGRAM                    19392    
unix  3      [ ]         STREAM     CONNECTED     21309    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     31287    
unix  2      [ ]         DGRAM                    21558    
unix  3      [ ]         STREAM     CONNECTED     24041    
unix  3      [ ]         STREAM     CONNECTED     22637    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     22634    
unix  3      [ ]         STREAM     CONNECTED     23820    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22651    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22904    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     26875    
unix  3      [ ]         STREAM     CONNECTED     26938    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     21158    
unix  3      [ ]         STREAM     CONNECTED     23386    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     22747    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     21383    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     20853    
unix  3      [ ]         STREAM     CONNECTED     26456    
unix  3      [ ]         STREAM     CONNECTED     26876    
unix  3      [ ]         DGRAM                    1384     
unix  3      [ ]         STREAM     CONNECTED     22742    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22635    
unix  3      [ ]         STREAM     CONNECTED     16449    /run/systemd/journal/stdout
unix  3      [ ]         DGRAM                    19236    
unix  3      [ ]         STREAM     CONNECTED     25739    
unix  3      [ ]         STREAM     CONNECTED     20854    
unix  3      [ ]         STREAM     CONNECTED     22270    
unix  2      [ ]         DGRAM                    15079    
unix  3      [ ]         STREAM     CONNECTED     19227    
unix  3      [ ]         STREAM     CONNECTED     31288    /run/dbus/system_bus_socket
unix  2      [ ]         DGRAM                    30910    
unix  3      [ ]         STREAM     CONNECTED     23819    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22902    
unix  3      [ ]         STREAM     CONNECTED     17418    
unix  3      [ ]         DGRAM                    19234    
unix  3      [ ]         STREAM     CONNECTED     30941    /run/containerd/containerd.sock
unix  3      [ ]         STREAM     CONNECTED     26904    
unix  2      [ ]         DGRAM                    22633    
unix  3      [ ]         STREAM     CONNECTED     16767    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22268    
unix  3      [ ]         DGRAM                    15082    
unix  2      [ ]         DGRAM                    23139    
***************************************************************************************************************************************************************
###############################################################################################################################################################
## process Monitoring(ps,top,htop,atop,lsof)
- ps
    PID TTY          TIME CMD
   1510 ?        00:00:01 Runner.Listener
   1530 ?        00:00:02 Runner.Worker
   1640 ?        00:00:00 bash
   1665 ?        00:00:00 sh
   1688 ?        00:00:00 ps
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
