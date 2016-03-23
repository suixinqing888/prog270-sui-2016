# SSH Commands
## Setup SSH
```
   sudo apt-get install ssh
   cd
   ssh-keygen -t rsa -P '' -f ~/.ssh/id_rsa
   cat  ~/.ssh/id_rsa.pub >> ~/.ssh/authorized_keys
   cd ~/.ssh
   cat id_rsa.pub
```
## Load SSH Key
```
mv ~/.ssh/id_rsa ~/.ssh/Prog270-Fall-2016
mv ~/.ssh/id_rsa.pub ~/.ssh/Prog270-Fall-2016.pub
ssh-add ~/.ssh/Isit320-Fall-2015
```
If this works as expected, you should see the words Identity added in the response:
```
ssh-add ~/.ssh/Prog270-Fall-2016
Identity added: /home/charliecalvert/.ssh/Prog270-Fall-2016 (rsa w/o comment)
```
## Automating the load process
```
ssh-add ~/.ssh/Prog270-Fall-2016
geany ~/.bashrc
source ~/.bashrc
cd ~/.ssh
ln -s Prog270-Fall-2016 main-key

```