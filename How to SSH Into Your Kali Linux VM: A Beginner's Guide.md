#####**How to SSH Into Your Kali Linux VM: A Beginner's Guide**

###**Introduction**
Kali Linux is a popular operating system used for penetration testing and ethical hacking. Being able to SSH into a Kali Linux VM can be extremely useful for remote management, file transfer, or running commands. This guide will walk you through the steps to set up SSH access to your Kali Linux VM from your host machine.

###**Prerequisites**
**A Kali Linux Virtual Machine up and running**
**Basic understanding of Linux terminal commands**
**Basic understanding of networking concepts like IP Address, Ports, etc.**

###**Steps**

##**Step 1: Update Package Lists**
Open the terminal in your Kali Linux VM and execute the following command to update your package list:
![Image Description](https://github.com/Hackroop/jags/blob/95d9d62343b6b9f527a4f5c3ef74671ec7d9b433/1.png?raw=true)

##**Step 2: Install the OpenSSH Server Package**
Execute the following command to install the OpenSSH Server:
![Image 2 Description](https://github.com/Hackroop/jags/blob/main/2.png?raw=true)

##**Step 3: Start and Enable the SSH Service**
After installing, you need to start the SSH service. You can also enable it to start automatically upon system boot.
![Image 2 Description](https://github.com/Hackroop/jags/blob/main/2.png?raw=true)

##**Step 4: Verify SSH Service Status**
To ensure that the SSH service is running correctly, you can check its status:
![Image 4 Description](https://github.com/Hackroop/jags/blob/main/4.png?raw=true)

##** Step 5: Obtain the IP Address of Your Kali Linux VM**
To SSH into your Kali Linux VM, you'll need to know its IP address. You can find this information by running:
![Image 5 Description](https://github.com/Hackroop/jags/blob/main/5.png?raw=true)
Look for the IP address listed under your active network interface.

##**Step 6: SSH from Your Host Machine**
Now, open a terminal on your host machine and execute the following command:
![Image 6 Description](https://github.com/Hackroop/jags/blob/main/6.png?raw=true)
Replace `username` with your Kali Linux username and `KALI_VM_IP_ADDRESS` with the IP address you obtained earlier.

##**Optional: Add an SSH Key for More Security**
_SSH keys offer a more secure way of logging into a server. To generate an SSH key pair, you can use the following command on your host machine:_
![Option Image Description](https://github.com/Hackroop/jags/blob/main/option.png?raw=true)

##**Conclusion**
You have successfully set up SSH access to your Kali Linux VM. You can now manage it remotely, which can be particularly useful for various penetration testing tasks or educational purposes. Remember that while SSH is secure, it's always a good idea to keep your system and packages up-to-date for the best security practices.
