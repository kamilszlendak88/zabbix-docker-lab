# LAB 11 – Ansible: Zabbix Agent2 + Handlers

## Goal
Install and configure Zabbix Agent2 using Ansible and validate handler-based restarts.

## Approach
- Zabbix Agent2 installed via apt
- Configuration deployed using an Ansible template
- Zabbix Server IP was discovered dynamically from the Docker container
- A handler restarts the agent only when configuration changes

## Result
Zabbix Agent2 is installed, enabled and running.
Configuration management is reproducible and idempotent.

## Verification
- systemctl status zabbix-agent2: active (running)
- ss -lntp: port 10050 is listening

Connectivity was verified from the Zabbix Server container perspective:
- Default gateway from `zbx-server`: 172.18.0.1
- TCP check: `nc -vz 172.18.0.1 10050` -> open

Agent status on the host:
- `systemctl status zabbix-agent2` -> active (running)
- `ss -lntp | grep 10050` -> LISTEN
