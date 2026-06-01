wslinux01
---

No LSB modules are available.
Distributor ID: Ubuntu
Description:    Ubuntu 24.04.4 LTS
Release:        24.04
Codename:       noble
---

1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN group default qlen 1000
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
    inet 127.0.0.1/8 scope host lo
       valid_lft forever preferred_lft forever
    inet6 ::1/128 scope host noprefixroute
       valid_lft forever preferred_lft forever
2: enp0s3: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc fq_codel state UP group default qlen 1000
    link/ether 08:00:27:23:3a:f5 brd ff:ff:ff:ff:ff:ff
    inet 10.24.82.216/24 brd 10.24.82.255 scope global enp0s3
       valid_lft forever preferred_lft forever
    inet 10.24.82.47/24 metric 100 brd 10.24.82.255 scope global secondary dynamic enp0s3
       valid_lft 27786sec preferred_lft 27786sec
---

default via 10.24.82.1 dev enp0s3 proto static
default via 10.24.82.1 dev enp0s3 proto dhcp src 10.24.82.47 metric 100
10.1.1.195 via 10.24.82.1 dev enp0s3 proto dhcp src 10.24.82.47 metric 100
10.1.1.242 via 10.24.82.1 dev enp0s3 proto dhcp src 10.24.82.47 metric 100
10.24.40.190 via 10.24.82.1 dev enp0s3 proto dhcp src 10.24.82.47 metric 100
10.24.82.0/24 dev enp0s3 proto kernel scope link src 10.24.82.216
10.24.82.1 dev enp0s3 proto dhcp scope link src 10.24.82.47 metric 100
---

Global
         Protocols: -LLMNR -mDNS -DNSOverTLS DNSSEC=no/unsupported
  resolv.conf mode: stub

Link 2 (enp0s3)
    Current Scopes: DNS
         Protocols: +DefaultRoute -LLMNR -mDNS -DNSOverTLS DNSSEC=no/unsupported
Current DNS Server: 8.8.8.8
       DNS Servers: 8.8.8.8 8.8.4.4 10.24.40.190 10.1.1.195 10.1.1.242
        DNS Domain: senac.br senacsp.edu.br
---

COMMAND    PID            USER   FD   TYPE DEVICE SIZE/OFF NODE NAME
systemd      1            root  196u  IPv4   8229      0t0  TCP *:22 (LISTEN)
systemd-r  571 systemd-resolve   14u  IPv4   7042      0t0  UDP 127.0.0.53:53
systemd-r  571 systemd-resolve   15u  IPv4   7043      0t0  TCP 127.0.0.53:53 (LISTEN)
systemd-r  571 systemd-resolve   16u  IPv4   7044      0t0  UDP 127.0.0.54:53
systemd-r  571 systemd-resolve   17u  IPv4   7045      0t0  TCP 127.0.0.54:53 (LISTEN)
systemd-n  595 systemd-network   19u  IPv4  14657      0t0  UDP 10.24.82.47:68
node_expo  732   node_exporter    3u  IPv6   9870      0t0  TCP *:9100 (LISTEN)
node_expo  732   node_exporter    6u  IPv6  15398      0t0  TCP 127.0.0.1:9100->127.0.0.1:59892 (ESTABLISHED)
prometheu  739      prometheus    6u  IPv6   9183      0t0  TCP *:9091 (LISTEN)
prometheu  739      prometheus    8u  IPv6  15369      0t0  TCP 127.0.0.1:9091->127.0.0.1:60516 (ESTABLISHED)
prometheu  739      prometheus   11u  IPv4  15397      0t0  TCP 127.0.0.1:59892->127.0.0.1:9100 (ESTABLISHED)
prometheu  739      prometheus   16u  IPv4  15368      0t0  TCP 127.0.0.1:60516->127.0.0.1:9091 (ESTABLISHED)
apache2    802            root    3u  IPv4   8431      0t0  TCP *:80 (LISTEN)
apache2    802            root    4u  IPv4   8433      0t0  TCP *:8888 (LISTEN)
java       836          tomcat   44u  IPv6   9202      0t0  TCP *:8080 (LISTEN)
mysqld     936           mysql   21u  IPv6  10116      0t0  TCP *:33060 (LISTEN)
mysqld     936           mysql   33u  IPv4  10118      0t0  TCP *:3306 (LISTEN)
apache2   1048        www-data    3u  IPv4   8431      0t0  TCP *:80 (LISTEN)
apache2   1048        www-data    4u  IPv4   8433      0t0  TCP *:8888 (LISTEN)
apache2   1049        www-data    3u  IPv4   8431      0t0  TCP *:80 (LISTEN)
apache2   1049        www-data    4u  IPv4   8433      0t0  TCP *:8888 (LISTEN)
apache2   1050        www-data    3u  IPv4   8431      0t0  TCP *:80 (LISTEN)
apache2   1050        www-data    4u  IPv4   8433      0t0  TCP *:8888 (LISTEN)
apache2   1053        www-data    3u  IPv4   8431      0t0  TCP *:80 (LISTEN)
apache2   1053        www-data    4u  IPv4   8433      0t0  TCP *:8888 (LISTEN)
apache2   1054        www-data    3u  IPv4   8431      0t0  TCP *:80 (LISTEN)
apache2   1054        www-data    4u  IPv4   8433      0t0  TCP *:8888 (LISTEN)
grafana   1137         grafana   16u  IPv6  10262      0t0  TCP *:3000 (LISTEN)
sshd      1975            root    3u  IPv4   8229      0t0  TCP *:22 (LISTEN)
sshd      1977            root    4u  IPv4  15253      0t0  TCP 10.24.82.216:22->10.24.82.38:53511 (ESTABLISHED)
sshd      2077           senac    4u  IPv4  15253      0t0  TCP 10.24.82.216:22->10.24.82.38:53511 (ESTABLISHED)
---

