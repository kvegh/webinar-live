# webinar-live

Ansible content for Windows DNS self-healing.

- `playbooks/restart-windows-dns.yml`: starts the Windows DNS Server service
  on the hosts in group `dns_servers` (override with `dns_target`).
