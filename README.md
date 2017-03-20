# Ansible playbook to deploy foreman with katello scenario

Ansible playbook to deploy katello and foreman on CentOS7.

Directory structure is as below:

```
.
├── hosts
├── katello.yml
├── README.md
└── roles
    ├── katello
    │   ├── defaults
    │   │   └── main.yml
    │   ├── handlers
    │   │   └── main.yml
    │   ├── tasks
    │   │   ├── cloudstack_integration.yml
    │   │   ├── configurations.yml
    │   │   ├── firewalld.yml
    │   │   ├── foreman-plugins.yml
    │   │   ├── foreman-smart-proxy-plugins.yml
    │   │   ├── install_katello.yml
    │   │   ├── main.yml
    │   │   ├── packages.yml
    │   │   └── repos.yml
    │   ├── templates
    │   │   ├── foreman_plugins.repo.j2
    │   │   ├── foreman.repo.j2
    │   │   └── rvm_installer.sh.j2
    │   └── vars
    │       └── CentOS7.yml
    └── selinux
        ├── defaults
        │   └── main.yml
        └── tasks
            └── main.yml
```

## Using playbook

```
$ ansible-playbook -i hosts katello.yml
```

Descriptive howto will be updated soon.
