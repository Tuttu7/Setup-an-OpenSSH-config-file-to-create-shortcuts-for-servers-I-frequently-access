#### You can avoid typing all of the ssh command parameters while logging into a remote machine and/or for executing commands on a remote machine. All you have to do is create an ssh config file. Open the Terminal application and create your config file by typing the following command :

````
vi ~/.ssh/config
Host webserver
     HostName 52.66.208.25
     User ec2-user
     Port 22
     IdentityFile /root/testvm.pem
````
#### To open your new SSH session to webserver by typing the following command :
```
[root@ip-172-31-36-156 ~]# ssh webserver

       __|  __|_  )
       _|  (     /   Amazon Linux 2 AMI
      ___|\___|___|

https://aws.amazon.com/amazon-linux-2/
5 package(s) needed for security, out of 13 available
Run "sudo yum update" to apply all updates.
[ec2-user@ip-172-31-42-182 ~]$ 
```
