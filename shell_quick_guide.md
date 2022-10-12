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
Linux 5.15.0-1020-azure (fv-az74-467) 	10/12/22 	_x86_64_	(2 CPU)

avg-cpu:  %user   %nice %system %iowait  %steal   %idle
          19.98    0.36   23.82    5.01    0.00   50.83

Device             tps    kB_read/s    kB_wrtn/s    kB_dscd/s    kB_read    kB_wrtn    kB_dscd
loop0             6.22        54.07         0.00         0.00       2250          0          0
loop1             1.63        26.44         0.00         0.00       1100          0          0
loop2            24.49       939.82         0.00         0.00      39106          0          0
loop3             0.29         0.43         0.00         0.00         18          0          0
sda            1104.11     19203.50      2825.20    732512.30     799057     117556   30479837
sdb              20.02       312.64      7197.02    595919.92      13009     299468   24796228


***************************************************************************************************************************************************************
- sar
***************************************************************************************************************************************************************
- vmstat
procs -----------memory---------- ---swap-- -----io---- -system-- ------cpu-----
 r  b   swpd   free   buff  cache   si   so    bi    bo   in   cs us sy id wa st
 1  0      0 5282264 214956 1057296    0    0 10571  5156  467 2818 20 24 51  5  0
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
/dev/root       87204404 54984484  32203536  64% /
devtmpfs         3550832        0   3550832   0% /dev
tmpfs            3555328        4   3555324   1% /dev/shm
tmpfs             711068     1100    709968   1% /run
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
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 10970
;; flags: qr rd ra; QUERY: 1, ANSWER: 13, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 65494
;; QUESTION SECTION:
;.				IN	NS

;; ANSWER SECTION:
.			515834	IN	NS	a.root-servers.net.
.			515834	IN	NS	m.root-servers.net.
.			515834	IN	NS	i.root-servers.net.
.			515834	IN	NS	h.root-servers.net.
.			515834	IN	NS	d.root-servers.net.
.			515834	IN	NS	l.root-servers.net.
.			515834	IN	NS	c.root-servers.net.
.			515834	IN	NS	b.root-servers.net.
.			515834	IN	NS	f.root-servers.net.
.			515834	IN	NS	k.root-servers.net.
.			515834	IN	NS	e.root-servers.net.
.			515834	IN	NS	j.root-servers.net.
.			515834	IN	NS	g.root-servers.net.

;; Query time: 4 msec
;; SERVER: 127.0.0.53#53(127.0.0.53)
;; WHEN: Wed Oct 12 05:24:57 UTC 2022
;; MSG SIZE  rcvd: 239

