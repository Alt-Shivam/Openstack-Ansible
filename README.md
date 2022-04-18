# Openstack-Ansible
## Do you think deploying openstack-helm is a tedious task?

### Not any more!!!

## Follow these simple steps to get started :)
Clone this repo:
```bash
git clone https://github.com/Alt-Shivam/Openstack-Ansible.git
```
Go to Directory:
```bash
cd Openstack-Ansible
```
Change the host ip address in host file:
``make the changes and save the file``  
  
Step 1: generate ssh key
```bash
ssh-keygen
```
Press enter, enter .... to go ahead with default options.  
  
Step 2: Copy ssh key to host(to deploy openstack helm)
```bash
ssh-copy-id <host ip address>@<host ip address>
```
  
Step 3: Cross check the passwordless ssh to remote host.
```bash
ssh <hostname>@<HostIp>
```
  
step 4: Run ansible with cluster.yml
```bash
ansible-playbook -i hosts cluster.yml
```
  
step 5: Run ansible with Openstack-helm.yml
```bash
ansible-playbook -i hosts Openstack-helm.yml
```
  
Now you can access your Openstack cluster

