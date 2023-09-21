# Installation Process of pfSense Firewall
Once you deploy the pfSense in VMWare Workstation, you will need to install the pfSense Firewall, just like any operating system.

First, you will find the Boot Menu, along with the pfSense logo. You need to continue on the boot process till you get copyright and distribution notice.

![pfSense-Firewall-Booting](https://github.com/malvika-thakur/pfSense-Firewall-Installation/assets/60217652/6ac15716-0cd1-4b9d-8228-63d22ebc4b9e)


You will get copyright and distribution notice, you need to Accept it.

![Accepting-Copyright-and-Distribution-notice](https://github.com/malvika-thakur/pfSense-Firewall-Installation/assets/60217652/d608a3db-5516-4318-bb86-9dc0dd4bfce0)


Now, you need to select the keymap during the installation process. Let’s keep it default and continue by clicking the select button.

![Keymap-for-the-pfSense-Open-Source-Firewall](https://github.com/malvika-thakur/pfSense-Firewall-Installation/assets/60217652/531a6f93-f310-4ff3-87dc-04beb5e9f728)


Now, you need to do the partitioning of the disk. Let’s keep it as Auto (UFS) and continue.

![Configuring-the-Disk-for-pfSense](https://github.com/malvika-thakur/pfSense-Firewall-Installation/assets/60217652/faf97485-1571-4340-9bed-4fa72060d231)


So, we are almost done here. It will take a few more minutes to complete the setup, obviously depends upon the system resources. Once, the installation process is completed, you will get the following screen.

Now, you need to reboot the firewall by selecting the reboot option.

![Rebooting-the-pfSense-Firewall](https://github.com/malvika-thakur/pfSense-Firewall-Installation/assets/60217652/8b4b87e7-5dd0-4c87-b24e-e7b3c83dc73f)


After clicking on the reboot button, you will find that the pfSense firewall is getting a reboot, you will get the pfSense Logo, and finally a Welcome screen the same as per the given image.

![pfSense-Welcome-Screen](https://github.com/malvika-thakur/pfSense-Firewall-Installation/assets/60217652/82c96e1b-bb87-4b37-8aaf-80722650b846)


So, in this step, we have successfully installed pfSense in VMWare. However, still you need to know a few more default configurations, so, let’s continue to the next steps.

## pfSense Firewall default configuration
As we have configured two interfaces, i.e. VMNET8 & VMNET1, so the first interface VMNET8 has DHCP enabled by default. So, our pfSense Firewall gets an IP from DHCP Pool.

If you want to access GUI/CLI from this IP address, you need to disable the packet filter. In this example, my VM gets IP address 192.168.83.129 from DHCP. So, to get CLI/GUI access, you need to enter in the shell by pressing key 8 and type the following command :

```
pfctl -d
```

![Enabling-the-Access-from-WAN-Interface-pfSense](https://github.com/malvika-thakur/pfSense-Firewall-Installation/assets/60217652/5be67958-9f09-468b-9a15-9966652a2bae)


Now, you can access Firewall CLI/GUI using IP 192.168.83.129. You could also verify it in the below screenshot.

![pfSense-GUI-login](https://github.com/malvika-thakur/pfSense-Firewall-Installation/assets/60217652/608709fc-0704-4307-8ec1-61fcfe213b70)


Note: The default `Username : admin` and `Password : pfSense`
