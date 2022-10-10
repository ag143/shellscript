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
Linux 5.15.0-1020-azure (fv-az177-244) 	10/10/22 	_x86_64_	(2 CPU)

avg-cpu:  %user   %nice %system %iowait  %steal   %idle
           3.08    0.04    3.40    0.67    0.00   92.80

Device             tps    kB_read/s    kB_wrtn/s    kB_dscd/s    kB_read    kB_wrtn    kB_dscd
loop0             1.17        10.01         0.00         0.00       2191          0          0
loop1             0.31         5.02         0.00         0.00       1100          0          0
loop2             4.85       183.44         0.00         0.00      40160          0          0
loop3             0.05         0.06         0.00         0.00         14          0          0
sda             211.28      3647.71       756.37    139182.83     798593     165593   30471297
sdb               3.86        59.42      1368.73    113260.99      13009     299656   24796228


***************************************************************************************************************************************************************
- sar
***************************************************************************************************************************************************************
- vmstat
procs -----------memory---------- ---swap-- -----io---- -system-- ------cpu-----
 r  b   swpd   free   buff  cache   si   so    bi    bo   in   cs us sy id wa st
 0  0      0 5247388 215228 1055360    0    0  1960  1066  105  583  3  3 93  1  0
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
/dev/root       87204404 54984352  32203668  64% /
devtmpfs         3550832        0   3550832   0% /dev
tmpfs            3555328        4   3555324   1% /dev/shm
tmpfs             711068     1096    709972   1% /run
tmpfs               5120        0      5120   0% /run/lock
tmpfs            3555328        0   3555328   0% /sys/fs/cgroup
/dev/loop0         64768    64768         0 100% /snap/core20/1623
/dev/loop1         69504    69504         0 100% /snap/lxd/22753
/dev/loop2         49152    49152         0 100% /snap/snapd/16778
/dev/sda15        106858     5321    101537   5% /boot/efi
/dev/sdb1       14341128  4194336   9396508  31% /mnt
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
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 57378
;; flags: qr rd ra; QUERY: 1, ANSWER: 13, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 65494
;; QUESTION SECTION:
;.				IN	NS

;; ANSWER SECTION:
.			515753	IN	NS	b.root-servers.net.
.			515753	IN	NS	j.root-servers.net.
.			515753	IN	NS	a.root-servers.net.
.			515753	IN	NS	c.root-servers.net.
.			515753	IN	NS	d.root-servers.net.
.			515753	IN	NS	f.root-servers.net.
.			515753	IN	NS	e.root-servers.net.
.			515753	IN	NS	i.root-servers.net.
.			515753	IN	NS	l.root-servers.net.
.			515753	IN	NS	g.root-servers.net.
.			515753	IN	NS	k.root-servers.net.
.			515753	IN	NS	m.root-servers.net.
.			515753	IN	NS	h.root-servers.net.

;; Query time: 4 msec
;; SERVER: 127.0.0.53#53(127.0.0.53)
;; WHEN: Mon Oct 10 07:53:12 UTC 2022
;; MSG SIZE  rcvd: 239

