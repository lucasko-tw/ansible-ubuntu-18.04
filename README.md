### Install Ansible

```
sudo apt-get update
sudo apt-get install software-properties-common
sudo apt-add-repository --yes --update ppa:ansible/ansible
sudo apt-get install ansible
```


### inventory

```
[webservers]
192.168.56.3  ansible_ssh_user=ubuntu ansible_sudo_pass=ubuntu
```



### Run


```
ansible-playbook -i inventory.ini    playbook.yml 
```
