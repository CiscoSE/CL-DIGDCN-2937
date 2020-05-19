# DGTL-DIGDCN-2937 - Migration Playbooks

Sample Ansible playbook used for Migration Demo during DGTL-DIGDCN-2937 at Cisco Live US 2020

---

## File Structure

| File Path | Description |
| :-------- | :--------- |
| `inventory.yaml` | Inventory file listing devices to pull data from, credentials, etc. Actual device names, etc. have been replaced with "placeholder" values are enclosed within < > characters |
| `migration_data.yaml`| Variable file that contains the detailed information about VRFs, BDs, IPs, etc. being migrated |
| `pre-migration-configuration.yaml`| Playbook for appling pre-migration configuratino to ACI (create BD, EPG, EPG Bindings, etc.) |
| `l2-migration.yaml`| Playbook for performing the Layer-2 migration step (VM move from a network point of view) |
| `l3-migration.yaml`| Playbook for performing Layer-3 migration step (move subnet from current network to ACI) |
| `rollback-pre-migration-config.yaml`| Playbook for rolling back / deleting pre-migration configuration in ACI (BD, EPG, etc.) |
| `rollback-l2-migration.yaml`| Playbook for rolling back the Layer-2 migration step (VM move from a network point of view) |
| `rollback-l3-migration.yaml`| Playbook for rolling back the Layer-3 migration step (move subnet from current network to ACI) |

## Tested Software Versions

For the discovery demo where the following software versions used:

* Ansible 2.9.1 (using Python 2.7.5)
* VMware vSphere version 6.7
* Cisco Nexus 9000 running NX-OS 7.0(3)I7(7)
* Cisco ACI running 4.2(2f)

## Installation

During the demo was Ansible running inside a docker container for ease of portability, but it could as well have run directly on a Linux host / VM.
