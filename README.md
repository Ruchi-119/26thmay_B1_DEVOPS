# 26thmay_B1_DEVOPS
### for creating a new directory in /mnt


cd /mnt

mkdir new

ls

<img src= day10a.PNG>

### after create a volume EBS and attach to ubuntu instance

fdisk -l


<img src = day10b.PNG>


### creating a partition and formating

fdisk /dev/xvdf

type p

type n

create a new partition of 500 mb

 +500M
 
 <img src = day10c.PNG>
 
 for formating
 
 mkfs.xfs /dev/xvdf1
 
<img src = day10d.PNG>

### for mounting in /mnt/new

mount /dev/xvdf1 /mnt/new

to check the mounted drive
 
 df -hT
 
 <img src =day10e.PNG>
 
 ### to install apache 
 
 apt install apache2
 
 ### to change the root directory from /var/www/html to /mnt/new
 
 copy the file 
 
  cp var/www/html /mnt/new
  
 change the root directory
  
  vi /etc/apache2/sites-enabled/000-default.conf
   
   DocumentRoot /mnt/new
   
   
 to check the root directory
 
 grep -i 'DocumentRoot' /etc/apache2/sites-available/000-default.conf
  
 <img src = day10f.PNG>
 
 
 
 

