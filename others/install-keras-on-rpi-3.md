# Install Keras on Raspberry Pi 3

by davinnovation

1  Miniconda 설치
: [http://stackoverflow.com/questions/39371772/how-to-install-anaconda-on-raspberry-pi-3-model-b]


```
wget http://repo.continuum.io/miniconda/Miniconda3-latest-Linux-armv7l.sh
sudo md5sum Miniconda3-latest-Linux-armv7l.sh
sudo /bin/bash Miniconda3-latest-Linux-armv7l.sh

sudo vim /home/pi/.bashrc
```
 change `/root/miniconda3` to `/home/pi/miniconda3` on `.bashrc`
 add `export PATH="/home/pi/miniconda3/bin:$PATH"` on `.bashrc`

2 Make conda env
: [https://conda.io/docs/using/envs.html#create-an-environment]


```
conda create --name ml_py34 python=3.4
```



3 change python env on terminal


```
source activate ml_py34
```

4 install requirement packages


```
pip install numpy
pip install scipy ( if not works conda install )
pip install pillow
pip install h5py
```

5 install tensorflow : [https://github.com/samjabrahams/tensorflow-on-raspberry-pi]


```
wget https://github.com/samjabrahams/tensorflow-on-raspberry-pi/releases/download/v1.1.0/tensorflow-1.1.0-cp34-cp34m-linux_armv7l.whl
sudo pip install tensorflow-1.1.0-cp34-cp34m-linux_armv7l.whl

sudo pip uninstall mock
sudo pip install mock
```

6 install keras : [http://www.pyimagesearch.com/2016/11/14/installing-keras-with-tensorflow-backend/]


```
pip install keras
```


7 change keras backend

change backend `theano` to `tensorflow` at `~/.keras/keras.json` 

8 test
open python.
import keras
nailed it