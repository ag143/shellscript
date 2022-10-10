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
Linux 5.15.0-1020-azure (fv-az573-523) 	10/10/22 	_x86_64_	(2 CPU)

avg-cpu:  %user   %nice %system %iowait  %steal   %idle
           6.49    0.11    6.94    1.34    0.00   85.11

Device             tps    kB_read/s    kB_wrtn/s    kB_dscd/s    kB_read    kB_wrtn    kB_dscd
loop0             1.76        15.33         0.00         0.00       2250          0          0
loop1             0.46         7.49         0.00         0.00       1100          0          0
loop2             6.18       234.76         0.00         0.00      34456          0          0
loop3             0.07         0.10         0.00         0.00         14          0          0
sda             322.85      5454.50      1154.14    207659.72     800557     169393   30478217
sdb               5.57        81.55      2041.70    168946.16      11969     299660   24796228


***************************************************************************************************************************************************************
- sar
***************************************************************************************************************************************************************
- vmstat
procs -----------memory---------- ---swap-- -----io---- -system-- ------cpu-----
 r  b   swpd   free   buff  cache   si   so    bi    bo   in   cs us sy id wa st
 1  0      0 5271236 215156 1057084    0    0  2947  1625  160  867  7  7 85  1  0
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
/dev/root       87204404 54976180  32211840  64% /
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
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 25523
;; flags: qr rd ra; QUERY: 1, ANSWER: 13, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 65494
;; QUESTION SECTION:
;.				IN	NS

;; ANSWER SECTION:
.			6112	IN	NS	a.root-servers.net.
.			6112	IN	NS	h.root-servers.net.
.			6112	IN	NS	k.root-servers.net.
.			6112	IN	NS	i.root-servers.net.
.			6112	IN	NS	j.root-servers.net.
.			6112	IN	NS	m.root-servers.net.
.			6112	IN	NS	g.root-servers.net.
.			6112	IN	NS	c.root-servers.net.
.			6112	IN	NS	f.root-servers.net.
.			6112	IN	NS	b.root-servers.net.
.			6112	IN	NS	d.root-servers.net.
.			6112	IN	NS	e.root-servers.net.
.			6112	IN	NS	l.root-servers.net.

;; Query time: 4 msec
;; SERVER: 127.0.0.53#53(127.0.0.53)
;; WHEN: Mon Oct 10 07:36:12 UTC 2022
;; MSG SIZE  rcvd: 239

