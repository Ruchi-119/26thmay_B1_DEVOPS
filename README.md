# 26thmay_B1_DEVOPS

## TASK 1
1.create your own docker image using alpine as a base image

vim Dockerfile

'''

FROM alpine
RUN apk update
CMD ["echo","hello world","date" ,"ls" ,"pwd", "cal", "whoami"]

''''

press ESC--> :wq!  // to save file

##  TASK 2

2 DEfault cmd that need to run

<img src = alpine_dockerfile.PNG>

