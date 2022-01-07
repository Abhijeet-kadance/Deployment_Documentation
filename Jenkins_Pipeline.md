## Creating a Jenkins CI/CD Pipeline for continuous Intergration of Web app Through Github Repo ##

### For this Documentation We are focusing on First Creating a Docker container then adding the jenkins image to it and further work on it .

> Start By installing docker on your linux Machine (note: if you dont have linux machine ypu can use VM virtual Host for the same in this documentaion we have used CentOS operating system)

> Step1) Download and install docker in the OS (You can use internet to succesfully download docker and install it accordingly)

> Step2) For making this documentaion more usefull we are using putty to access the Virtual Machine through putty console so that we can learn ho to connect to host machine through ssh

> Step3) For this we have to go to the setting of the OS networking adapter and add a bridge network that would be the one with the internet connection (if you have a wifi connection then use Wireless connection adapter and if the internet connection is wired then go for Ethernet Connection)

> Step4) Add the Bridged network setting and boot into the linux system. then use the command 

        $> ip a

        //this command will show you the IP Address that we are going to use on putty to connect to the Linux server

> Step5) Go to Putty and Choose SSH over there and add the IP which we got from 'ip a' command , Port must be 22.

> Step6) Click on Open and there comes a cli asking Who wants to login

        add your linux username and password over there

        You are Logged In to the linux using ssh connection 

> Step7) Next we are going to 