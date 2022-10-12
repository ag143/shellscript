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
Linux 5.15.0-1020-azure (fv-az259-73) 	10/12/22 	_x86_64_	(2 CPU)

avg-cpu:  %user   %nice %system %iowait  %steal   %idle
           6.29    0.09    7.26    1.15    0.00   85.21

Device             tps    kB_read/s    kB_wrtn/s    kB_dscd/s    kB_read    kB_wrtn    kB_dscd
loop0             1.97        17.13         0.00         0.00       2246          0          0
loop1             0.52         8.39         0.00         0.00       1100          0          0
loop2             6.70       253.05         0.00         0.00      33172          0          0
loop3             0.10         0.17         0.00         0.00         22          0          0
sda               6.23        91.30      2285.88    189154.23      11969     299656   24796228
sdb             361.31      6095.00      1274.40    232125.05     798993     167061   30429273


***************************************************************************************************************************************************************
- sar
***************************************************************************************************************************************************************
- vmstat
procs -----------memory---------- ---swap-- -----io---- -system-- ------cpu-----
 r  b   swpd   free   buff  cache   si   so    bi    bo   in   cs us sy id wa st
 0  0      0 5274636 215280 1055400    0    0  3275  1803  159  946  6  7 85  1  0
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
/dev/root       87204404 54984400  32203620  64% /
devtmpfs         3550832        0   3550832   0% /dev
tmpfs            3555328        4   3555324   1% /dev/shm
tmpfs             711068     1096    709972   1% /run
tmpfs               5120        0      5120   0% /run/lock
tmpfs            3555328        0   3555328   0% /sys/fs/cgroup
/dev/loop0         64768    64768         0 100% /snap/core20/1623
/dev/loop2         49152    49152         0 100% /snap/snapd/16778
/dev/loop1         69504    69504         0 100% /snap/lxd/22753
/dev/sdb15        106858     5321    101537   5% /boot/efi
/dev/sda1       14341128  4194336   9396508  31% /mnt
tmpfs             711064        0    711064   0% /run/user/1001
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
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 147
;; flags: qr rd ra; QUERY: 1, ANSWER: 13, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 65494
;; QUESTION SECTION:
;.				IN	NS

;; ANSWER SECTION:
.			517278	IN	NS	d.root-servers.net.
.			517278	IN	NS	e.root-servers.net.
.			517278	IN	NS	m.root-servers.net.
.			517278	IN	NS	i.root-servers.net.
.			517278	IN	NS	b.root-servers.net.
.			517278	IN	NS	f.root-servers.net.
.			517278	IN	NS	h.root-servers.net.
.			517278	IN	NS	k.root-servers.net.
.			517278	IN	NS	c.root-servers.net.
.			517278	IN	NS	a.root-servers.net.
.			517278	IN	NS	j.root-servers.net.
.			517278	IN	NS	g.root-servers.net.
.			517278	IN	NS	l.root-servers.net.

;; Query time: 4 msec
;; SERVER: 127.0.0.53#53(127.0.0.53)
;; WHEN: Wed Oct 12 05:27:15 UTC 2022
;; MSG SIZE  rcvd: 239

