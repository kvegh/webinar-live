# Design decisions history

## 2026-11-25 (CET): Zabbix rulebook, version 0.0.2

- User request: rulebook that reacts to the monitoring event and runs the
  restart job automatically (activation only after approval).
- `ansible.eda.webhook` source, replaced in AAP by the EDA event stream Zabbix
  posts to; rule matches problems containing "DNS" with `event_value == 1`.

## 2026-11-25 (CET): first version 0.0.1

- User request: new public repository with a playbook that restarts the
  Windows DNS service if it has failed; nothing else.
- Native `ansible.windows.win_service` with `state: started`, target group
  `dns_servers`.
