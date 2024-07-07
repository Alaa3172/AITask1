# AI Task 1
## Download VirtualBox
VirtualBox is a powerful, open-source virtualization software developed by Oracle. It allows you to create and run multiple virtual machines (VMs) on a single physical computer. Each VM behaves like a complete computer system, with its own operating system (such as Windows, Linux, or macOS) and applications, running independently from the host system where VirtualBox itself is installed.

VirtualBox has certain minimum requirements for the host system (the physical computer where VirtualBox is installed).

### Real Use Minimum Requirements
1. X86 64-Bit Processor
2. 4 Gigabytes of RAM (The Windows host you are currently using will be using about 2 gigabytes which leaves two gigabytes for VirtualBox. If you have less than that, it's not recommended to install it. The virtual machine may run but it will be quite slow.
3. 300 Megabytes for VirtualBox 
4. 25 Gigabytes for Each Virtual Machine

### Installation Steps
1. Open your browser and paste this [link](https://www.virtualbox.org/wiki/Downloads).
2. Click Windows Hosts to download the software.
3. Close your browser and open your downloaded files.
4. Click on this file "VirtualBox-7.0.18-162988-Win" to start the installation process for the VirtualBox application.
5. Progress throught the first welcome screen by pressing next.
6. Press next on the next screen as it isnt recommended to change the various components VirtualBox intends to install.
7. Ignore the warning about the possible temporary disruption to the network and press yes.
8. Now, it has detected that there is a missing dependency which is the Python language core modules that it needs. Press next to include it in the installation components.
9. Press install to begin installation.
10. Once it finishes installing, press finish to start the application. 

## Download Ubuntu 20.04
Ubuntu is widely used both for personal computing and in enterprise environments due to its stability, security, ease of use, and extensive software ecosystem. It has become one of the most popular Linux distributions globally, attracting a diverse user base from beginners to experienced developers and system administrators.

### System Requirements
1. Windows 10
2. 4+ GB of RAM
3. 25 GB Free Disk Space
4. VirtualBox
5. Ubuntu 20.04 ISO

### Installation Steps
1. Open your browser and paste this [link](https://releases.ubuntu.com/20.04/).
2. Click on Desktop Image to download the ISO file.
3. Open the VirtualBox application.
4. Click new.
5. A window will pop up. Provide a name for your new machine (ex. Ubuntu).
6. In the ISO image section, click the drop down arrow and click on "C:\Users\aalka\Downloads\ubuntu-20.04.6-desktop-amd64.iso"
7. Check the box that says Skip Unattended Installation then click next.
8. Specify how much of the host machine's memory and processors the virtual machine can use. For good performance it's recommended to provide your VM with around 8 gigabytes of RAM although four gigabytes will still be usable.
9. Provide 4 CPU value or higher then click next.
10. Specify the size of the hard disk for the virtual machine (for Ubuntu recommend around 25 gigabytes as a minimum) then click next to continue.
11. Click finish to initialize the machine.
12. Select the created virtual machine and click start to launch the machine.
13. A message saying powering the VM up will appear and tne desktop window will appear; select install Ubuntu.
14. Click install Ubuntu again.
15. Select your keyboard layout then click continue in the bottom right corner of the page.
16. In the updates and other software section, check Normal Installation and click continue.
17. In installation type, check Erase disk and install Ubuntu then click install now.
18. Click continue and choose your current location then click continue.
19. Set up your profile (enter your name, computer name, username, and password) then click continue.
20. After the installtion ends, restart it and login with your username and password. The Ubuntu desktop has been installed.

### Fix Window Resolution
Notice that the resolution of the window is fixed at 800 by 600. This is because the guest additions features are not installed. To install that:

1. Open terminal
2. Run this command "sudo apt update".
3. Enter your password.
4. Run this command "sudo apt install build-essential dkms linux-headers-$(uname -r)".
5. Click yes or Y to continue.
6. Close the terminal.
7. Click devices from Virtual Machine menu.
8. Select insert guest Edition CD image.
9. Click the CD image in the taskbar on the left.
10. If a window pops up, autorun isn't working.
11. Right click mouse and select Open in terminal.
12. Type "./autorun.sh" then enter your password.
13. After installation, close the terminal.

Now you will get full screen when you are maximizing the machine window.
    
## Install ROS 1
ROS, short for Robot Operating System, is an open-source middleware framework specifically designed for robotics applications. It provides a collection of tools, libraries, and conventions that aim to simplify the development of complex and robust robotic systems.

### Installation Steps
1. Open your browser and paste this [link](http://wiki.ros.org/ROS/Installation).
2. Select ROS Noetic Ninjemys.
3. Select your platform which is Ubuntu.
4. Open your Ubuntu virtual machine and open terminal.
5. Follow the instructions on the browser page and paste the commands in the terminal.

To see if ROS has been installed correctly:
1. Type roscore in the terminal and hit enter.
2. A message will pop up letting you know if it was done correctly.
