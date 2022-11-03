# FA22: CMPE-283 Sec 48 - Virtual Technologies Assignment-1 
Here are the steps detailed to execute Assignment-1 on Ubuntu VM hosted on VMWare Workstation.
# System & Prerequisites
- System Type:	x64-based PC
- Processor: 12th Gen Intel(R) Core(TM) i7-1260P (12 Cores)
- Installed Physical Memory (RAM): 16.0 GB
- Windows 11 Professional
- VMware® Workstation 16 Pro [Trial/Download](https://www.vmware.com/products/workstation-pro.html)
- Ubuntu 22 [Download](https://releases.ubuntu.com/22.10/ubuntu-22.10-live-server-amd64.iso?_ga=2.70008919.652567418.1667472597-1208328021.1667382980)
- Intel® 64 and IA-32 Architectures Software Developer Manuals - [Download](https://www.intel.com/content/www/us/en/developer/articles/technical/intel-sdm.html)
# Enabling Nested Virtualization
To enable nested virtualization for VMs running on Windows 11
- Disable the default security features on Core Isolation.
![](resources/1.Disable%20Core%20Isolation.png)
- Turn-off the following windows features. Start > Type "**Turn Windows features on**"
![](resources/2.Turn%20off%20windows%20features.png)
# Installing Ubuntu
- Before creating Ubuntu VM using VMWare Workstation, enable the following options on VM > Settings > Processors 
![](resources/3.Enable%20Intel%20VT-x.png)
- Create a VM with 4 cores(2x2 cores), 8GB RAM and 200GB HDD and install Ubuntu.
- Once the VM is booted, verify that nested VMM capabilities are available. 
![](resources/4.Verify%20nested%20VMM%20features.png)
# Initial setup and run
- Create a github repo, checkout and place the initial/draft setup files
![](resources/5.Initial_setup.png)
- Verify dmesg logs

 ![](resources/6.sudo%20dmesg.png)
# Contributors
JAYA KRISHNA THUPILI
# License  [![License: Unlicense](https://camo.githubusercontent.com/a0f44681d578ce545f4614325d26eac4036b273d21a61de5293af355cb969bac/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f6c6963656e73652d556e6c6963656e73652d626c75652e737667)](http://unlicense.org/) 
# References
- [VMWare KB 76918:  VMware workstation with hyper-v or device/credential guard enabled](https://kb.vmware.com/s/article/76918)
- [Disable Side Channel Mitigation in VMware Workstation (windowsloop.com)](https://windowsloop.com/disable-side-channel-mitigation-in-vmware/#:~:text=1%20First%2C%20open%20the%20VMware%20application.%20You%20can,re-open%20VMware%20Workstation%20to%20fully%20apply%20the%20changes.)
- [Ostechnix.com How-to-enable-nested-virtualization-in-kvm-in-linux](https://ostechnix.com/how-to-enable-nested-virtualization-in-kvm-in-linux/)