***************************************************************************************************************************************************************
- iptables
***************************************************************************************************************************************************************
- netstat
Active Internet connections (w/o servers)
Proto Recv-Q Send-Q Local Address           Foreign Address         State      
tcp        0      0 fv-az573-523.uspn:44302 lb-192-30-255-113:https TIME_WAIT  
tcp6       0      0 fv-az573-523.uspn:45860 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az573-523.uspn:45856 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az573-523.uspn:55494 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az573-523.uspn:60170 lb-192-30-255-121:https TIME_WAIT  
tcp6       0      0 fv-az573-523.uspn:46792 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az573-523.uspn:42110 lb-192-30-255-116:https TIME_WAIT  
tcp6       0      0 fv-az573-523.uspn:45830 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az573-523.uspn:45854 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az573-523.uspn:45832 13.107.42.16:https      ESTABLISHED
tcp6       0      0 fv-az573-523.uspn:45852 13.107.42.16:https      ESTABLISHED
Active UNIX domain sockets (w/o servers)
Proto RefCnt Flags       Type       State         I-Node   Path
unix  2      [ ]         DGRAM                    26799    /run/user/1001/systemd/notify
unix  3      [ ]         DGRAM      CONNECTED     1439     /run/systemd/notify
unix  2      [ ]         DGRAM                    1456     /run/systemd/journal/syslog
unix  9      [ ]         DGRAM      CONNECTED     1466     /run/systemd/journal/dev-log
unix  9      [ ]         DGRAM      CONNECTED     1470     /run/systemd/journal/socket
unix  2      [ ]         DGRAM      CONNECTED     21073    /run/chrony/chronyd.sock
unix  2      [ ]         DGRAM                    28709    @00014
unix  3      [ ]         STREAM     CONNECTED     26803    
unix  2      [ ]         DGRAM      CONNECTED     1941     
unix  3      [ ]         STREAM     CONNECTED     26070    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     21067    
unix  3      [ ]         STREAM     CONNECTED     22474    /run/dbus/system_bus_socket
unix  3      [ ]         DGRAM      CONNECTED     26801    
unix  2      [ ]         DGRAM      CONNECTED     20540    
unix  3      [ ]         STREAM     CONNECTED     23433    
unix  3      [ ]         DGRAM      CONNECTED     15520    
unix  3      [ ]         STREAM     CONNECTED     26493    
unix  3      [ ]         STREAM     CONNECTED     19874    
unix  3      [ ]         STREAM     CONNECTED     26950    
unix  3      [ ]         STREAM     CONNECTED     23198    
unix  3      [ ]         DGRAM      CONNECTED     20547    
unix  3      [ ]         STREAM     CONNECTED     23754    
unix  2      [ ]         DGRAM      CONNECTED     21070    
unix  3      [ ]         DGRAM      CONNECTED     1440     
unix  3      [ ]         STREAM     CONNECTED     26342    
unix  3      [ ]         STREAM     CONNECTED     21297    
unix  3      [ ]         STREAM     CONNECTED     31983    /run/dbus/system_bus_socket
unix  2      [ ]         DGRAM      CONNECTED     25371    
unix  3      [ ]         DGRAM      CONNECTED     20544    
unix  3      [ ]         STREAM     CONNECTED     20568    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22473    
unix  2      [ ]         DGRAM      CONNECTED     16875    
unix  3      [ ]         DGRAM      CONNECTED     18229    
unix  3      [ ]         STREAM     CONNECTED     27346    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22268    
unix  3      [ ]         STREAM     CONNECTED     21970    
unix  3      [ ]         STREAM     CONNECTED     28760    /run/containerd/containerd.sock
unix  3      [ ]         STREAM     CONNECTED     21458    
unix  3      [ ]         STREAM     CONNECTED     22888    
unix  3      [ ]         STREAM     CONNECTED     20924    
unix  3      [ ]         STREAM     CONNECTED     28756    
unix  3      [ ]         STREAM     CONNECTED     24442    
unix  3      [ ]         DGRAM      CONNECTED     15521    
unix  2      [ ]         DGRAM      CONNECTED     19879    
unix  3      [ ]         STREAM     CONNECTED     24015    
unix  3      [ ]         STREAM     CONNECTED     18240    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     26081    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM      CONNECTED     26742    
unix  2      [ ]         DGRAM      CONNECTED     22274    
unix  3      [ ]         STREAM     CONNECTED     21801    
unix  3      [ ]         DGRAM      CONNECTED     1441     
unix  3      [ ]         STREAM     CONNECTED     26951    
unix  3      [ ]         STREAM     CONNECTED     23530    
unix  3      [ ]         STREAM     CONNECTED     26343    
unix  3      [ ]         STREAM     CONNECTED     29640    
unix  3      [ ]         STREAM     CONNECTED     25664    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     20538    
unix  3      [ ]         STREAM     CONNECTED     22472    
unix  2      [ ]         DGRAM      CONNECTED     22471    
unix  3      [ ]         STREAM     CONNECTED     26804    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     19729    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     26034    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     26015    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     26155    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM      CONNECTED     28710    
unix  3      [ ]         STREAM     CONNECTED     22967    
unix  3      [ ]         DGRAM      CONNECTED     26800    
unix  3      [ ]         STREAM     CONNECTED     21969    
unix  3      [ ]         STREAM     CONNECTED     26118    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     15509    
unix  3      [ ]         STREAM     CONNECTED     25990    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     26157    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     26891    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     26117    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     26778    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22477    /run/dbus/system_bus_socket
unix  2      [ ]         DGRAM                    23593    
unix  3      [ ]         STREAM     CONNECTED     26065    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     26890    
unix  3      [ ]         STREAM     CONNECTED     23355    
unix  3      [ ]         STREAM     CONNECTED     26349    
unix  3      [ ]         STREAM     CONNECTED     16323    
unix  3      [ ]         STREAM     CONNECTED     28757    /run/containerd/containerd.sock
unix  2      [ ]         DGRAM      CONNECTED     14300    
unix  3      [ ]         STREAM     CONNECTED     25983    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     25731    /run/systemd/journal/stdout
unix  3      [ ]         SEQPACKET  CONNECTED     21074    
unix  3      [ ]         STREAM     CONNECTED     26067    /run/systemd/journal/stdout
unix  3      [ ]         DGRAM      CONNECTED     18230    
unix  3      [ ]         STREAM     CONNECTED     24046    /run/dbus/system_bus_socket
unix  3      [ ]         DGRAM      CONNECTED     20545    
unix  3      [ ]         STREAM     CONNECTED     28759    
unix  2      [ ]         DGRAM      CONNECTED     25568    
unix  3      [ ]         STREAM     CONNECTED     17169    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     16867    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM      CONNECTED     24022    
unix  3      [ ]         STREAM     CONNECTED     22475    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     23755    /run/dbus/system_bus_socket
unix  2      [ ]         DGRAM                    33101    
unix  3      [ ]         STREAM     CONNECTED     26718    
unix  3      [ ]         STREAM     CONNECTED     26356    
unix  3      [ ]         STREAM     CONNECTED     15246    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22476    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     22656    
unix  3      [ ]         STREAM     CONNECTED     24045    
unix  3      [ ]         STREAM     CONNECTED     26348    
unix  3      [ ]         STREAM     CONNECTED     18789    
unix  3      [ ]         STREAM     CONNECTED     21459    
unix  3      [ ]         STREAM     CONNECTED     21300    
unix  3      [ ]         STREAM     CONNECTED     16866    
unix  3      [ ]         STREAM     CONNECTED     24650    
unix  3      [ ]         STREAM     CONNECTED     22657    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     26162    /run/systemd/journal/stdout
unix  3      [ ]         SEQPACKET  CONNECTED     21075    
unix  3      [ ]         STREAM     CONNECTED     26357    
unix  2      [ ]         DGRAM      CONNECTED     15518    
unix  3      [ ]         STREAM     CONNECTED     26064    /run/systemd/journal/stdout
unix  2      [ ]         DGRAM      CONNECTED     26729    
unix  3      [ ]         STREAM     CONNECTED     22272    
unix  3      [ ]         DGRAM      CONNECTED     20546    
***************************************************************************************************************************************************************
###############################################################################################################################################################
## process Monitoring(ps,top,htop,atop,lsof)
- ps
    PID TTY          TIME CMD
    864 ?        00:00:00 systemd
    868 ?        00:00:00 (sd-pam)
   1540 ?        00:00:02 Runner.Listener
   1555 ?        00:00:03 Runner.Worker
   1663 ?        00:00:00 bash
   1688 ?        00:00:00 sh
   1711 ?        00:00:00 ps
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