***************************************************************************************************************************************************************
- iptables
***************************************************************************************************************************************************************
- netstat
Active Internet connections (w/o servers)
Proto Recv-Q Send-Q Local Address           Foreign Address         State      
tcp        0      0 fv-az74-467.rg1nh:50476 168.63.129.16:http      TIME_WAIT  
tcp        0      0 fv-az74-467.rg1nh:50490 168.63.129.16:http      TIME_WAIT  
tcp        0      0 fv-az74-467.rg1nh:59380 lb-140-82-113-3-i:https TIME_WAIT  
tcp        0      0 fv-az74-467.rg1nh:59252 169.254.169.254:http    TIME_WAIT  
tcp6       0      0 fv-az74-467.rg1nh:40086 lb-140-82-112-6-i:https TIME_WAIT  
tcp6       0      0 fv-az74-467.rg1nh:36196 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az74-467.rg1nh:42984 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az74-467.rg1nh:43016 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az74-467.rg1nh:35796 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az74-467.rg1nh:43004 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az74-467.rg1nh:46094 lb-140-82-114-10-:https TIME_WAIT  
tcp6       0      0 fv-az74-467.rg1nh:55880 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az74-467.rg1nh:43024 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az74-467.rg1nh:42990 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az74-467.rg1nh:42988 13.107.42.16:https      ESTABLISHED
Active UNIX domain sockets (w/o servers)
Proto RefCnt Flags       Type       State         I-Node   Path
unix  2      [ ]         DGRAM                    26818    /run/user/1001/systemd/notify
unix  3      [ ]         DGRAM      CONNECTED     13992    /run/systemd/notify
unix  2      [ ]         DGRAM                    14009    /run/systemd/journal/syslog
unix  9      [ ]         DGRAM      CONNECTED     14019    /run/systemd/journal/dev-log
unix  10     [ ]         DGRAM      CONNECTED     14023    /run/systemd/journal/socket
unix  2      [ ]         DGRAM      CONNECTED     23117    /run/chrony/chronyd.sock
unix  2      [ ]         DGRAM                    28369    @00014
unix  3      [ ]         STREAM     CONNECTED     27762    
unix  3      [ ]         STREAM     CONNECTED     23475    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM      CONNECTED     24600    
unix  3      [ ]         STREAM     CONNECTED     23553    
unix  3      [ ]         STREAM     CONNECTED     32707    
unix  2      [ ]         DGRAM      CONNECTED     15816    
unix  3      [ ]         STREAM     CONNECTED     22697    
unix  2      [ ]         DGRAM      CONNECTED     23101    
unix  3      [ ]         STREAM     CONNECTED     27755    
unix  3      [ ]         STREAM     CONNECTED     22822    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     21209    
unix  3      [ ]         STREAM     CONNECTED     26699    
unix  3      [ ]         STREAM     CONNECTED     32708    /run/dbus/system_bus_socket
unix  3      [ ]         DGRAM      CONNECTED     18750    
unix  3      [ ]         STREAM     CONNECTED     26822    
unix  3      [ ]         STREAM     CONNECTED     27225    
unix  3      [ ]         STREAM     CONNECTED     26805    /run/dbus/system_bus_socket
unix  3      [ ]         SEQPACKET  CONNECTED     23119    
unix  3      [ ]         STREAM     CONNECTED     22813    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     23366    /run/systemd/journal/stdout
unix  3      [ ]         DGRAM      CONNECTED     15819    
unix  3      [ ]         STREAM     CONNECTED     23096    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     21376    
unix  3      [ ]         STREAM     CONNECTED     18754    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     25074    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     19325    
unix  2      [ ]         DGRAM      CONNECTED     16299    
unix  3      [ ]         STREAM     CONNECTED     23095    
unix  3      [ ]         STREAM     CONNECTED     21515    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     25071    
unix  3      [ ]         STREAM     CONNECTED     20508    
unix  3      [ ]         STREAM     CONNECTED     27754    
unix  3      [ ]         STREAM     CONNECTED     26823    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     28804    /run/containerd/containerd.sock
unix  3      [ ]         STREAM     CONNECTED     22992    
unix  3      [ ]         STREAM     CONNECTED     23869    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM      CONNECTED     28370    
unix  3      [ ]         STREAM     CONNECTED     27746    
unix  3      [ ]         STREAM     CONNECTED     22815    /run/dbus/system_bus_socket
unix  2      [ ]         DGRAM                    30655    
unix  2      [ ]         DGRAM      CONNECTED     22809    
unix  3      [ ]         STREAM     CONNECTED     23211    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     32810    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     19912    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM      CONNECTED     15474    
unix  3      [ ]         STREAM     CONNECTED     22812    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     24682    /run/systemd/journal/stdout
unix  3      [ ]         DGRAM      CONNECTED     13994    
unix  3      [ ]         STREAM     CONNECTED     27227    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22912    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     30670    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     23871    
unix  3      [ ]         STREAM     CONNECTED     25682    
unix  3      [ ]         STREAM     CONNECTED     21673    
unix  3      [ ]         STREAM     CONNECTED     28806    
unix  3      [ ]         STREAM     CONNECTED     32808    
unix  3      [ ]         STREAM     CONNECTED     23975    /run/systemd/journal/stdout
unix  3      [ ]         DGRAM      CONNECTED     19332    
unix  3      [ ]         STREAM     CONNECTED     16270    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22699    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22811    
unix  3      [ ]         STREAM     CONNECTED     23976    /run/systemd/journal/stdout
unix  3      [ ]         DGRAM      CONNECTED     13993    
unix  3      [ ]         STREAM     CONNECTED     25072    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     22524    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     32822    
unix  3      [ ]         DGRAM      CONNECTED     19334    
unix  3      [ ]         STREAM     CONNECTED     16269    
unix  3      [ ]         DGRAM      CONNECTED     26819    
unix  3      [ ]         STREAM     CONNECTED     26979    
unix  3      [ ]         STREAM     CONNECTED     22993    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     23329    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     25073    
unix  3      [ ]         DGRAM      CONNECTED     18749    
unix  3      [ ]         DGRAM      CONNECTED     15818    
unix  2      [ ]         DGRAM                    23327    
unix  3      [ ]         STREAM     CONNECTED     22289    
unix  2      [ ]         DGRAM      CONNECTED     19327    
unix  3      [ ]         STREAM     CONNECTED     17729    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     28807    /run/containerd/containerd.sock
unix  3      [ ]         STREAM     CONNECTED     22810    
unix  3      [ ]         STREAM     CONNECTED     23328    
unix  2      [ ]         DGRAM      CONNECTED     21674    
unix  2      [ ]         DGRAM      CONNECTED     14296    
unix  2      [ ]         DGRAM      CONNECTED     24968    
unix  3      [ ]         STREAM     CONNECTED     26701    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     23116    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     14915    
unix  3      [ ]         STREAM     CONNECTED     24199    
unix  2      [ ]         DGRAM      CONNECTED     24969    
unix  3      [ ]         STREAM     CONNECTED     19927    /run/systemd/journal/stdout
unix  3      [ ]         SEQPACKET  CONNECTED     23118    
unix  3      [ ]         DGRAM      CONNECTED     26820    
unix  3      [ ]         STREAM     CONNECTED     26978    
unix  3      [ ]         STREAM     CONNECTED     22907    
unix  2      [ ]         DGRAM      CONNECTED     26726    
unix  3      [ ]         DGRAM      CONNECTED     19333    
unix  3      [ ]         STREAM     CONNECTED     24322    
unix  3      [ ]         STREAM     CONNECTED     22293    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM      CONNECTED     20513    
unix  3      [ ]         STREAM     CONNECTED     27763    
unix  3      [ ]         STREAM     CONNECTED     18208    
unix  3      [ ]         STREAM     CONNECTED     28803    
unix  3      [ ]         STREAM     CONNECTED     26804    
unix  3      [ ]         STREAM     CONNECTED     22814    /run/dbus/system_bus_socket
unix  2      [ ]         DGRAM      CONNECTED     32819    
unix  3      [ ]         STREAM     CONNECTED     21986    
unix  3      [ ]         STREAM     CONNECTED     14928    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     23706    
unix  3      [ ]         STREAM     CONNECTED     23972    
unix  2      [ ]         DGRAM      CONNECTED     26752    
unix  3      [ ]         STREAM     CONNECTED     21377    
unix  3      [ ]         DGRAM      CONNECTED     19331    
unix  3      [ ]         STREAM     CONNECTED     17728    
unix  3      [ ]         STREAM     CONNECTED     22449    
unix  3      [ ]         STREAM     CONNECTED     21210    
unix  3      [ ]         STREAM     CONNECTED     27747    
unix  3      [ ]         STREAM     CONNECTED     21596    
***************************************************************************************************************************************************************
###############################################################################################################################################################
## process Monitoring(ps,top,htop,atop,lsof)
- ps
    PID TTY          TIME CMD
    847 ?        00:00:00 systemd
    857 ?        00:00:00 (sd-pam)
   1495 ?        00:00:02 Runner.Listener
   1512 ?        00:00:03 Runner.Worker
   1616 ?        00:00:00 bash
   1645 ?        00:00:00 sh
   1667 ?        00:00:00 ps
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
