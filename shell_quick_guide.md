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
Linux 5.13.0-1022-azure (fv-az246-872) 	05/08/22 	_x86_64_	(2 CPU)

avg-cpu:  %user   %nice %system %iowait  %steal   %idle
          24.27    0.50   22.90    2.83    0.00   49.50

Device             tps    kB_read/s    kB_wrtn/s    kB_dscd/s    kB_read    kB_wrtn    kB_dscd
loop0             7.34        66.60         0.00         0.00       2305          0          0
loop1             1.96        31.78         0.00         0.00       1100          0          0
loop2            24.04       941.12         0.00         0.00      32572          0          0
loop3             0.32         0.40         0.00         0.00         14          0          0
sda            1225.40     22868.84      3102.93       217.97     791490     107392       7544
sdb              29.53       345.82      8656.46    424097.54      11969     299600   14678016


***************************************************************************************************************************************************************
- sar
***************************************************************************************************************************************************************
- vmstat
procs -----------memory---------- ---swap-- -----io---- -system-- ------cpu-----
 r  b   swpd   free   buff  cache   si   so    bi    bo   in   cs us sy id wa st
 1  0      0 5369224 207768 1025132    0    0 12620  6116  612 3172 25 23 49  3  0
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
/dev/root       87218124 55263024  31938716  64% /
devtmpfs         3552988        0   3552988   0% /dev
tmpfs            3556560        4   3556556   1% /dev/shm
tmpfs             711316     1080    710236   1% /run
tmpfs               5120        0      5120   0% /run/lock
tmpfs            3556560        0   3556560   0% /sys/fs/cgroup
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
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 4696
;; flags: qr rd ra; QUERY: 1, ANSWER: 13, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 65494
;; QUESTION SECTION:
;.				IN	NS

;; ANSWER SECTION:
.			4670	IN	NS	a.root-servers.net.
.			4670	IN	NS	e.root-servers.net.
.			4670	IN	NS	h.root-servers.net.
.			4670	IN	NS	k.root-servers.net.
.			4670	IN	NS	i.root-servers.net.
.			4670	IN	NS	c.root-servers.net.
.			4670	IN	NS	m.root-servers.net.
.			4670	IN	NS	f.root-servers.net.
.			4670	IN	NS	l.root-servers.net.
.			4670	IN	NS	j.root-servers.net.
.			4670	IN	NS	d.root-servers.net.
.			4670	IN	NS	b.root-servers.net.
.			4670	IN	NS	g.root-servers.net.

;; Query time: 4 msec
;; SERVER: 127.0.0.53#53(127.0.0.53)
;; WHEN: Sun May 08 09:58:00 UTC 2022
;; MSG SIZE  rcvd: 239

