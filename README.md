# webinar-live

Ansible content for Windows DNS self-healing.

- `playbooks/restart-windows-dns.yml`: starts the Windows DNS Server service
  on the hosts in group `dns_servers` (override with `dns_target`).
- `extensions/eda/rulebooks/zabbix-dns-restart.yml`: rulebook that launches the
  job template "Webinar - Restart Windows DNS" when a Zabbix problem whose name
  contains "DNS" fires (`event_value == 1`).
