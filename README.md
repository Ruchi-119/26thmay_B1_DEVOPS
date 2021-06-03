# 26thmay_B1_DEVOPS
#### task 1a
sudo adduser test
su - test
cd Desktop
<img src ="task1(a).PNG">


#### task 1b
mkdir welcome
sudo groupadd lnb
sudo chgrp lnb welcome/
ls -l
<img src="task1(b).PNG">


####task 1c
sudo useradd u1
sudo useradd u2
sudo useradd u3
sudo usermod -a -G lnb u1
sudo usermod -a -G lnb u2
sudo usermod -a -G lnb u3
sudo getent group lnb
<img src ="task1(c).PNG">


