# Red Hat Advanced Developer Suite 2026 Automation Collection

This Ansible collection provides automation roles for Red Hat Advanced Developer Suite 2026 deployments.

## Roles

### data_grid
Installs and configures Red Hat Data Grid operator and instances.

### rhads_customisation
Provides customisations for RHADS 2026 environments.

## Installation

```bash
ansible-galaxy collection install rhpds.rhads_2026_automation
```

Or via requirements file:

```yaml
collections:
  - name: https://github.com/rhpds/rhads-2026-automation.git
    type: git
    version: main
```

## Usage

```yaml
- name: Deploy Data Grid
  hosts: localhost
  roles:
    - rhpds.rhads_2026_automation.data_grid

- name: Apply RHADS Customisations
  hosts: localhost
  roles:
    - rhpds.rhads_2026_automation.rhads_customisation
```

## License

GPL-2.0-or-later

## Author Information

Red Hat Partner Demo System
