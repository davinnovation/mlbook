# Install Keras on Raspberry Pi 3

1. Miniconda 설치
: [http://stackoverflow.com/questions/39371772/how-to-install-anaconda-on-raspberry-pi-3-model-b]


```
wget http://repo.continuum.io/miniconda/Miniconda3-latest-Linux-armv7l.sh
sudo md5sum Miniconda3-latest-Linux-armv7l.sh
sudo /bin/bash Miniconda3-latest-Linux-armv7l.sh

sudo vim /home/pi/.bashrc
```
 change `/root/miniconda3` to `/home/pi/miniconda3` on `.bashrc`
 add `export PATH="/home/pi/miniconda3/bin:$PATH"` on `.bashrc`

2. Make conda env
: [https://conda.io/docs/using/envs.html#create-an-environment]

3. change