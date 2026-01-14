# LAB 07 – Network Monitoring in Zabbix

## Goal
Monitor host availability and service-level connectivity using ICMP and TCP checks.

## ICMP monitoring
ICMP ping and packet loss checks were configured using simple checks.
A trigger was created to detect host unreachability based on 100% packet loss.

## TCP port monitoring
A TCP service check was added to monitor HTTP availability on port 80.
A trigger was configured to alert when the service becomes unavailable.

## Incident simulation
Network issues were simulated by blocking ICMP traffic and stopping the HTTP service.
Alerts were triggered and resolved accordingly.

## Result
Successfully implemented network-level and service-level monitoring
with validated alerting and recovery behavior.

## Notes
TCP monitoring was adjusted to target port 10050 (Zabbix Agent),
ensuring service checks were performed from the Zabbix Server
network perspective in a Docker-based setup.
