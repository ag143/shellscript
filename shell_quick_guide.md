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
Linux 5.15.0-1020-azure (fv-az264-177) 	10/12/22 	_x86_64_	(2 CPU)

avg-cpu:  %user   %nice %system %iowait  %steal   %idle
           8.05    0.15    8.66    1.29    0.00   81.85

Device             tps    kB_read/s    kB_wrtn/s    kB_dscd/s    kB_read    kB_wrtn    kB_dscd
loop0             2.09        18.09         0.00         0.00       2256          0          0
loop1             7.99       313.28         0.00         0.00      39063          0          0
loop2             0.55         8.82         0.00         0.00       1100          0          0
loop3             0.09         0.11         0.00         0.00         14          0          0
sda               6.56        95.99      2403.24    198863.00      11969     299660   24796228
sdb             373.20      6409.51      1343.66    244283.66     799201     167541   30459729


***************************************************************************************************************************************************************
- sar
***************************************************************************************************************************************************************
- vmstat
procs -----------memory---------- ---swap-- -----io---- -system-- ------cpu-----
 r  b   swpd   free   buff  cache   si   so    bi    bo   in   cs us sy id wa st
 1  0      0 5261708 214832 1055932    0    0  3470  1898  171  996  8  9 82  1  0
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
/dev/loop1         49152    49152         0 100% /snap/snapd/16778
/dev/loop2         69504    69504         0 100% /snap/lxd/22753
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
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 4612
;; flags: qr rd ra; QUERY: 1, ANSWER: 13, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 65494
;; QUESTION SECTION:
;.				IN	NS

;; ANSWER SECTION:
.			517968	IN	NS	c.root-servers.net.
.			517968	IN	NS	d.root-servers.net.
.			517968	IN	NS	i.root-servers.net.
.			517968	IN	NS	j.root-servers.net.
.			517968	IN	NS	l.root-servers.net.
.			517968	IN	NS	k.root-servers.net.
.			517968	IN	NS	f.root-servers.net.
.			517968	IN	NS	b.root-servers.net.
.			517968	IN	NS	m.root-servers.net.
.			517968	IN	NS	a.root-servers.net.
.			517968	IN	NS	e.root-servers.net.
.			517968	IN	NS	g.root-servers.net.
.			517968	IN	NS	h.root-servers.net.

;; Query time: 0 msec
;; SERVER: 127.0.0.53#53(127.0.0.53)
;; WHEN: Wed Oct 12 05:24:15 UTC 2022
;; MSG SIZE  rcvd: 239

