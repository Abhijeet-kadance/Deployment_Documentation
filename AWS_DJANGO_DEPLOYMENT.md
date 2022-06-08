### AWS DEPLOYMENT (DJANGO APPLICATION) ###

**Must Follw some steps to create a AWS account and create an EC2 Instance for AWS Ubuntu Server**

***Log On to an AWS Account that you have created and that may require some Payment details too. Dont worry you can allways cancel the subscription***

***You must choose the plan from a free tier itself***
    
     1. Once done doing all the Required things you can get access to EC2 instance.

     2. SSH the AWS EC2 instance on local machine using putty or git bash or any other CLI.

     3. Once you got access to AWS thats it. we can move forward to next step.

***Note: When creating EC2 Instance you have a .pem file that has to be used to access EC2 Instance. DO NOT LOSE THIS .pem***

***Note: You must remember to add permission to .pem file in case you dont have***

     $ chmod 400 test.pem

### SSH to th AWS EC2 Client ###

     $  ssh -i "test.pem" ubuntu@ec2-54-221-4*-*.compute-1.amazonaws.com

     The authenticity of host 'ubuntu@ec2-54-221-4*-*.compute-1.amazonaws.com (54.221.4*.*)' can't be established.
     ED25519 key fingerprint is SHA256:AsNdH24ruj6jEHBTzAV0OgjxsFvLCQAKaqfHGBP6puI.
     This key is not known by any other names
     Are you sure you want to continue connecting (yes/no/[fingerprint])? y
     Please type 'yes', 'no' or the fingerprint: yes
     Warning: Permanently added 'ec2-54-221-4*-*.compute-1.amazonaws.com' (ED25519) to the list of known hosts.
     Welcome to Ubuntu 20.04.3 LTS (GNU/Linux 5.11.0-1022-aws x86_64)

     * Documentation:  https://help.ubuntu.com
     * Management:     https://landscape.canonical.com
     * Support:        https://ubuntu.com/advantage

     System information as of Sun Dec 26 15:59:49 UTC 2021

     System load:  0.08              Processes:             99
     Usage of /:   18.4% of 7.69GB   Users logged in:       0
     Memory usage: 21%               IPv4 address for eth0: 172.31.94.9
     Swap usage:   0%

     1 update can be applied immediately.
     To see these additional updates run: apt list --upgradable


     The list of available updates is more than a week old.
     To check for new updates run: sudo apt update


     The programs included with the Ubuntu system are free software;
     the exact distribution terms for each program are described in the
     individual files in /usr/share/doc/*/copyright.

     Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
     applicable law.

     To run a command as administrator (user "root"), use "sudo <command>".
     See "man sudo_root" for details.

     ubuntu@ip-172-**-**-*:~$ ls

### Lets do some Basic Ubuntu Changes to get our Instacne ready for working ###

     ubuntu@ip-172-31-94-9:~$ sudo apt-get update

     // Lets upgrade our system

     ubuntu@ip-172-31-94-9:~$ sudo apt-get upgrade -y

---

