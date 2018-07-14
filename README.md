# Linux Configuration

This repository includes the description about how I deploy [this project](https://github.com/michaella21/blog_hosting) on linux server (amazon EC2). The details of this project can be read it [here](https://github.com/michaella21/blog_hosting). To deploy it, I installed apache webserver/python 2.7/flask framework/sqlalchemy. `grader` user is creagted as a sudoer and, `grader` can log in with the provided ssh key. Also, password authentification is deabled so that `grader` must use ssh key to log in as 
```
ssh -p 2200 -i ~/ec2/id_rsa grader@ec2-18-219-50-167.us-east-2.compute.amazonaws.com
```

The security group instance was made to allow connections for SSH (port 2200), HTTP (port 80), and NTP (port 123).
- IP address: 18.219.50.167
- URL: http://ec2-18-219-50-167.us-east-2.compute.amazonaws.com/
