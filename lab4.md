#### IT13036812
### Baremetal Virtual Machine Installation

There are two options for the baremetal vm installation

1. Format the whole hard disk and install the hypervisor on top of baremetal (if you have a brand new computer with good specs this option can help you to utilize maximum CPU power). 
2. Install VMware and create a virtual machine without an OS (which acts as baremetal) and install the hypervisor on top of that.

In our case we used the second option.

###Creating the VMware virtual machine and installing Hypervisor (Esxi)

* Open VMware Workstation and Create a New Virtual Machine(VM)
![Imgur](http://i.imgur.com/fl43shq.png)
* Select the Typical option
![Imgur](http://i.imgur.com/vt6S444.png)
* Browse the iso image of the hypervisor and click Next
![Imgur](http://i.imgur.com/BX1ZGuz.png)
![Imgur](http://i.imgur.com/LYpQWkn.png)
* Provide a name for the VM and select a location to save the VM
![Imgur](http://i.imgur.com/RJSVpZ5.png)
* Give the disk size (recommended 40GB) and select the option to Store virtual disk as single file and click Next
![Imgur](http://i.imgur.com/7Y6dKZG.png)
* Review settings and click Finish
![Imgur](http://i.imgur.com/C8FWTBK.png)
* Turn on the VM (usually will be automatically on) and install the hypervisor on the VM. (You may want to click inside VM to continue. To go out of vm press Alt+Ctrl)
![Imgur](http://i.imgur.com/xYjPpI1.png)
![Imgur](http://i.imgur.com/VDLOYd9.png)
![Imgur](http://i.imgur.com/DOVYpbc.png)
![Imgur](http://i.imgur.com/mRDhCyg.png)
![Imgur](http://i.imgur.com/HFsmrRh.png)
![Imgur](http://i.imgur.com/8BCh12r.png)
![Imgur](http://i.imgur.com/ETLvBf6.png)
![Imgur](http://i.imgur.com/plGc8aQ.png)
* Reboot and the Esxi will be loaded in the VM
![Imgur](http://i.imgur.com/Rb01atM.png)
![Imgur](http://i.imgur.com/690uH0h.png)
### Connect with vSphere
* Now open the VMware vSphere Client
![Imgur](http://i.imgur.com/zFOZkKB.png)
* Provide the IP address which is displayed in the Esxi. Provide the username as 'root'. Then type the password that was provided during the Esxi installation and click login button
![Imgur](http://i.imgur.com/AAokKW9.png)
* You can choose to ignore the certificate warning and press ok for the notice
![Imgur](http://i.imgur.com/oLX8SZQ.png)
![Imgur](http://i.imgur.com/Sx07Ujr.png)
* Click on the Inventory
![Imgur](http://i.imgur.com/yao9f8P.png)
* Here you can view all the information about the Esxi 
![Imgur](http://i.imgur.com/g2unzT9.png)
* Select the summary tab
![Imgur](http://i.imgur.com/tGThnIW.png)
* Right click on the datastore and select Browse datastore
![Imgur](http://i.imgur.com/CpsAJvM.png)
* Select upload icon and choose upload file
![Imgur](http://i.imgur.com/HYaJIiM.png)
* Browse the Kali linux iso image and click open
![Imgur](http://i.imgur.com/rebPs4Z.png)
* Click OK in the operation warning and the image will be uploaded. This image will be stored in the datastore and can be used by VM's.
![Imgur](http://i.imgur.com/Q2L7MLN.png)
![Imgur](http://i.imgur.com/xaj39Nb.png)
* Right click on the IP address and select Create New Virtual Machine
![Imgur](http://i.imgur.com/DFWvIyF.png)
* Continue with the typical option (These steps are very similar to creating in VMware workstation)
![Imgur](http://i.imgur.com/lLUOfQv.png)
* Select datastore and click Next
![Imgur](http://i.imgur.com/WOpuq5E.png)
* Select Linux and click Next
![Imgur](http://i.imgur.com/zhKMGer.png)
* Select E1000 as the adapter and click Next
![Imgur](http://i.imgur.com/JQ4vvat.png)
* Provide virtual disk size as 10GB(recommended) and select Thin provison option
![Imgur](http://i.imgur.com/Tv8cQWp.png)
* Review the settings and click Finish
![Imgur](http://i.imgur.com/jKab9Xt.png)
* Then the VM will appear in awhile. Then right click on the VM and select Edit settings
![Imgur](http://i.imgur.com/n0nbGmw.png)
* Select CD/DVD 
![Imgur](http://i.imgur.com/tvsoU1Z.png)
* Select the datastore iso and browse for the Kali linux image uploaded to datastore earlier
![Imgur](http://i.imgur.com/1DoMDg4.png)
![Imgur](http://i.imgur.com/0mIGDT8.png)
* Select the following options. Make sure Datastore iso option is actively selected before clicking OK
![Imgur](http://i.imgur.com/kMkxdfz.png)
* Then power on the VM
![Imgur](http://i.imgur.com/5j7rpt1.png)
* Install Kali linux on the VM
![Imgur](http://i.imgur.com/vhHSQkt.png)
![Imgur](http://i.imgur.com/HsJbhs6.jpg)