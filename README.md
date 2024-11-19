### Weathering With U Deployment

### Configuring Github
1.Set the repository secret for SSH_PRIVATE_KEY and VAULT_PASSWORD

2.Update the inventory file for the server ip

3.Clone this repository inside the server as deploy directory

4.Run the action to verify the configuration

### Install ansible
sudo apt install ansible-core

### Deploy APP
ansible-playbook playbook/deploy_app_dev.yml -i playbook/inventory.yml

### Stop APP
ansible-playbook playbook/stop_app_dev.yml -i playbook/inventory.yml
