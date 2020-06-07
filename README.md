# install-a-Linux-by-network
A Linux Scripts which can help you reinstall to another Distribution even Windows.

You should take your own risk to use this tools.

It's not created by me, reupload here and try to add Kali inside for my personal use.

Credit: Vicer - moeclub

# Instructions:

## 1. Install required tools on:

### a. Debian/Ubuntu:
```
apt-get update
apt-get install -y xz-utils openssl gawk file
```
### b. RedHat/CentOS:
```
yum update
yum install -y xz openssl gawk file
```
## 2. Download script
```
wget --no-check-certificate https://raw.githubusercontent.com/leonguyen52/installNET/master/InstallNET.sh && chmod -x InstallNET.sh
```
## 3. Install OS via script

### a. Linux: Default password is "root1234". Please change it after finishing installation.

Debian 7 x32:
```
bash InstallNET.sh -d 7 -v 32 -a
```
Debian 7 x64:
```
bash InstallNET.sh -d 7 -v 64 -a
```
Debian 8 x32:
```
bash InstallNET.sh -d 8 -v 32 -a
```
Debian 8 x64:
```
bash InstallNET.sh -d 8 -v 64 -a
```
Debian 9 x32:
```
bash InstallNET.sh -d 9 -v 32 -a
```
Debian 9 x64:
```
bash InstallNET.sh -d 9 -v 64 -a
```
Debian 10 x32:
```
bash InstallNET.sh -d 10 -v 32 -a
```
Debian 10 x64:
```
bash InstallNET.sh -d 10 -v 64 -a
```
Ubuntu 14.04 x32:
```
bash InstallNET.sh -u trusty -v 32 -a
```
Ubuntu 14.04 x64:
```
bash InstallNET.sh -u trusty -v 64 -a
```
Ubuntu 16.04 x32:
```
bash InstallNET.sh -u xenial -v 32 -a
```
Ubuntu 16.04 x64:
```
bash InstallNET.sh -u xenial -v 64 -a
```
Ubuntu 17.04 x32:
```
bash InstallNET.sh -u zesty -v 32 -a
```
Ubuntu 17.04 x64:
```
bash InstallNET.sh -u zesty -v 64 -a
```
Ubuntu 18.04 x32：
```
bash InstallNET.sh -u bionic -v 64 -a
```
Ubuntu 18.04 x64：
```
bash InstallNET.sh -u bionic -v 32 -a
```
CentOS 6.8 x32:
```
bash InstallNET.sh -c 6.8 -v 32 -a
```
CentOS 6.8 x64:
```
bash InstallNET.sh -c 6.8 -v 64 -a
```
CentOS 6.9 x32:
```
bash InstallNET.sh -c 6.9 -v 32 -a
```
CentOS 6.9 x64:
```
bash InstallNET.sh -c 6.9 -v 64 -a
```
CentOS 7 x32：
```
bash InstallNET.sh -c 7 -v 32 -a
```
CentOS 7 x64：
```
bash InstallNET.sh -c 7 -v 64 -a
```

### b. Windows (you will need the Windows image to install)
```
bash InstallNET.sh -dd 'link-to-vhd-image'
```

## Advance Example
```
# Automatically install using the default mirror
bash InstallNET.sh -d 8 -v 64 -a
 
# Automatically install using custom mirror
bash InstallNET.sh -c 6.9 -v 64 -a --mirror 'http://mirror.centos.org/centos'
 
 
# In the following example, replace X.X.X.X with its own network parameters.
# --ip-addr :IP Address
# --ip-gate :Gateway
# --ip-mask :Netmask
 
#Use custom mirror and custom Network Parameters
#bash InstallNET.sh -u 16.04 -v 64 -a --ip-addr x.x.x.x --ip-gate x.x.x.x --ip-mask x.x.x.x --mirror 'http://archive.ubuntu.com/ubuntu'
 
#Use the custom network parameters to install windows
#bash InstallNET.sh --ip-addr x.x.x.x --ip-gate x.x.x.x --ip-mask x.x.x.x -dd 'link-to-image-vhd'
 ```