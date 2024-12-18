# Nexus VLAN Deployment with Ansible

This repository demonstrates an Ansible-based approach to configure VLANs on Cisco Nexus switches.

## Features

- Uses Ansible and the `nxos_vlan` module.
- Applies VLAN configurations to multiple Nexus switches defined in `inventory.yml`.
- Variables stored in role variables for easy updates.

## Prerequisites

- Ansible installed locally.
- Access to Nexus switches via SSH.
- Python and required libraries on the control machine.

## How to Run

1. Update `inventory.yml` with your Nexus device details.
2. Adjust VLAN IDs and names in `roles/nexus_vlan/vars/main.yml`.
3. Run `ansible-playbook -i inventory.yml playbook.yml`.
4. Confirm VLANs on the Nexus switches using `show vlan`.
