Question 1
Start your VirtualBox software. Before you click Start on your Ubuntu Graphical User Interface (GUI) desktop, at the very top of your VirtualBox bar, click “Machine”, and then click “Show Log” and a file will be displayed. Scroll up to the top of the file. You will see your desktop installation information and your desktop server name. Get a screenshot of this file and paste it in this question as proof of your system installation. 
Answer 1: 
System info on Oracle virtual box machine and followed by System logs. 

 





System Logs
 

Question 2
Explain how you would get/display an Overview information on your Linux desktop information hardware. Copy and paste the information in your answering document as proof of your work.
Answer 2:
There are plenty of commands to check information about the hardware of the Linux system. Some commands report only specific hardware components like CPU or memory while the rest cover multiple hardware units. The list includes lscpu, hwinfo, lshw, dmidecode, lspci etc.
lscpu - The lscpu command displays information about the CPU and processing units. 
lshw – List Hardware.
Lists information about different hardware units such as CPU, disk, memory, usb controllers, network adapters etc. lshw extracts the information from different /proc files.
hwinfo – Hardware information.
hwinfo is another general-purpose hardware probing utility that can display detailed and brief information about multiple different hardware components, and more than what lshw can report.
Inxi - Inxi is a 10K line mega bash script that fetches hardware details from multiple different sources and commands on the system and generates a beautiful looking report that non-technical users can read easily.

lscpu
 





lshw - lshw -short displays the hardware list in short

  










hwinfo 
  







inxi
 










Question 3
Explain how you would get/display information on your Linux desktop Network Wired information. Copy and paste the information in your answering document as proof of your work.
Answer 3: The quick way to check whether you are connected or not is to click on the right-hand side of the machine which displays wired connection information of the network being connected. Once you see that the command for finding your IP Address is ifconfig. When you issue this command, you will receive information for every network connection you have available. Most likely you will see information for both the loopback (lo) and your wired network connection (eth0). If you have a wireless connection that will be listed, most likely, as wlan0.

  



 ifconfig
 


Question 4
There are two types of users; general users and super user. Explain how do you become a super user? Demonstrate how you become a super user. When you have successfully becoming a super user, exit from it and do a screenshot on your work and submit the screenshot as proof of your activities.
Answer 4: 
To verify user identity, use the command whoami and check. If you are a general user and wants to become a super user, use the command super su or just su. The difference between the two is su command must know the root user’s password where as sudo need not know root user’s password.  And then whoami. The result displays root and the prompt changes from $ to #. To exit out of a super user click either CTRL D or use command logout or exit and become a general user again. Screenshot explains the same. 
 

Question 5
Using Microsoft Word write a summary of what you have learned in this assignment (minimum of 100 words, use your own words). Summarize your report, do not use bullet items.
Answer 5:
Homework 1 is all about installing Linux on Oracle VirtualBox. I knew how to install Linux before as I learned in the prerequisite class ITMO 556 – Intro to Open Source Software. The installation was quick and easy. Though I knew about the basic commands but had never tried to look up for hardware information. But during this assignment I could get to know different types of commands like lscpu, lshw, hwinfo and inxi. I googled to see the difference between all these. Apart from this ifconfig command was known before to find the IP address details. Becoming a super user using su or sudo su I learned the need for password in these. whoami identifies the user logged in. Also, to login as a super user one can use sudo -i. The option i tells sudo to run the shell specified by the root user’s password database entry as a login shell. If you pass -s to the sudo command, it runs the shell specified by the Shell environment variable if it exists or the shell defined by the invoking user’s password database entry.
