```
 __   __  _______  _______  __   __  ___      _______  _______  
|  |_|  ||       ||       ||  | |  ||   |    |   _   ||  _    | 
|       ||    ___||  _____||  |_|  ||   |    |  |_|  || |_|   |
|       ||   |___ | |_____ |       ||   |    |       ||       |
|       ||    ___||_____  ||       ||   |___ |       ||  _   |
| ||_|| ||   |___  _____| ||   _   ||       ||   _   || |_|   |
|_|   |_||_______||_______||__| |__||_______||__| |__||_______|
```

...our seminar/lecture repository of the networking group MeshLab @HS-Nordhausen


# Network technology (NWT) SoSe 24
Repo for the 'Network technology' seminar course in summer semester 2024

MeshLab - Networking Seminar & Material   
This repository provides sofware tools and documentation used in the Networking courses at HSN (Nordhausen - University of Applied Sciences). To create, configure, run and troubleshoot different network experiments a virtual machine (VM) based on OpenWrt Linux is used.

# SSH access

In `ssh_keys.yaml` we will collect public SSH keys from you to provide you with a virtual machine running OpenWrt and access to it via private-public key authentication. See the file on how to add your SSH key to the list.
You need to generate an SSH keypair and submit a pull request to the repository where you add your SSH key. When you submit a pull request, it will be automatically checked for syntax and semantics of the YAML file.

After your pull request has been merged, a VM will be prepared for you. This VM will be accesible through a 2-step login process:
1. Login to our stepping stone with `ssh remote@evernet.duckdns.org -p 20322 -i <path to your private key file>`
2. After you have successfully logged in to the stepping stone, just connect to your virtual machine depending with the appropriate IP (where X is 10 + your team number): `ssh root@172.20.1.X`
