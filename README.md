

[![Build Status](https://drone.kiwi-labs.net/api/badges/Diesel-Net/cerebro/status.svg)](https://drone.kiwi-labs.net/Diesel-Net/cerebro)

# cerebro
Elasticsearch Cluster Admin WebUI

## Notes
- [Crebro Configuration](https://marcofranssen.nl/building-a-elasticsearch-cluster-using-docker-compose-and-traefik#cerebro-as-your-elasticsearch-admin-interface)
  

## Installing External Dependencies
Ansible `2.10.3` was used at the time of this writing.
```bash
ansible-galaxy install -r .ansible/roles/requirements.deploy.yaml -p .ansible/roles --force
```

## Deploy
```bash
ansible-playbook .ansible/deploy.yaml -i .ansible/inventories/production/hosts --vault-id ~/.tokens/vault.txt
```
