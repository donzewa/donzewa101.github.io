Donna's Projects



Project #1
SIEM Alerts and Results Project:


 
Azure Sentinel(SIEM) is connected to a live virtual machine, in which it is then acting as a honey pot. I was able to see live attacks (RDP Brute Force) from various places around the globe. Then I was able to use a formated PowerShell Script to find the attackers Geolocation, and datalize it into the Azure Sentintel Map. 
>
-The following 2 pictures below is the Custom Security Log Code to develop the azure sentinel VM logs and results
![customer security log code](https://github.com/user-attachments/assets/707521b9-e84a-4292-838e-8caa00c16831)

![custom security log code 2](https://github.com/user-attachments/assets/62770008-9cc2-4210-bb3a-0ce11041395f)

-The following 2 pictures are the VM event viewer setup: Which show the login patterns

![VM_event viewer](https://github.com/user-attachments/assets/8ab0a7c1-a8fb-4140-bcac-ece36004cb6c)

![VM event viewer alerts and details](https://github.com/user-attachments/assets/195bd3b9-d751-4bc6-911d-e2b46acb279e)

The folliwng 4 pictures are on the Microsoft Sentinel page of the Scheduled Alerts for login: Medium to High depeding if activity is done by authorized user or not. The pcitures show the detailed info for each schedule login. 

![1 scheduled alert and its tab info](https://github.com/user-attachments/assets/785dbc16-a64d-4de6-81ea-9815c3ded417)

![2 Schedule alerts and tab info](https://github.com/user-attachments/assets/69d21089-f0ff-4c02-ab50-10aa80f60e4c)

![3 schedule alerts and tab info](https://github.com/user-attachments/assets/c6528278-f26a-43fd-9a59-c64d2e78d248)

![4 schedule alerts and login  of me](https://github.com/user-attachments/assets/e51adbbd-909a-4117-a5ca-f4e6c2e15cbf)

The following picture shows the Medium Alert on sentinel which show the successful logins for myself

![data of medium alert](https://github.com/user-attachments/assets/bd797ee1-3a96-4a11-99d7-6f941cda15fd)

The following picture shows the High Alert, in which it detects attacks

![Data of high alert](https://github.com/user-attachments/assets/7237c98d-a8eb-46f3-9f9c-f28ad542cc50)

The following shows the Query Log Code on the Virtual Machine to set up the attacker log results

![query log](https://github.com/user-attachments/assets/4f6c2e1e-88ca-43f7-9d2b-8156bc195ee5)

The following is the results SIEM map of various place around world my Virtual Machine got attacked by.

![SEIM_map](https://github.com/user-attachments/assets/54b8aa0d-8ff4-436c-ac7f-774ce0ad2f83)


The following shows the results in the Virtual Machine of the directory of data logs and Geolocation of countries name that attacked my Virtual Machine. 

![Logs_for vv Country hackers](https://github.com/user-attachments/assets/211cd990-6f80-4075-81e0-8bcbb10b6d88)



Project #2
Active Directory Project

Basic Overview Chart

![Map of Active Directory VM users set up](https://github.com/user-attachments/assets/73c2837b-c5b4-409b-b852-d8780db77acd)

Step 1: I Downloaded and installed Oracle Virtual Box: use to run my virtual machine

![Screenshot 2024-11-09 184939](https://github.com/user-attachments/assets/8fc76784-ec5d-48b1-9f90-3032b9f7aa02)

![Screenshot 2024-11-09 185449](https://github.com/user-attachments/assets/7a2da910-3403-4e4f-8dc1-d123038c2ac2)


Step 2: I Downloaded and installed Windows 10 ISO and Server 2019 ISO: these both used to install 2 separate virtual machines.

![Screenshot 2024-11-09 185002](https://github.com/user-attachments/assets/7c9e758d-cfa4-4228-8940-4d8d612ca16e)

![Screenshot 2024-11-09 185032](https://github.com/user-attachments/assets/2dd01646-2f89-4f40-8c70-74c5346653de)

Step 3: I Createed 1st virtual machine(domain controller): house’s the active directory

![DC](https://github.com/user-attachments/assets/7ab31b4b-c4b3-4ce4-b8ee-6ed4b1fdb2a1)

Step 4: I Gave 1st virtual machine 2 separate network adapter: 1st adapter connects to outside internet, 2nd one to connect to virtual box(private network for clients).

![Screenshot 2024-11-09 185308](https://github.com/user-attachments/assets/4c9449ea-7a1a-43a4-8f26-db74d01ea372)

![Screenshot 2024-11-09 185352](https://github.com/user-attachments/assets/b3fd9816-1b29-4a91-8e96-60f0f5fc4cf6)

Step 5: I Installed Server 2019: assign IP address for internal network, external network gets automatic IP addressing. 

![Screenshot 2024-11-09 185539](https://github.com/user-attachments/assets/18e91775-c1e7-4375-8e7f-72299f2ffd02)

![Screenshot 2024-11-09 190035](https://github.com/user-attachments/assets/bd2a18db-65a2-4b97-b645-85347e62a051)

![Screenshot 2024-11-09 190120](https://github.com/user-attachments/assets/208fc3fd-af8f-4088-89c9-7ecad0f33433)

![Screenshot 2024-11-09 190153](https://github.com/user-attachments/assets/7b304703-e74f-4af3-827e-b9cc09a0730c)

![Screenshot 2024-11-09 190235](https://github.com/user-attachments/assets/943ef033-dd5b-4885-adae-cf351320e422)

![Screenshot 2024-11-09 190322](https://github.com/user-attachments/assets/d63e3563-6405-4808-a39b-83db682cc3e0)

Step 6: I named the server, installed active directory and create domain: configure NAT and routing (so client on private network can reach the domain controller) **Following shows configuring the Active directory into VM and Domain name. 

![Screenshot 2024-11-09 190400](https://github.com/user-attachments/assets/3c72f1d8-43d2-4851-ba36-667029a5f23d)

![Screenshot 2024-11-09 190437](https://github.com/user-attachments/assets/2ade12ca-4fa9-4af9-a2d9-99403d892c0b)

![Screenshot 2024-11-09 190543](https://github.com/user-attachments/assets/f5f1ea71-ec4f-4b06-b2a4-0208da9daf12)

![Screenshot 2024-11-09 190605](https://github.com/user-attachments/assets/1891220a-1081-4fac-82d0-cd64ac7fa38b)

![Screenshot 2024-11-09 190629](https://github.com/user-attachments/assets/1a6decbd-76d6-4e00-aa79-5ed6cebe210d)

The Following shows How I configured the RAS/NAT: 

![Screenshot 2024-11-09 190742](https://github.com/user-attachments/assets/da8d373d-d99a-460e-99bd-eaa4629b6196)

![Screenshot 2024-11-09 190831](https://github.com/user-attachments/assets/5d3757c3-fdfa-4e85-bbe0-aa3b8a3043bd)

![Screenshot 2024-11-09 190848](https://github.com/user-attachments/assets/26483aed-3678-4ca8-b7f2-5c3ba4034da3)

![Screenshot 2024-11-09 190931](https://github.com/user-attachments/assets/be97754e-a335-4c97-ab94-65d9522dd08d)

The following shows how my Server Dashboard: including all the roles and server groups I configured together. 

![Screenshot 2024-11-09 190909](https://github.com/user-attachments/assets/3d59adc5-d154-421a-a226-344e0167e2b6)

Step 7: I Installed DHCP on domain controller (for windows 10 to get automatic IP addressing)

![Screenshot 2024-11-09 191024](https://github.com/user-attachments/assets/e688865c-282e-4af1-9059-50de286aa032)

![Screenshot 2024-11-09 191120](https://github.com/user-attachments/assets/6d2d00a3-1d7b-41f5-bdc6-3b9667e12327)

![Screenshot 2024-11-09 191148](https://github.com/user-attachments/assets/12ce1014-c9f6-4f32-bb26-1f1eec7f3986)


![Screenshot 2024-11-09 191234](https://github.com/user-attachments/assets/6033ae6a-b2ac-4851-9e55-ef9842c45682)

Step 8: On domain controller I ran a powershell script in order to automatically create 1,000 users on active directory

The following 2 photos shows the file I used to house all the users and powershell script
![Screenshot 2024-11-09 192659](https://github.com/user-attachments/assets/93ea6785-e90c-4839-bcff-5928da1f1d05)

![Screenshot 2024-11-09 191455](https://github.com/user-attachments/assets/f36be074-9b9f-4ae7-9875-dc7f3e8ab12e)

![Screenshot 2024-11-09 191548](https://github.com/user-attachments/assets/5f448517-b237-45f6-9496-fa8cb0250b12)

![Screenshot 2024-11-09 191620](https://github.com/user-attachments/assets/097185f5-e572-4f8f-9acd-dc974c1540d6)

![Screenshot 2024-11-09 191712](https://github.com/user-attachments/assets/d9a46a85-f108-4c1d-8170-5159f47e35e3)

![Screenshot 2024-11-09 191835](https://github.com/user-attachments/assets/7b86c1bd-6bf6-44f4-ad60-160bfa8c9599)

![Screenshot 2024-11-09 192011](https://github.com/user-attachments/assets/ec94b00e-98f8-4aeb-880b-860067afab55)

Here is the Active Directory with usernames provided: 

![Screenshot 2024-11-09 192028](https://github.com/user-attachments/assets/a02e7a9b-4a26-417c-b54b-2f145e1167f2)

Step 10: I Created another virtual machine: by installing windows 10 on it. This virtual machine connected to private virtual network. I Named it client 1, joined it to the domain. And I log into it with domain account

![Screenshot 2024-11-09 192147](https://github.com/user-attachments/assets/1a84a1bd-196d-42a6-9d43-c2aec3d8b49a)

