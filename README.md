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

<h3>3. Download and install pyLoad</h3>

```shell script
wget https://github.com/pyload/pyload/releases/download/v0.4.20/pyload-cli_0.4.20_all.deb
sudo dpkg -i pyload-cli_0.4.20_all.deb
```

<h3>You can restart configuration over cli with:</h3>

```shell script
sudo python /usr/share/pyload/pyLoadCore.py -s
```
