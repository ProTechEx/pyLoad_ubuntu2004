# How to install pyLoad under Ubuntu 20.04

<h3> 1. Adding Key Server </h3>

```shell script
gpg --keyserver keyserver.ubuntu.com --recv-keys 16126D3A3E5C1192
gpg --keyserver hkp://subkeys.pgp.net --recv-keys 16126D3A3E5C1192
```


<h3>2. Installaing packeges and dependencies</h3>

```shell script
sudo add-apt-repository ppa:launchpad/ppa && sudo apt-get update
apt-get install -y python python-crypto python3-pycurl python-openssl tesseract-ocr libmozjs-68-0 libmozjs-68-dev
sudo apt-get install -f
```
