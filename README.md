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
* set runlevel to 3

# usage
```
# apt-get update
# apt-get install ansible
# echo "localhost ansible_connection=local" >> /etc/ansible/hosts
# apt-get install git
# git clone https://github.com/juanino/pi-bootstrap.git
# cd pi-bootstrap
# ansible-playbook pi-base.yml
# ansible-playbook clean-svc.yml
# ./getmodules.sh
```
# post tasks
```
# aws configure
# git config --global user.email "XX@XXX.com"
```
* setup rc.local to slack ip to room
* setup /etc/waterpi.yaml for slack integration
