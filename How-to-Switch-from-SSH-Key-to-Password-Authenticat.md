# How to Switch from SSH Key to Password Authentication After Losing an SSH Key

###### 1. Go to [https://virt.crunchbits.com](https://virt.crunchbits.com) 
###### 2. [Power off your VM](https://www.notion.so/Using-the-basic-functions-of-the-server-102f2d21f0f44ac5b694603d41357ed6?pvs=21)
###### 3. [Enable VNC console](https://www.notion.so/Using-the-basic-functions-of-the-server-102f2d21f0f44ac5b694603d41357ed6?pvs=21)
###### 4. [Change the root password](https://www.notion.so/Using-the-basic-functions-of-the-server-102f2d21f0f44ac5b694603d41357ed6?pvs=21)
###### 5. Enter the VNC console
    
![46375456745645 (1).png](How%20to%20Switch%20from%20SSH%20Key%20to%20Password%20Authenticat%201324f4be317a4dc8b791e69dd84e6594/46375456745645_(1).png)
    
###### 6. Enter the recovery/emergency mode [google the following phrase to check how to: How to enter recovery mode in DISTRO]
###### 7. Log in and use the username "root" and the password that was sent to your email.
###### 8. Move to the ssh config directory [cd /etc/ssh/sshd_config.d]
###### 9. Then we need to edit the configuration file [nano cloud-init***.conf]
###### 10. Please modify the "PasswordAuthentication" setting in the configuration file by changing its value from "no" to "yes"
###### 11. Hit Ctrl+X then click Y
###### 12. Input the following command: reboot -n
###### 13. Now you can SSH into the VPS using you Password