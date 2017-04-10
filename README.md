# Ansible RHEV/Ovirt
Playbook to create, customize and run VMs on RHV/Ovirt
Uses Version 4 of the RHV/Ovirt API

What the example does:
- Creates VMs as defined in teh Vars file
- uses cloud-init to set static IPs, password and shared key
- adds a second disk to each VM
- reboots all VMs (to apply IP changes)

Requires:
- python-ovirt-engine-sdk4-4.1 (and up, don't use sdk4-4-0.x it has bugs)

Tested with python-ovirt-engine-sdk4-4.1.3-2 and the rhel7-cloud-image as template
