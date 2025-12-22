# homelab-ansible-roles

Reusable Ansible roles for homelab infrastructure.

## Structure

```
roles/
└── <role_name>/
    ├── tasks/
    ├── handlers/
    ├── templates/
    ├── files/
    ├── vars/
    ├── defaults/
    └── meta/
```

## Usage

Include roles via `requirements.yml`:

```yaml
- src: git@github.com:RobertYoung/homelab-ansible-roles.git
  scm: git
  version: main
```

Install with:

```bash
ansible-galaxy install -r requirements.yml
```

## Requirements

- Ansible >= 2.15

## License

MIT
