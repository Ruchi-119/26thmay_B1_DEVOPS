# 26thmay_B1_DEVOPS

##  Task1

--Launch 5 nginx webserver from port 3000-3004 with name nginx-count no(nginx-1).

docker run -d -p 3000:80  --name nginx-1 nginx

docker run -d -p 3001:80  --name nginx-2 nginx

docker run -d -p 3002:80  --name nginx-3 nginx

docker run -d -p 3003:80  --name nginx-4 nginx

docker run -d -p 3004:80  --name nginx-5 nginx

docker ps

<img src= docker_mulcont.PNG>

## task2

--Launch a alpine image conatiner and install nginx on it curl the webpage from inside the container

docker run -d -p 80:80 --name nginx-test nginx:stable-alpine

docker ps

docker ecec -it nginx-test sh

cat /etc/nginx/conf.d/default.conf   // to view the root location

cd /usr/share/nginx/html            // root location

 ls
 
 echo "Welcome to nginx" > index.html

curl localhost

<img src= curl.PNG>

