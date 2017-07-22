# Use Pytorch in Windows 10

with Bash on Ubuntu on Windows :)

0 Requirements

    - Windows 10
    - Nice PC
    

1 Install Bash on Ubuntu : 
[https://www.howtogeek.com/249966/how-to-install-and-use-the-linux-bash-shell-on-windows-10/]

read above url!

2 Install Anaconda on Bash on Ubuntu on Windows

```
wget http://repo.continuum.io/archive/Anaconda3-4.4.0-Linux-x86_64.sh

bash Anaconda3-4.4.0-Linux-x86_64.sh

```

add `export PATH="/home/{username}/anaconda3/bin:$PATH"` on `.bashrc`

3 Make conda env
```
conda create --name ml_py36 python=3.6
```

4 Change python env on terminal

```
source activate ml_py36
```



