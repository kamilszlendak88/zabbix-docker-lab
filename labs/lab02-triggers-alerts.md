# LAB 02 – Triggers and Alerts

## Goal
Create a custom CPU trigger and simulate an incident.

## Trigger
avg(/zbx-agent/system.cpu.util,5m) > 80

## Incident simulation
Generated sustained CPU load in the agent container (multiple `yes` processes) to exceed 80% CPU usage for >5 minutes.

## Result
Zabbix raised a problem event and automatically resolved it after the load was stopped.
