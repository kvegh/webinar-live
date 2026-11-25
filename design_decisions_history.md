# Design decisions history

## 2026-11-25 (CET): first version 0.0.1

- User request: new public repository with a playbook that restarts the
  Windows DNS service if it has failed; nothing else.
- Native `ansible.windows.win_service` with `state: started`, target group
  `dns_servers`.
