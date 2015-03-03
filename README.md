# Install-Ubuntu-Server

Server version
==============================
```
$ lsb_release -a
No LSB modules are available.
Distributor ID:	Ubuntu
Description:	Ubuntu 14.04.1 LTS
Release:	14.04
Codename:	trusty
```

Update Server Sources && Update apt-get
==============================
```
1,copy sources.list to /etc/apt
2,sudo apt-get update
```

Fix GPG Error
===============================
```
#W: GPG error: http://extras.ubuntu.com trusty Release: The following signatures couldn't be verified because the public key is not available: NO_PUBKEY 16126D3A3E5C1192

gpg --keyserver keyserver.ubuntu.com --recv 3E5C1192
gpg --export --armor  3E5C1192 | sudo apt-key add -
```

Install dev-tools
=================================
```
sudo apt-get install build-essential
```
