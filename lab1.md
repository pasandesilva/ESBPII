####ESBPII Lab1 - IT13036812
###Creating Amazon EC2 instance (Windows)
####1. Log In to Amazon Web Service(AWS) console.
![login](http://i.imgur.com/BEAfHwa.png)
![AWS_Console](http://i.imgur.com/Pm55f3h.png)
####2. Create a Windows EC2 instance.
* Press launch instace button to start creating a new EC2 instance.
![Launch_Instance](http://i.imgur.com/Z4Xap5u.png)

* Choose Microsoft Windows Server 2012 R2 Base as the Amazon Machine Image(AMI).
![Windows_AMI](http://i.imgur.com/LRZPBD5.png)

* Then choose the instance type.
![Instance_Type](http://i.imgur.com/I8al6EZ.png)

* Then configure the instance details.
![Configure](http://i.imgur.com/ccj41Gr.png) 

* Then add storage.
![Add_Storage](http://i.imgur.com/x0qMvU9.png)

* Review and launch the instance. After going through tag instance and configuring security group steps press the launch button.
![Tag_Instance](http://i.imgur.com/spGxDIs.png)
![Security_Group](http://i.imgur.com/0FfQXRd.png)
![Launch](http://i.imgur.com/YskvZvt.png)

#####3. Retrieve the administrator password using key pair. 
* Select Crete New Key Pair from the dropdown list to create a new key pair. Provide a name for the key pair and press download key pair button. Save the key pair and press Launch Instances button.
![Key_Pair#1](http://i.imgur.com/dtJ3Pj8.png)
![Key_Pair#2](http://i.imgur.com/3rn8Ull.png)

* Then press view instance button in the launch status window to see the created instance.
![View_Instance](http://i.imgur.com/JyjRSXh.png)

* Press Connect button.
![Instances](http://i.imgur.com/lw2hEb7.png)

* Press Get Password button.
![Get_Password](http://i.imgur.com/cH9YKji.png)

* Browse and select the saved key pair. Then press Decrypt Password button to retrieve the administrator password.
![Browse_keypair](http://i.imgur.com/hGpoo49.png)
![Decrypt](http://i.imgur.com/JYwQQht.png)
![Password](http://i.imgur.com/QPd6z5q.png)

#####4. Connect to the Windows Instance using Remote Desktop Connection.
* Open Remote Desktop Connection App and provide the Public IP of the  Windows instance which is under the instance description.
![Remote_Desktop](http://i.imgur.com/OuMMtyh.png)

* Provide login credentials (Administrator as username and decrypted password).
![RDC_Login](http://i.imgur.com/VSVcBlF.png)

* Press yes for the security warning. Then the Windows instance is connected.
![Warning](http://i.imgur.com/goKZDjy.png)
![Connected](http://i.imgur.com/lBVOxKP.png)

#####5. Interact with the created Windows instance.
* Once the instance is created you can perform normal activities and interact normally with the Windows instance.
![windows1](http://i.imgur.com/hBwrFcO.png)
![windows2](http://i.imgur.com/GRqvPr9.png)
![windows3](http://i.imgur.com/cXzf3sE.png)
![windows4](http://i.imgur.com/kYa2aUl.png)

#####6. Terminate the instance.
* Right click on the running Windows instance. Select Instance State > Terminate.
![Terminate](http://i.imgur.com/4ol7kQR.png)

* Confirm the action. Then the instance gets terminated.
![Confirm](http://i.imgur.com/7xsITj3.png)
![Terminated](http://i.imgur.com/CZp9Tna.png)




