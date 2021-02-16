# ansible-firewall 

This is a project to enable inbound/outbound traffic on firewalld, using ansible.

## Getting Started

To start, you'd need to clone/fork repo to your local machine.

### Prerequisites

Ansible is required to run ansible runbooks.
I was using ssh with public/private key pair to connect to my instances.

### Configuring the firewalld

Firewalld configuration is managed from firewall_config.yml file.

## Deployment

Once firewalld configration is setup, you can start the playbook by running:

```
ansible-playbook -i hosts firewall_play.yml
```

hosts file should contain all the relevant data for the hosts. In my case, those were host IP address and host variables (ssh username and private key)