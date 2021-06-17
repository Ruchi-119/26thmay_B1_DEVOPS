# 26thmay_B1_DEVOPS
 1  Creating a web page using apache2 to host a webpage having content as "welcome to linux"
 
 sudo apt install apache2   //on devops(m/c1)
 
 cd /var/www/html  //root directory of web server
 
 vim index.html // "insert welcome to linux"
 
 


2 installing nginx on new instance(ubuntu)

sudo apt install nginx

systemctl stop apache2

systemctl restart nginx

systemctl status nginx.service




3 for creating a proxy pass in machine 2 (ubuntu) to redirect the  traffic to tha machine1

cd /etc/nginx/sites-available

vim default

server_name 18.191.232.6;

// in location

proxy_pass http://18.118.2.179; 

systemctl restart nginx.service




 
