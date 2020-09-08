# ansible-powerstore-example
Ansible playbooks for PowerStore demo
## Before start
Before your demo make sure to:
- set the IP and credentials of your PowerStore array in the creds.yml
- change the host, volume and snapshot details according to whatever naming convention and size makes sense for your environment
## Demo steps
The demo has been designed with the following steps in mind
- Create a host and a volume
```shell
ansible-playbook prov.yml
```
- Create a snapshot of the volume
```shell
ansible-playbook create_snap.yml
```
- Remove the snapshot
```shell
ansible-playbook remove_snap.yml
```
- Delete the host and the volume
```shell
ansible-playbook deprov.yml
```
