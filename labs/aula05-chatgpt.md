COMMAND    PID            USER   FD   TYPE DEVICE SIZE/OFF NODE NAME
systemd      1            root   92u  IPv4   8221      0t0  TCP *:22 (LISTEN)
systemd-n  560 systemd-network   11u  IPv4   8758      0t0  UDP 10.24.82.47:68
systemd-r  572 systemd-resolve   14u  IPv4   6957      0t0  UDP 127.0.0.53:53
systemd-r  572 systemd-resolve   15u  IPv4   6958      0t0  TCP 127.0.0.53:53 (LISTEN)
systemd-r  572 systemd-resolve   16u  IPv4   6959      0t0  UDP 127.0.0.54:53
systemd-r  572 systemd-resolve   17u  IPv4   6960      0t0  TCP 127.0.0.54:53 (LISTEN)
node_expo  685   node_exporter    3u  IPv6   7941      0t0  TCP *:9100 (LISTEN)
node_expo  685   node_exporter    7u  IPv6   8912      0t0  TCP 127.0.0.1:9100->127.0.0.1:42452 (ESTABLISHED)
prometheu  699      prometheus    6u  IPv6   8721      0t0  TCP *:9091 (LISTEN)
prometheu  699      prometheus   11u  IPv4   9795      0t0  TCP 127.0.0.1:42452->127.0.0.1:9100 (ESTABLISHED)
prometheu  699      prometheus   20u  IPv6   9773      0t0  TCP 127.0.0.1:9091->127.0.0.1:41350 (ESTABLISHED)
prometheu  699      prometheus   24u  IPv4   9772      0t0  TCP 127.0.0.1:41350->127.0.0.1:9091 (ESTABLISHED)
apache2    771            root    3u  IPv4   8399      0t0  TCP *:80 (LISTEN)
apache2    771            root    4u  IPv4   8401      0t0  TCP *:8888 (LISTEN)
java       773          tomcat   44u  IPv6   8757      0t0  TCP *:8080 (LISTEN)
mysqld     834           mysql   21u  IPv6   8761      0t0  TCP *:33060 (LISTEN)
mysqld     834           mysql   39u  IPv4   9551      0t0  TCP *:3306 (LISTEN)
apache2    851        www-data    3u  IPv4   8399      0t0  TCP *:80 (LISTEN)
apache2    851        www-data    4u  IPv4   8401      0t0  TCP *:8888 (LISTEN)
apache2    852        www-data    3u  IPv4   8399      0t0  TCP *:80 (LISTEN)
apache2    852        www-data    4u  IPv4   8401      0t0  TCP *:8888 (LISTEN)
apache2    853        www-data    3u  IPv4   8399      0t0  TCP *:80 (LISTEN)
apache2    853        www-data    4u  IPv4   8401      0t0  TCP *:8888 (LISTEN)
apache2    854        www-data    3u  IPv4   8399      0t0  TCP *:80 (LISTEN)
apache2    854        www-data    4u  IPv4   8401      0t0  TCP *:8888 (LISTEN)
apache2    858        www-data    3u  IPv4   8399      0t0  TCP *:80 (LISTEN)
apache2    858        www-data    4u  IPv4   8401      0t0  TCP *:8888 (LISTEN)
grafana    993         grafana   13u  IPv6   8824      0t0  TCP *:3000 (LISTEN)
sshd      1230            root    3u  IPv4   8221      0t0  TCP *:22 (LISTEN)
sshd      1606            root    4u  IPv4  13448      0t0  TCP 10.24.82.216:22->10.24.82.39:58270 (ESTABLISHED)
sshd      1680           senac    4u  IPv4  13448      0t0  TCP 10.24.82.216:22->10.24.82.39:58270 (ESTABLISHED)
---

apache2.service             loaded active running The Apache HTTP Server
  cron.service                loaded active running Regular background program processing daemon
  dbus.service                loaded active running D-Bus System Message Bus
  fwupd.service               loaded active running Firmware update daemon
  getty@tty1.service          loaded active running Getty on tty1
  grafana-server.service      loaded active running Grafana instance
  ModemManager.service        loaded active running Modem Manager
  multipathd.service          loaded active running Device-Mapper Multipath Device Controller
  mysql.service               loaded active running MySQL Community Server
  node_exporter.service       loaded active running Node Exporter
  polkit.service              loaded active running Authorization Manager
  prometheus.service          loaded active running Prometheus
  rsyslog.service             loaded active running System Logging Service
  ssh.service                 loaded active running OpenBSD Secure Shell server
  systemd-journald.service    loaded active running Journal Service
  systemd-logind.service      loaded active running User Login Management
  systemd-networkd.service    loaded active running Network Configuration
  systemd-resolved.service    loaded active running Network Name Resolution
  systemd-timesyncd.service   loaded active running Network Time Synchronization
  systemd-udevd.service       loaded active running Rule-based Manager for Device Events and Files
  tomcat11.service            loaded active running Apache Tomcat11
  udisks2.service             loaded active running Disk Manager
  unattended-upgrades.service loaded active running Unattended Upgrades Shutdown
  upower.service              loaded active running Daemon for power management
  user@1000.service           loaded active running User Manager for UID 1000
  ---