# 26thmay_B1_DEVOPS
## task1

After creating a alb go to


listener-> view/edit rules-> edit target traffic (target1-70%, target2-30%)


<img src="target.PNG">


intsall apache server in both targets


apt install apache2



for target1 webserver output 


 cd  /var/www/html
 
 
 echo "" > index.html //redirect the content of this file

 
 vim index.html
 
 
 Hii i am target1
 
 And the output is-
 
 
 <img src="target1.PNG">
 
 
 for target2 webserver output 


 cd  /var/www/html
 
 
 echo "" > index.html //redirect the content of this file

 
 vim index.html
 
 
 Hii i am target2
 
 And the output is-
 
 
 <img src="target2.PNG">
 
 
 
 
 
 
 
