# DGTL-DIGDCN-2937 - Discovery Analysis Script

Sample Python scripts used for Discovery Analysis Demo during DGTL-DIGDCN-2937 at Cisco Live US 2020

---

## File Structure

| File Path | Description |
| :-------- | :--------- |
| `analysis.py` | Python script to analyse discovered state. Output is controlled using `composer.yaml` |
| `data_model.yaml` | File that provides the mapping between CLI command / Configuration item to textFSM parser |
| `composer.yaml`| File that controls which Sheets to create and which columns to include in each sheet when executing the `analysis.py` Python script |
| `parsers/cisco_nxos_config_acl.textfsm`| TextFSM parser for NXOS ACL Config |
| `parsers/cisco_nxos_config_interface.textfsm`| TextFSM parser for NXOS Interface Config |
| `parsers/cisco_nxos_show_hsrp_brief.textfsm`| TextFSM parser for NXOS CLI Command "show hsrp brief" |
| `parsers/cisco_nxos_show_ip_arp_vrf_all.textfsm`| TextFSM parser for NXOS CLI Command "show ip arp vrf all" |
| `parsers/cisco_nxos_show_mac_address-table.textfsm`| TextFSM parser for NXOS CLI Command "show mac address-table" |
| `parsers/cisco_nxos_show_vrf_all_interface.textfsm`| TextFSM parser for NXOS CLI Command "show vrf all interface" |
| `parsers/cisco_nxos_show_vrf.textfsm`| TextFSM parser for NXOS CLI Command "show vrf" |
| `requirements.txt` | Requirements file specifying the Python modules required |

## Tested Software Versions

For the discovery demo where the following software versions used:

* Python 3.6.8)
* Cisco Nexus 9000 running NX-OS 7.0(3)I7(7)

## Installation

During the demo was Python running inside a docker container for ease of portability, but it could as well have run directly on a Linux host / VM.
