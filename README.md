# pi-bootstrap
setup utils for new pi's i add to my house

# purpose
Everyone I build a new raspberry pi I just want all the utilities on there possible
because I'm cheap and use really slow SD cards and get annoyed later when I have to install something.

# usage
```
# apt-get install anisble
# echo "localhost ansible_connection=local" >> /etc/ansible/hosts
# ansible-playbook pi-base.yml
```
