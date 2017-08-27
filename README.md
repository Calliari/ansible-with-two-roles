# Instruction show to use this deployment ansible notes

Description for this mini projects using ansible.

I have built and ran this ansible project using vagrant (vm), after spin up a vm the installation step should be taken place.

## Install ansible in the vm and follow the steps


Install ansible

```
apt-get -y ansible
```

cd /home/ubuntu/

To create a role "lamp" and "webapplication", first create two directories
so this will keep the roles organised, with ansible commands, type:

create the directory called "roles"
```
cd ~ && mkdir roles && cd roles
```

create a files infrastructure for "lamp" role with this commands
```
ansible-galaxy init lamp
```

create a files infrastructure for "webapplication" role with this commands
```
ansible-galaxy init webapplication
```


Run the ansible-playbook to install the packages and the dependencies defines;
The "app.yml" has the configuration for pointing to what the two rode ness to install...

```
ansible-playbook ~/app.yml
```
<hr>

The "app.yml" has the "lamp" directory which contains the defaults file with the main.yml, this main.yml has the config wit for "lamp" role, as such the same happens with the webapplication role.
