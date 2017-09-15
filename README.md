# pi-bootstrap
setup utils for new pi's i add to my house

# purpose
Every time I build a new raspberry pi I just want all the utilities on there possible
because I'm cheap and use really slow SD cards and get annoyed later when I have to install something.

# pre tasks
* Run raspi-config
* turn on sshd
* set timezone
* set hostname

# usage
```
# apt-get install ansible
# echo "localhost ansible_connection=local" >> /etc/ansible/hosts
# apt-get install git
# git clone https://github.com/juanino/pi-bootstrap.git
# cd pi-bootstrap
# ansible-playbook pi-base.yml
# ./getmodules.sh
```
# post tasks
```
# aws configure
```