***************************************************************************************************************************************************************
- iptables
***************************************************************************************************************************************************************
- netstat
Active Internet connections (w/o servers)
Proto Recv-Q Send-Q Local Address           Foreign Address         State      
tcp        0      0 fv-az177-244.le1l:44414 lb-140-82-114-3-i:https TIME_WAIT  
tcp6       0      0 fv-az177-244.le1l:44814 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az177-244.le1l:44856 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az177-244.le1l:44834 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az177-244.le1l:33538 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az177-244.le1l:44866 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az177-244.le1l:36144 lb-140-82-113-10-:https TIME_WAIT  
tcp6       0      0 fv-az177-244.le1l:32962 lb-140-82-114-6-i:https TIME_WAIT  
tcp6       0      0 fv-az177-244.le1l:44826 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az177-244.le1l:33546 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az177-244.le1l:44848 13.107.42.16:https      ESTABLISHED
Active UNIX domain sockets (w/o servers)
Proto RefCnt Flags       Type       State         I-Node   Path
unix  2      [ ]         DGRAM                    27063    /run/user/1001/systemd/notify
unix  3      [ ]         DGRAM      CONNECTED     1419     /run/systemd/notify
unix  2      [ ]         DGRAM                    1436     /run/systemd/journal/syslog
unix  9      [ ]         DGRAM      CONNECTED     1446     /run/systemd/journal/dev-log
unix  9      [ ]         DGRAM      CONNECTED     1450     /run/systemd/journal/socket
unix  2      [ ]         DGRAM      CONNECTED     21920    /run/chrony/chronyd.sock
unix  2      [ ]         DGRAM                    31964    @00014
unix  3      [ ]         STREAM     CONNECTED     19677    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     27492    
unix  3      [ ]         STREAM     CONNECTED     17944    /run/systemd/journal/stdout
unix  3      [ ]         DGRAM      CONNECTED     27065    
unix  3      [ ]         STREAM     CONNECTED     21937    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     16535    
unix  3      [ ]         STREAM     CONNECTED     25930    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     27950    
unix  3      [ ]         STREAM     CONNECTED     27466    
unix  3      [ ]         DGRAM      CONNECTED     20651    
unix  3      [ ]         STREAM     CONNECTED     22041    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     24068    
unix  3      [ ]         STREAM     CONNECTED     21589    
unix  3      [ ]         STREAM     CONNECTED     27857    
unix  3      [ ]         STREAM     CONNECTED     20454    
unix  3      [ ]         STREAM     CONNECTED     19660    /run/systemd/journal/stdout
unix  3      [ ]         DGRAM      CONNECTED     1421     
unix  3      [ ]         STREAM     CONNECTED     23384    
unix  2      [ ]         DGRAM      CONNECTED     27034    
unix  3      [ ]         STREAM     CONNECTED     20145    
unix  3      [ ]         STREAM     CONNECTED     22039    
unix  2      [ ]         DGRAM      CONNECTED     16541    
unix  3      [ ]         STREAM     CONNECTED     27171    
unix  3      [ ]         DGRAM      CONNECTED     19072    
unix  3      [ ]         STREAM     CONNECTED     26624    
unix  3      [ ]         STREAM     CONNECTED     23465    
unix  2      [ ]         DGRAM      CONNECTED     21950    
unix  3      [ ]         STREAM     CONNECTED     15520    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM      CONNECTED     27025    
unix  2      [ ]         DGRAM      CONNECTED     1867     
unix  2      [ ]         DGRAM                    22376    
unix  3      [ ]         STREAM     CONNECTED     32022    /run/containerd/containerd.sock
unix  3      [ ]         STREAM     CONNECTED     22040    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     16547    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     23229    
unix  3      [ ]         STREAM     CONNECTED     22490    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     27491    
unix  3      [ ]         DGRAM      CONNECTED     20652    
unix  3      [ ]         STREAM     CONNECTED     27951    
unix  3      [ ]         STREAM     CONNECTED     21952    
unix  3      [ ]         STREAM     CONNECTED     27172    /run/dbus/system_bus_socket
unix  3      [ ]         DGRAM      CONNECTED     20653    
unix  2      [ ]         DGRAM      CONNECTED     14466    
unix  3      [ ]         STREAM     CONNECTED     32025    /run/containerd/containerd.sock
unix  3      [ ]         STREAM     CONNECTED     27067    
unix  3      [ ]         STREAM     CONNECTED     21953    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     17066    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM      CONNECTED     21835    
unix  2      [ ]         DGRAM      CONNECTED     24831    
unix  3      [ ]         STREAM     CONNECTED     22502    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     21825    
unix  3      [ ]         STREAM     CONNECTED     26735    
unix  3      [ ]         STREAM     CONNECTED     32021    
unix  2      [ ]         DGRAM      CONNECTED     20646    
unix  3      [ ]         STREAM     CONNECTED     21961    /run/dbus/system_bus_socket
unix  2      [ ]         DGRAM      CONNECTED     24914    
unix  2      [ ]         DGRAM      CONNECTED     20806    
unix  3      [ ]         STREAM     CONNECTED     22287    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     20644    
unix  3      [ ]         STREAM     CONNECTED     20292    
unix  3      [ ]         STREAM     CONNECTED     32543    
unix  3      [ ]         STREAM     CONNECTED     22363    
unix  3      [ ]         STREAM     CONNECTED     27465    
unix  2      [ ]         DGRAM      CONNECTED     21826    
unix  3      [ ]         STREAM     CONNECTED     15153    
unix  3      [ ]         STREAM     CONNECTED     25420    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     25825    
unix  3      [ ]         STREAM     CONNECTED     22583    
unix  3      [ ]         DGRAM      CONNECTED     20650    
unix  3      [ ]         DGRAM      CONNECTED     1420     
unix  3      [ ]         STREAM     CONNECTED     25921    /run/systemd/journal/stdout
unix  3      [ ]         SEQPACKET  CONNECTED     21922    
unix  3      [ ]         DGRAM      CONNECTED     15165    
unix  3      [ ]         STREAM     CONNECTED     27210    
unix  3      [ ]         STREAM     CONNECTED     19134    
unix  3      [ ]         STREAM     CONNECTED     26625    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     21960    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     22286    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     17065    
unix  3      [ ]         STREAM     CONNECTED     20442    
unix  2      [ ]         DGRAM      CONNECTED     22501    
unix  3      [ ]         STREAM     CONNECTED     20293    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     21936    
unix  3      [ ]         DGRAM      CONNECTED     15164    
unix  3      [ ]         STREAM     CONNECTED     22191    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     23962    
unix  3      [ ]         STREAM     CONNECTED     21962    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     21915    
unix  3      [ ]         STREAM     CONNECTED     27012    
unix  3      [ ]         STREAM     CONNECTED     23963    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     29662    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     27209    
unix  3      [ ]         STREAM     CONNECTED     20801    
unix  3      [ ]         STREAM     CONNECTED     27859    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22284    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     23730    
unix  3      [ ]         STREAM     CONNECTED     27068    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     25060    /run/dbus/system_bus_socket
unix  3      [ ]         SEQPACKET  CONNECTED     21921    
unix  2      [ ]         DGRAM      CONNECTED     15162    
unix  2      [ ]         DGRAM      CONNECTED     31969    
unix  3      [ ]         DGRAM      CONNECTED     19071    
unix  3      [ ]         STREAM     CONNECTED     22364    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM                    33798    
unix  3      [ ]         STREAM     CONNECTED     25919    
unix  3      [ ]         STREAM     CONNECTED     20453    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     23620    
unix  3      [ ]         STREAM     CONNECTED     23072    
unix  3      [ ]         STREAM     CONNECTED     21951    
unix  3      [ ]         STREAM     CONNECTED     32024    
unix  3      [ ]         DGRAM      CONNECTED     27064    
unix  3      [ ]         STREAM     CONNECTED     21934    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22585    /run/systemd/journal/stdout
***************************************************************************************************************************************************************
###############################################################################################################################################################
## process Monitoring(ps,top,htop,atop,lsof)
- ps
    PID TTY          TIME CMD
    871 ?        00:00:00 systemd
    873 ?        00:00:00 (sd-pam)
   1527 ?        00:00:01 Runner.Listener
   1545 ?        00:00:02 Runner.Worker
   1648 ?        00:00:00 bash
   1674 ?        00:00:00 sh
   1698 ?        00:00:00 ps
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
