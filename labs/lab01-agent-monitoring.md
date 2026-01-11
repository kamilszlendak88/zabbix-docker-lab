# LAB 01 – Agent-based Monitoring

## Goal
Configure agent-based monitoring for a Linux host using Zabbix Agent 2.

## Environment
- Zabbix 6.4 LTS
- Docker Compose
- Linux (ARM64)

## Configuration
- Host name: zbx-agent
- Interface: Agent (DNS)
- DNS name: zbx-agent
- Port: 10050
- Template: Linux by Zabbix agent

## Result
Host successfully monitored.
CPU, memory and disk metrics are visible in Zabbix.
Availability status is green.
