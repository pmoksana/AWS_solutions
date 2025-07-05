INSTRUCTION :
 
 Use SSH to connect to an Amazon Linux EC2 instance

 Windows Users: Using SSH to Connect

Select the Download PPK button and save the labsuser.ppk file.
Typically your browser will save it to the Downloads directory.
Make a note of the PublicIP address.
Then exit the Details panel by selecting the X.
Download  PuTTY to SSH into the Amazon EC2 instance. If you do not have PuTTY installed on your computer, download it here.

Open putty.exe

Configure your PuTTY session by following the directions in the following link: Connect to your Linux instance using PuTTY
 

macOS  and Linux  Users
These instructions are specifically for Mac/Linux users.
cd ~/Downloads
Change the permissions on the key to be read-only, by running this command:

chmod 400 labsuser.pem
Run the below command (replace <public-ip> with the PublicIP address you copied earlier).
Alternatively, return to the EC2 Console and select Instances. Check the box next to the instance you want to connect to and in the Description tab copy the IPv4 Public IP value.:

ssh -i labsuser.pem ec2-user@<public-ip>
 


 
