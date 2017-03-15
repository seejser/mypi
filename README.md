# install rasbperry pi debian
## download
[res](https://downloads.raspberrypi.org)
## tool
[res:win32diskimager](https://sourceforge.net/projects/win32diskimager/?source=typ_redirect)

## install nodejs

### download
```
 wget http://nodejs.org/dist/latest/node-v7.7.3-linux-armv7l.tar.gz
 
```
### tar
```
tar -xvf node-v7.7.3-linux-armv7l.tar.gz
```
### test
```
cd node-v7.7.3-linux-armv7l.tar.gz

./node -v
```
### add PATH
```
cd ~/


mv node-v7.7.3-linux-armv7l.tar.gz /usr/local/node


echo PATH=$PATH:/usr/local/node/bin >> ~/.bashrc


source .bashrc
```
### uninstall nodejs
```
sudo apt-get remove nodejs
```
## check set
```
uname -a
```
## root Q

### change pw
```
sudo passwd root
```
### unlock root
```
sudo passwd --unlock root
```
### Access denied
```
sudo nano /etc/ssh/sshd_config
```
### search:```^W```
```
PermitRootLogin without-password
```
update
```
PermitRootLogin yes
```
save:```^O```