***************************************************************************************************************************************************************
- iptables
***************************************************************************************************************************************************************
- netstat
Active Internet connections (w/o servers)
Proto Recv-Q Send-Q Local Address           Foreign Address         State      
tcp6       0      0 fv-az264-177.ca02:37712 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az264-177.ca02:37692 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az264-177.ca02:37696 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az264-177.ca02:37698 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az264-177.ca02:51202 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az264-177.ca02:40516 13.107.43.16:https      ESTABLISHED
tcp6       0      0 fv-az264-177.ca02:42380 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az264-177.ca02:37686 13.107.42.16:https      ESTABLISHED
Active UNIX domain sockets (w/o servers)
Proto RefCnt Flags       Type       State         I-Node   Path
unix  2      [ ]         DGRAM                    25545    /run/user/1001/systemd/notify
unix  3      [ ]         DGRAM      CONNECTED     1222     /run/systemd/notify
unix  2      [ ]         DGRAM                    1239     /run/systemd/journal/syslog
unix  9      [ ]         DGRAM      CONNECTED     1249     /run/systemd/journal/dev-log
unix  9      [ ]         DGRAM      CONNECTED     1253     /run/systemd/journal/socket
unix  2      [ ]         DGRAM      CONNECTED     22898    /run/chrony/chronyd.sock
unix  2      [ ]         DGRAM                    28899    @00014
unix  3      [ ]         STREAM     CONNECTED     27415    
unix  3      [ ]         STREAM     CONNECTED     23536    
unix  3      [ ]         STREAM     CONNECTED     15024    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     25549    
unix  3      [ ]         STREAM     CONNECTED     23381    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22762    /run/systemd/journal/stdout
unix  3      [ ]         SEQPACKET  CONNECTED     22900    
unix  3      [ ]         DGRAM      CONNECTED     19221    
unix  3      [ ]         STREAM     CONNECTED     27738    
unix  3      [ ]         STREAM     CONNECTED     22845    
unix  3      [ ]         DGRAM      CONNECTED     25546    
unix  3      [ ]         STREAM     CONNECTED     31784    
unix  3      [ ]         DGRAM      CONNECTED     15714    
unix  3      [ ]         STREAM     CONNECTED     25742    
unix  2      [ ]         DGRAM      CONNECTED     22864    
unix  2      [ ]         DGRAM      CONNECTED     19217    
unix  3      [ ]         DGRAM      CONNECTED     25547    
unix  3      [ ]         STREAM     CONNECTED     16132    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22884    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     23284    
unix  2      [ ]         DGRAM      CONNECTED     1846     
unix  3      [ ]         STREAM     CONNECTED     24904    
unix  3      [ ]         STREAM     CONNECTED     20054    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     27897    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     23559    
unix  2      [ ]         DGRAM      CONNECTED     25519    
unix  3      [ ]         DGRAM      CONNECTED     19461    
unix  3      [ ]         DGRAM      CONNECTED     15713    
unix  3      [ ]         STREAM     CONNECTED     21194    
unix  3      [ ]         STREAM     CONNECTED     25506    
unix  2      [ ]         DGRAM      CONNECTED     24043    
unix  3      [ ]         STREAM     CONNECTED     15011    
unix  2      [ ]         DGRAM                    29455    
unix  3      [ ]         STREAM     CONNECTED     19374    
unix  3      [ ]         STREAM     CONNECTED     27761    
unix  3      [ ]         SEQPACKET  CONNECTED     22899    
unix  2      [ ]         DGRAM      CONNECTED     15711    
unix  3      [ ]         STREAM     CONNECTED     16131    
unix  3      [ ]         STREAM     CONNECTED     32764    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     26681    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     25644    
unix  3      [ ]         STREAM     CONNECTED     22881    
unix  2      [ ]         DGRAM      CONNECTED     24891    
unix  3      [ ]         STREAM     CONNECTED     18631    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     21502    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     23377    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     17689    
unix  3      [ ]         STREAM     CONNECTED     28940    /run/containerd/containerd.sock
unix  3      [ ]         STREAM     CONNECTED     22980    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     18625    
unix  3      [ ]         STREAM     CONNECTED     22882    
unix  3      [ ]         STREAM     CONNECTED     23133    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22883    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     21636    
unix  3      [ ]         STREAM     CONNECTED     28937    /run/containerd/containerd.sock
unix  2      [ ]         DGRAM      CONNECTED     21639    
unix  3      [ ]         STREAM     CONNECTED     21428    
unix  3      [ ]         STREAM     CONNECTED     21181    
unix  3      [ ]         STREAM     CONNECTED     27414    
unix  3      [ ]         STREAM     CONNECTED     23547    /run/dbus/system_bus_socket
unix  2      [ ]         DGRAM      CONNECTED     25526    
unix  3      [ ]         STREAM     CONNECTED     23934    /run/systemd/journal/stdout
unix  3      [ ]         DGRAM      CONNECTED     1223     
unix  3      [ ]         DGRAM      CONNECTED     19462    
unix  3      [ ]         STREAM     CONNECTED     23057    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM      CONNECTED     19379    
unix  3      [ ]         STREAM     CONNECTED     27248    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     23537    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22750    
unix  3      [ ]         STREAM     CONNECTED     23927    
unix  3      [ ]         STREAM     CONNECTED     21637    
unix  3      [ ]         STREAM     CONNECTED     23285    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     27752    
unix  3      [ ]         STREAM     CONNECTED     23459    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     19215    
unix  3      [ ]         STREAM     CONNECTED     25550    /run/dbus/system_bus_socket
unix  2      [ ]         DGRAM      CONNECTED     16241    
unix  3      [ ]         STREAM     CONNECTED     25750    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22073    
unix  3      [ ]         STREAM     CONNECTED     25894    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     27737    
unix  3      [ ]         STREAM     CONNECTED     22850    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     27387    
unix  2      [ ]         DGRAM      CONNECTED     25076    
unix  2      [ ]         DGRAM      CONNECTED     22880    
unix  2      [ ]         DGRAM                    23545    
unix  3      [ ]         DGRAM      CONNECTED     19223    
unix  3      [ ]         STREAM     CONNECTED     23290    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     23056    
unix  2      [ ]         DGRAM      CONNECTED     1372     
unix  3      [ ]         STREAM     CONNECTED     22886    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     26771    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM      CONNECTED     28900    
unix  3      [ ]         DGRAM      CONNECTED     1224     
unix  3      [ ]         DGRAM      CONNECTED     19222    
unix  3      [ ]         STREAM     CONNECTED     27762    
unix  3      [ ]         STREAM     CONNECTED     22885    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     23132    
unix  3      [ ]         STREAM     CONNECTED     20070    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     17690    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     28939    
unix  3      [ ]         STREAM     CONNECTED     21968    
unix  3      [ ]         STREAM     CONNECTED     27753    
unix  3      [ ]         STREAM     CONNECTED     22761    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     23375    
unix  3      [ ]         STREAM     CONNECTED     21350    
unix  3      [ ]         STREAM     CONNECTED     27247    
unix  3      [ ]         STREAM     CONNECTED     29430    
unix  3      [ ]         STREAM     CONNECTED     25084    
unix  3      [ ]         STREAM     CONNECTED     25743    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     23546    
unix  3      [ ]         DGRAM      CONNECTED     19224    
unix  3      [ ]         STREAM     CONNECTED     23458    
***************************************************************************************************************************************************************
###############################################################################################################################################################
## process Monitoring(ps,top,htop,atop,lsof)
- ps
    PID TTY          TIME CMD
    870 ?        00:00:00 systemd
    873 ?        00:00:00 (sd-pam)
   1503 ?        00:00:02 Runner.Listener
   1519 ?        00:00:03 Runner.Worker
   1627 ?        00:00:00 bash
   1652 ?        00:00:00 sh
   1674 ?        00:00:00 ps
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
