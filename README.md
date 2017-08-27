# Instruction show to use this deployment ansible notes

Description for this mini projects using ansible.

I have built and ran this ansible project using vagrant (vm), after spin up a vm the installation step should be taken place.

## Install ansible in the vm and follow the steps


Install ansible

```
apt-get -y ansible
```

cd /home/ubuntu/

To create a role "lamp" and "webapplication", first create a directory
so this will keep the roles organised, with ansible commands, type:

```
cd ~ && mkdir roles && cd roles
```

```
ansible-galaxy init lamp
```

```
ansible-galaxy init webapplication
```


Run the ansible-playbook to install the packages and the dependencies

```
ansible-playbook ~/app.yml
```
