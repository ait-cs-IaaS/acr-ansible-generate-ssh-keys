# Ansible-Role: acr-ansible-generate-ssh-keys

AIT-CyberRange: Generates ssh key pairs. 


## Requirements

- Debian or Ubuntu 

## Role Variables

```yaml
# List of user to create keys for
ssh_users: []

# Basepath to store keys in
ssh_keys_base_path: ''

# Optional additional settings
ssh_type: rsa
ssh_size: 4096
ssh_mode: '0600'

```

## Example Playbook

```yaml
- hosts: localhost
  roles:
    - acr-ansible-generate-ssh-keys
      vars:
        ssh_users: []
        ssh_keys_base_path: "/tmp/data/keys"
```

## License

GPL-3.0

## Author

- Lenhard Reuter