Now please run below commands: 
```sh
vagrant up
vagrant ssh
```
Ones you are in the machine connected to mysql: connect to mysql and provide below credentials~~ 
```sh
user: root
password: Passw0rd!
```
Somewhere in /etc/sudoers (or /etc/sudoers.d if it's included) you have to have
```sh
vagrant ALL=(ALL) NOPASSWD:ALL
Defaults:vagrant !requiretty
```
without that, the vagrant ssh (without tty) fails mysteriously. 
