# DGTL-DIGDCN-2937 - Discovery Playbooks

Sample Ansible playbook used for Discovery Demo during DGTL-DIGDCN-2937 at Cisco Live US 2020

---

## File Structure

| File Path | Description |
| :-------- | :--------- |
| `inventory.yaml` | Inventory file listing devices to pull data from, credentials, etc. Actual device names, etc. have been replaced with "placeholder" values are enclosed within < > characters |
| `network-discovery.yaml`| The discovery playbook it self |
| `commands.yaml` | Lists the set of CLI commands to executed during discovery |

## Tested Software Versions

For the discovery demo where the following software versions used:

* Ansible 2.9.1 (using Python 2.7.5)
* Cisco Nexus 9000 running NX-OS 7.0(3)I7(7)

## Installation

During the demo was Ansible running inside a docker container for ease of portability, but it could as well have run directly on a Linux host / VM.