***************************************************************************************************************************************************************
- iptables
***************************************************************************************************************************************************************
- netstat
Active Internet connections (w/o servers)
Proto Recv-Q Send-Q Local Address           Foreign Address         State      
tcp6       0      0 fv-az259-73.nxnqh:59688 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az259-73.nxnqh:52902 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az259-73.nxnqh:59748 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az259-73.nxnqh:59732 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az259-73.nxnqh:59716 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az259-73.nxnqh:59690 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az259-73.nxnqh:34948 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az259-73.nxnqh:59738 13.107.42.16:https      ESTABLISHED
Active UNIX domain sockets (w/o servers)
Proto RefCnt Flags       Type       State         I-Node   Path
unix  2      [ ]         DGRAM                    27304    /run/user/1001/systemd/notify
unix  3      [ ]         DGRAM      CONNECTED     13719    /run/systemd/notify
unix  2      [ ]         DGRAM                    13736    /run/systemd/journal/syslog
unix  9      [ ]         DGRAM      CONNECTED     13746    /run/systemd/journal/dev-log
unix  9      [ ]         DGRAM      CONNECTED     13750    /run/systemd/journal/socket
unix  2      [ ]         DGRAM      CONNECTED     22676    /run/chrony/chronyd.sock
unix  2      [ ]         DGRAM                    31242    @00014
unix  3      [ ]         STREAM     CONNECTED     27309    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     23642    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     21258    
unix  3      [ ]         DGRAM      CONNECTED     18278    
unix  3      [ ]         STREAM     CONNECTED     32032    
unix  3      [ ]         STREAM     CONNECTED     22157    
unix  3      [ ]         STREAM     CONNECTED     27308    
unix  3      [ ]         STREAM     CONNECTED     21416    
unix  3      [ ]         STREAM     CONNECTED     21716    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22847    
unix  3      [ ]         STREAM     CONNECTED     25060    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     27729    
unix  2      [ ]         DGRAM      CONNECTED     14723    
unix  3      [ ]         STREAM     CONNECTED     19986    
unix  2      [ ]         DGRAM                    22434    
unix  2      [ ]         DGRAM      CONNECTED     25980    
unix  2      [ ]         DGRAM      CONNECTED     24965    
unix  3      [ ]         STREAM     CONNECTED     24482    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     21417    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     18767    
unix  3      [ ]         STREAM     CONNECTED     22688    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     21800    /run/systemd/journal/stdout
unix  3      [ ]         DGRAM      CONNECTED     13720    
unix  3      [ ]         DGRAM      CONNECTED     19995    
unix  3      [ ]         STREAM     CONNECTED     22243    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     23084    
unix  2      [ ]         DGRAM      CONNECTED     22593    
unix  3      [ ]         STREAM     CONNECTED     23888    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     23085    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22433    
unix  3      [ ]         STREAM     CONNECTED     17517    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM      CONNECTED     14356    
unix  3      [ ]         STREAM     CONNECTED     23316    
unix  3      [ ]         DGRAM      CONNECTED     15289    
unix  3      [ ]         STREAM     CONNECTED     26444    
unix  3      [ ]         STREAM     CONNECTED     24234    
unix  3      [ ]         STREAM     CONNECTED     27171    
unix  3      [ ]         STREAM     CONNECTED     22246    /run/dbus/system_bus_socket
unix  2      [ ]         DGRAM      CONNECTED     21717    
unix  3      [ ]         STREAM     CONNECTED     23643    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     17516    
unix  3      [ ]         STREAM     CONNECTED     22242    
unix  3      [ ]         STREAM     CONNECTED     21257    
unix  3      [ ]         STREAM     CONNECTED     23886    
unix  3      [ ]         STREAM     CONNECTED     22685    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM      CONNECTED     17626    
unix  3      [ ]         STREAM     CONNECTED     22437    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     17939    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM                    33633    
unix  2      [ ]         DGRAM      CONNECTED     26105    
unix  3      [ ]         STREAM     CONNECTED     27438    
unix  3      [ ]         STREAM     CONNECTED     23319    /run/systemd/journal/stdout
unix  3      [ ]         DGRAM      CONNECTED     27306    
unix  2      [ ]         DGRAM      CONNECTED     22240    
unix  3      [ ]         SEQPACKET  CONNECTED     22677    
unix  2      [ ]         DGRAM      CONNECTED     19410    
unix  3      [ ]         STREAM     CONNECTED     25945    
unix  3      [ ]         STREAM     CONNECTED     31274    /run/containerd/containerd.sock
unix  3      [ ]         STREAM     CONNECTED     21715    
unix  3      [ ]         STREAM     CONNECTED     23009    
unix  3      [ ]         STREAM     CONNECTED     19262    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     20460    
unix  3      [ ]         STREAM     CONNECTED     26590    
unix  3      [ ]         STREAM     CONNECTED     19405    
unix  3      [ ]         DGRAM      CONNECTED     19993    
unix  3      [ ]         DGRAM      CONNECTED     13721    
unix  3      [ ]         STREAM     CONNECTED     31273    
unix  3      [ ]         STREAM     CONNECTED     15278    
unix  2      [ ]         DGRAM      CONNECTED     25318    
unix  3      [ ]         STREAM     CONNECTED     27006    /run/systemd/journal/stdout
unix  3      [ ]         DGRAM      CONNECTED     27305    
unix  3      [ ]         STREAM     CONNECTED     22241    
unix  3      [ ]         SEQPACKET  CONNECTED     22678    
unix  3      [ ]         DGRAM      CONNECTED     19992    
unix  3      [ ]         STREAM     CONNECTED     15295    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22248    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     31270    
unix  3      [ ]         STREAM     CONNECTED     25733    
unix  3      [ ]         STREAM     CONNECTED     27501    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22234    
unix  3      [ ]         STREAM     CONNECTED     22245    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     27730    
unix  3      [ ]         STREAM     CONNECTED     27437    
unix  3      [ ]         STREAM     CONNECTED     23550    
unix  3      [ ]         STREAM     CONNECTED     22845    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22585    
unix  3      [ ]         STREAM     CONNECTED     26437    
unix  3      [ ]         STREAM     CONNECTED     22848    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     23641    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM      CONNECTED     24609    
unix  3      [ ]         STREAM     CONNECTED     16596    
unix  3      [ ]         DGRAM      CONNECTED     15290    
unix  3      [ ]         DGRAM      CONNECTED     18277    
unix  3      [ ]         STREAM     CONNECTED     26936    
unix  3      [ ]         STREAM     CONNECTED     26591    
unix  3      [ ]         STREAM     CONNECTED     20015    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM      CONNECTED     31243    
unix  3      [ ]         DGRAM      CONNECTED     19994    
unix  3      [ ]         STREAM     CONNECTED     22436    
unix  2      [ ]         DGRAM      CONNECTED     15287    
unix  3      [ ]         STREAM     CONNECTED     22680    
unix  3      [ ]         STREAM     CONNECTED     24361    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     26117    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     33172    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     23636    
unix  2      [ ]         DGRAM      CONNECTED     19988    
unix  3      [ ]         STREAM     CONNECTED     22244    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     24479    
unix  3      [ ]         STREAM     CONNECTED     26443    
unix  3      [ ]         STREAM     CONNECTED     18773    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     31271    /run/containerd/containerd.sock
unix  3      [ ]         STREAM     CONNECTED     22587    
unix  3      [ ]         STREAM     CONNECTED     25830    /run/dbus/system_bus_socket
***************************************************************************************************************************************************************
###############################################################################################################################################################
## process Monitoring(ps,top,htop,atop,lsof)
- ps
    PID TTY          TIME CMD
    831 ?        00:00:00 systemd
    851 ?        00:00:00 (sd-pam)
   1511 ?        00:00:01 Runner.Listener
   1527 ?        00:00:02 Runner.Worker
   1634 ?        00:00:00 bash
   1660 ?        00:00:00 sh
   1683 ?        00:00:00 ps
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
