####ESBPII Lab3 - IT13036812
###Creating Amazon RDS instance (MySQL)
####1. Log In to Amazon Web Service(AWS) console.
![login](http://i.imgur.com/BEAfHwa.png)

####2. Create RDS instance.
* Select RDS from the Database section in the console.
![AWS_Console](http://i.imgur.com/Pm55f3h.png)

* Select Subnet Groups from the RDS dashboard.
![1](http://i.imgur.com/zX8iy53.png)

* Give a name and a description for the subnet group and select VPC ID from the dropdown list. 
![2](http://i.imgur.com/0kgPinT.png)

* Select Availability Zone, Subnet ID from dropdown list and press Add. If a 2b zone selected three subnet ids will be added and you may remove the last id. After that press Create button.
![3](http://i.imgur.com/P3fGW70.png)

* Then you can see the created subnet group.
![4](http://i.imgur.com/V2RiQUB.png)

* Then select RDS dashboard again and click Get Started Now button.
![5](http://i.imgur.com/yL6Rmpc.png)

*  Step 1. Select MySQL as the engine.
![6](http://i.imgur.com/1dIdi1D.png)

*  Step 2. Select MySQL from Dev/Test (Free tier eligible option) and click next step.
![7](http://i.imgur.com/UTxD4lo.png)

*  Step 3. Specify DB Details. Select DB instance class as db.t2.micro (free tier eligible)
![8new](http://i.imgur.com/cpYcpGy.png)

*   In the settings section provide a db identifier, a master username and a password. Remember these as they will be used to connect to the db instance later. Then go to the next step.
![9](http://i.imgur.com/JWfSvSP.png)

* Step 4. Configure advanced settings. Select the subnet group you created. Then select the availability zone. Provide a database name in the database. Set backup period to 0 if you prefer the free option. Then click Launch DB instance button.
![10](http://i.imgur.com/Jw51fE7.png)

* You can view the created instance by clicking View Your DB Instances button.
![10.2](http://i.imgur.com/o7tHjjs.png)
![11](http://i.imgur.com/oqRHr53.png)
![12](http://i.imgur.com/Fb5UzLr.png)
![13](http://i.imgur.com/Bkaqv9O.png)

####3. Connecting to RDS.
* You will need MySQL workbench installed on your computer in order to interact with the created MySQL db instance.
![14](http://i.imgur.com/efGkNG9.png)

* Open the command prompt and change the path to workbench installation location (alternately you can add mysql to environment variables so that mysql can be accessed from anywhere in the command line).
![15](http://i.imgur.com/lUchLtK.png)

* Type the following command at a command prompt on a client computer to connect to a database on a MySQL DB instance using the MySQL monitor. Substitute the DNS name for your DB instance for <endpoint>, the master user name you used for <mymasteruser>, and the master password you used for <password>.
   
* PROMPT> mysql -h <endpoint> -P 3306 -u <mymasteruser> -p
*** Do not  forget to remove the :3306 from the endpoint at the end. Then enter your password and press enter.
![16](http://i.imgur.com/JXEhULH.png)

####4. Interacting with MySQL instance.
* Then you will be connected with the RDS instance and you can interact normally with the MySQL db instance.
![17](http://i.imgur.com/11S1Jk8.png)
![18](http://i.imgur.com/kCDzdrK.png)

####5. Delete the db instance.
* Right click on the instance and select Delete. If you choose not to use the db instance anymore you can select No in 'Create final snapshot'. Tick acknowledge and click delete.
![19](http://i.imgur.com/jju9sPq.png)
![20](http://i.imgur.com/Z8qoPEJ.png)