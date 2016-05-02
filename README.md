# Description
Monitoring DHCP requests in dnsmasq via zabbix agent.

# Dependencies
Required GNU awk, sudo, zabbix_sender.

# Installation

```
mkdir /etc/zabbix/scripts
chown zabbix:zabbix /etc/zabbix/scripts
cp zabbix/scripts/dhsmasq_dhcp.sh /etc/zabbix/scripts
cp zabbix/zabbix_agentd.d/dhsmasq_dhcp.conf /etc/zabbix/zabbix_agentd.d
service zabbix-agent restart
```
Goto zabbix web gui and import template for you zabbix version from `template` directory.
