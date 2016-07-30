####ESBPII Lab2 - IT13036812
###Creating Amazon EC2 instance (Linux)
####1. Log In to Amazon Web Service(AWS) console.
![login](http://i.imgur.com/BEAfHwa.png)
![AWS_Console](http://i.imgur.com/Pm55f3h.png)
####2. Create a Windows EC2 instance.
* Press launch instace button to start creating a new EC2 instance.
![Launch_Instance](http://i.imgur.com/Z4Xap5u.png)

* Choose Amazon Linux AMI or Red Hat Enterprise Linux 7.2 as the Amazon Machine Image(AMI). Here Amazon Linux AMI was chosen.
![Choose_AMI](http://i.imgur.com/2w173F2.png)

* Then choose the instance type.
![Instance_Type](http://i.imgur.com/I8al6EZ.png)

* Then configure the instance details.
![Configure](http://i.imgur.com/ccj41Gr.png) 

* Then add storage.
![Add_Storage](http://i.imgur.com/qhPzHer.png)

* Review and launch the instance. After going through tag instance and configuring security group steps press the launch button.
![Tag_Instance](http://i.imgur.com/spGxDIs.png)
![Security_Group](http://i.imgur.com/lf5pkar.png)
![Launch](http://i.imgur.com/Ulbjgfm.png)

#####3. Convert a PEM key to a PPK key  
* For this lab we used Putty application to connect with the linux instance.

* Select Crete New Key Pair from the dropdown list to create a new key pair. Provide a name for the key pair and press download key pair button. Save the key pair and press Launch Instances button.
![Key_Pair#1](http://i.imgur.com/ynejqri.png)
![Key_Pair#2](http://i.imgur.com/pzcDa3t.png)

* Then press view instance button in the launch status window to see the created instance.
![View_Instance](http://i.imgur.com/JyjRSXh.png)
![Instances](http://i.imgur.com/lw2hEb7.png)

* To convert the downloaded key pair to .ppk open Putty_Generator.exe
![Putty_Gen](http://i.imgur.com/9XtnLvN.png)

* Press Load button and select the key pair(.pem file) and press Open.
![Load_key](http://i.imgur.com/eZU1EHS.png)
![Imported](http://i.imgur.com/a6Gr2QN.png)

* After successfully importing the .pem key file save it as .ppk file. Make sure key type is selected as SSH-2 RSA and save it as private key.
![Save](http://i.imgur.com/OpQT4mL.png)
![Save2](http://i.imgur.com/SnTNwMo.png)

#####4.Connect to a remote shell using an SSH connection 

* Then open Putty.exe. Provide the IP address in the description of the instance running.
![putty1](http://i.imgur.com/hZPJYm9.png)

* Then from the left side menu select SSH > Auth. Set the neccessary options for SSH authentication. Then browse and select the key saved in .ppk format.
![putty2](http://i.imgur.com/urO34sR.png)

* Press open and select Yes in the security alert window.
![putty3](http://i.imgur.com/EtZjLVB.png)
![putty4](http://i.imgur.com/cui9bI5.png)

* Log in as: ec2-user. This is the default user login for the AWS services. Then you will be logged into the LInux console.
![putty5](http://i.imgur.com/g0yV2VT.png)
![putty6](http://i.imgur.com/qN7xc3p.png)

#####5. Interact with the created instance
* Type 'sudo yum update' to update to latest packages. Download size will be displayed. Confirm download by pressing 'y'.
![putty7](http://i.imgur.com/t5TEEDe.png)
![putty8](http://i.imgur.com/eFixYfv.png)

* Once completed you can use the console to interact with the linux normally.
![putty9](http://i.imgur.com/XG19Onq.png)
![putty10](http://i.imgur.com/urGrPwA.png)

#####6. Terminate the instance.
* Right click on the running Linux instance. Select Instance State > Terminate.
![Terminate](http://i.imgur.com/4ol7kQR.png)

* Confirm the action. Then the instance gets terminated.
![Confirm](http://i.imgur.com/7xsITj3.png)
![Terminated](http://i.imgur.com/CZp9Tna.png)



