# LAB 09 – Ansible Basics (Configuration Management)

## Goal
Introduce Ansible as a configuration management tool and validate
idempotent behavior on a Linux system.

## Environment
- Linux (Ubuntu, ARM64)
- Ansible
- Localhost inventory (no SSH)

## Inventory
A simple local inventory was created to manage the same host
using a local connection.

## Playbook
Created a simple playbook to ensure required packages are installed.

## Idempotency
Verified that running the playbook multiple times does not introduce changes
once the desired state is achieved.

## Result
Successfully used Ansible to manage system configuration declaratively.
