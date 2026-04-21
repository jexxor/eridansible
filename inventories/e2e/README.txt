E2E / lab inventory (single VM)
-------------------------------

group_vars/all/     - host-wide: network (nip.io), base OS, firewall, Docker, vault
group_vars/matrix/  - Matrix stack, Caddy, validation (hosts in the matrix group)

Secrets: group_vars/all/vault.yml (ansible-vault). Example plaintext keys:
group_vars/all/vault.example.yml

Default vault password file: vault_password.demo (see repo ansible.cfg).

Run:
  ansible-playbook -i inventories/e2e/inventory.yml playbooks/bootstrap.yml
