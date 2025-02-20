# 42_born2beroot

## Purpose

> The Born2beRoot project aims to teach the participant core system administration and virtualization skills. It challenges them to configure a secure server within a virtual machine using only the command line, selecting an operating system like Debian—known for stability and APT package management—or Rocky Linux, with its DNF and SELinux features. The participant secures it with SSH for encrypted access, UFW for firewall management, and sudo for privilege control, gaining practical experience in server management and key concepts like LVM and AppArmor, preparing them for real-world administration tasks.

## Overview of What I Did and Learned  

1. **Virtualization**  
I started by setting up a virtual machine with VirtualBox and installed Debian without a graphical interface. It was my first time working entirely in the terminal, and I learned that a virtual machine acts like a separate computer, running on my host system’s resources but staying isolated, which is great for testing safely.

2. **Operating System Configuration**  
I configured Debian by setting a hostname, creating a user with my login, and organizing partitions with LVM. Using commands like `lsblk` to check my setup was eye-opening. I learned how LVM makes storage management more flexible compared to traditional methods, which feels powerful for future projects.

3. **Security Practices**  
I secured my server by setting up UFW to only allow traffic on port 4242, confirmed with `sudo ufw status`, and configured SSH to use that port while blocking root login, checked via `sudo service ssh status`. I also enforced a strong password policy and set up sudo logging. I learned that firewalls and SSH are critical for keeping a server safe, and sudo helps me manage admin tasks securely.

4. **System Management**  
I added myself to the sudo and user42 groups with `sudo adduser` and managed packages using `apt`. I learned how these tools keep the system running smoothly and how group assignments control access, which is key for administration.

5. **Automation**  
I wrote a script to monitor system stats and scheduled it with `cron` to run every 10 minutes, set up via `sudo crontab -u root -e`. I learned that automation with cron saves time and keeps things consistent—super useful for repetitive tasks.

6. **Core Concepts**  
This project taught me to explain tools like SSH for secure access, UFW for traffic control, LVM for storage, and sudo for privilege management. I gained a solid grasp of how they work together to make a server secure and efficient.

## Grade: 100 / 100