***************************************************************************************************************************************************************
- iptables
***************************************************************************************************************************************************************
- netstat
Active Internet connections (w/o servers)
Proto Recv-Q Send-Q Local Address           Foreign Address         State      
tcp        0      0 fv-az246-872.py5d:46208 168.63.129.16:http      TIME_WAIT  
tcp        0      0 fv-az246-872.py5d:38276 169.254.169.254:http    TIME_WAIT  
tcp        0      0 fv-az246-872.py5d:46210 168.63.129.16:http      TIME_WAIT  
tcp        0      0 fv-az246-872.py5d:50136 lb-140-82-114-4-i:https TIME_WAIT  
tcp6       0      0 fv-az246-872.py5d:49668 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az246-872.py5d:49680 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az246-872.py5d:49682 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az246-872.py5d:60116 lb-140-82-114-9-i:https TIME_WAIT  
tcp6       0      0 fv-az246-872.py5d:49674 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az246-872.py5d:49666 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az246-872.py5d:49672 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az246-872.py5d:49678 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az246-872.py5d:49670 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az246-872.py5d:57708 lb-140-82-112-6-i:https TIME_WAIT  
Active UNIX domain sockets (w/o servers)
Proto RefCnt Flags       Type       State         I-Node   Path
unix  3      [ ]         DGRAM                    14053    /run/systemd/notify
unix  2      [ ]         DGRAM                    14070    /run/systemd/journal/syslog
unix  8      [ ]         DGRAM                    14080    /run/systemd/journal/dev-log
unix  9      [ ]         DGRAM                    14084    /run/systemd/journal/socket
unix  2      [ ]         DGRAM                    21223    /run/chrony/chronyd.sock
unix  2      [ ]         DGRAM                    27293    @00014
unix  3      [ ]         STREAM     CONNECTED     27340    /run/containerd/containerd.sock
unix  3      [ ]         STREAM     CONNECTED     21304    
unix  3      [ ]         STREAM     CONNECTED     21207    
unix  3      [ ]         STREAM     CONNECTED     18024    /run/systemd/journal/stdout
unix  3      [ ]         DGRAM                    14054    
unix  3      [ ]         STREAM     CONNECTED     26276    
unix  3      [ ]         DGRAM                    19716    
unix  3      [ ]         STREAM     CONNECTED     23510    
unix  3      [ ]         STREAM     CONNECTED     25148    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     25053    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     25146    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     14886    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     19406    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     25102    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     23336    
unix  3      [ ]         STREAM     CONNECTED     25296    
unix  2      [ ]         DGRAM                    15535    
unix  2      [ ]         DGRAM                    27302    
unix  2      [ ]         DGRAM                    23204    
unix  2      [ ]         DGRAM                    22045    
unix  3      [ ]         STREAM     CONNECTED     21208    
unix  3      [ ]         STREAM     CONNECTED     14877    
unix  3      [ ]         STREAM     CONNECTED     25077    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     23030    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     25149    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     31132    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     31124    /run/dbus/system_bus_socket
unix  2      [ ]         DGRAM                    23328    
unix  3      [ ]         STREAM     CONNECTED     27337    
unix  3      [ ]         DGRAM                    19717    
unix  3      [ ]         STREAM     CONNECTED     20475    
unix  3      [ ]         STREAM     CONNECTED     25276    
unix  2      [ ]         DGRAM                    14362    
unix  3      [ ]         SEQPACKET  CONNECTED     21225    
unix  3      [ ]         STREAM     CONNECTED     23857    
unix  3      [ ]         STREAM     CONNECTED     25585    
unix  3      [ ]         STREAM     CONNECTED     18610    
unix  3      [ ]         STREAM     CONNECTED     25201    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     23120    
unix  3      [ ]         STREAM     CONNECTED     22040    
unix  3      [ ]         STREAM     CONNECTED     25949    
unix  3      [ ]         STREAM     CONNECTED     22934    
unix  2      [ ]         DGRAM                    15939    
unix  3      [ ]         STREAM     CONNECTED     19421    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     25318    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22450    
unix  3      [ ]         DGRAM                    19719    
unix  3      [ ]         STREAM     CONNECTED     25297    
unix  3      [ ]         STREAM     CONNECTED     31813    
unix  3      [ ]         STREAM     CONNECTED     23028    
unix  3      [ ]         STREAM     CONNECTED     23031    /run/dbus/system_bus_socket
unix  2      [ ]         DGRAM                    23509    
unix  3      [ ]         STREAM     CONNECTED     22456    
unix  3      [ ]         STREAM     CONNECTED     16568    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     19710    
unix  3      [ ]         DGRAM                    15537    
unix  3      [ ]         STREAM     CONNECTED     25948    
unix  2      [ ]         DGRAM                    23026    
unix  3      [ ]         STREAM     CONNECTED     31801    
unix  2      [ ]         DGRAM                    21218    
unix  3      [ ]         STREAM     CONNECTED     17001    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     25137    /run/systemd/journal/stdout
unix  3      [ ]         DGRAM                    15538    
unix  3      [ ]         STREAM     CONNECTED     24227    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     22123    
unix  3      [ ]         STREAM     CONNECTED     23701    
unix  3      [ ]         DGRAM                    14055    
unix  3      [ ]         STREAM     CONNECTED     27338    /run/containerd/containerd.sock
unix  2      [ ]         DGRAM                    19712    
unix  3      [ ]         STREAM     CONNECTED     24491    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     23032    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     24759    /run/dbus/system_bus_socket
unix  2      [ ]         DGRAM                    848      
unix  2      [ ]         DGRAM                    31302    
unix  3      [ ]         DGRAM                    18020    
unix  3      [ ]         STREAM     CONNECTED     23211    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     25054    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     30587    
unix  3      [ ]         DGRAM                    19718    
unix  3      [ ]         STREAM     CONNECTED     25078    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     20476    
unix  3      [ ]         STREAM     CONNECTED     25161    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     23033    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     23027    
unix  3      [ ]         STREAM     CONNECTED     21967    
unix  3      [ ]         STREAM     CONNECTED     16161    
unix  3      [ ]         STREAM     CONNECTED     19869    
unix  3      [ ]         STREAM     CONNECTED     23029    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     25275    
unix  3      [ ]         STREAM     CONNECTED     21464    
unix  2      [ ]         DGRAM                    31811    
unix  2      [ ]         DGRAM                    23894    
unix  3      [ ]         STREAM     CONNECTED     22775    
unix  3      [ ]         STREAM     CONNECTED     15934    
unix  3      [ ]         STREAM     CONNECTED     26422    
unix  3      [ ]         DGRAM                    18019    
unix  3      [ ]         STREAM     CONNECTED     31127    /run/systemd/journal/stdout
unix  3      [ ]         SEQPACKET  CONNECTED     21224    
unix  3      [ ]         STREAM     CONNECTED     23210    
unix  3      [ ]         STREAM     CONNECTED     22121    
unix  3      [ ]         STREAM     CONNECTED     26423    
unix  2      [ ]         DGRAM                    19874    
unix  3      [ ]         STREAM     CONNECTED     24758    
unix  3      [ ]         STREAM     CONNECTED     25195    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     24224    
unix  3      [ ]         STREAM     CONNECTED     25062    /run/systemd/journal/stdout
***************************************************************************************************************************************************************
###############################################################################################################################################################
## process Monitoring(ps,top,htop,atop,lsof)
- ps
    PID TTY          TIME CMD
   1450 ?        00:00:02 Runner.Listener
   1471 ?        00:00:02 Runner.Worker
   1574 ?        00:00:00 bash
   1601 ?        00:00:00 sh
   1623 ?        00:00:00 ps
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
