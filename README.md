# ansible-create-users
Ansible Playbook to create multiple users and deploy SSH keypairs

Usage

1. Populate the inventory file (inventory.yml) with your intended Linux Hosts
2. Change ```remote_user``` value in ```create-users.yml``` file with the correct one.
3. Put the user's public key to ```roles/ssh/files/<username.pub>```
3. Run the playbook.

```ansible-playbook -i inventory.yml create-users.yml```
