# eridansible

Ansible playbooks for a Matrix-centric server.

- **E2E:** `inventories/e2e/` — single VM, modular `group_vars` under `all/` and `matrix/`; secrets in `group_vars/all/vault.yml` (ansible-vault); shape in `group_vars/all/vault.example.yml`. See `inventories/e2e/README.txt`.
