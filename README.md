## Build php7.1 jenkins slave
### Clone repository
```
git clone https://github.com/sinhhn/jenkins-php7.1.git
```
### Create ssh key on master instance of jenkins 
```
$ su jenkins
$ ssh-keygen
Generating public/private rsa key pair.
Enter file in which to save the key (/var/lib/jenkins/.ssh/id_rsa): authorized_keys
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in authorized_keys.
Your public key has been saved in authorized_keys.pub.
The key fingerprint is:
SHA256:ZsZZnX9M/X61tZAp3dPEntOdeIcLUdElqSHLP3vfpZA
The key's randomart image is:
+---[RSA 2048]----+
|              ++o|
|          ...o.oo|
|         ..o+o  =|
|       . oo oo=*B|
|        S  o.*oB%|
|       +    +oo+O|
|            Eo.o+|
|            ....+|
|             ...o|
+----[SHA256]-----+
```

### Copy file to image folder
```
cp /var/lib/jenkins/.ssh/authorized_keys.pub /path/to/jenkins-php7.1/authorized_keys
```