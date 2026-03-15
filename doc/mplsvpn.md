# Title: MPLS VPN in a Service Provider Network

## Abstract: 
This lecture will use a network emulation software, called GNS3, to build the MPLS VPN on the provider backbone networks. We will use OSPF, ISIS, BGP, VRF (virtual routing and forward), MPLS, and LDP on Cisco IOS. We would also discuss the pros and cons of the route leaks in multi-tenants VRF networks, and illustrate the application of applying route maps for access control and  route redistribution.  All these are the fundamental networking techniques on the Internet.  We could also discuss the Inter-AS VPN if time permits.

## Preparation: 
In order to better understand the material in the lecture, it is important for students to install GNS3 on their laptop (Intel based) and study the projects used in the lecture.  

Here are the steps:
  
1. To facilitate quick download without registration then [download from GNS3.com](https://www.gns3.com/software/download), you can choose to get the version 2.56.1 installers for your platform from [GNS3 github](https://github.com/GNS3/gns3-gui/releases/tag/v2.2.56.1) directly. 

2. Install [virtualbox](https://www.virtualbox.org/wiki/Downloads) on your laptop, then download [GNS3 VM for virtualbox](https://github.com/GNS3/gns3-gui/releases/download/v2.2.56.1/GNS3.VM.VirtualBox.2.2.56.1.zip) from GNS3 github.   Attention: this only works for Intel CPUs.

3. Download a Cisco 7200 IOS image file [c7200-advipservicesk9-mz.124-24.T8.image](https://github.com/GNS3/gns3-gui/releases/download/v2.2.56.1/GNS3.VM.VirtualBox.2.2.56.1.zip) (limited available only on UMich campus - use UM VPN), and put it on your laptop folder:  ```$HOME/GNS3/images/IOS/```.  

4. Go to GNS3 UI's menu```[GNS3|Edit]->Preferences->Dynamips->Cisco IOS```, click the ```New``` button to add this image as "Run this IOS router on GNS3 VM". 

5. Download the related GNS3 router config files at [this github repo](https://github.com/UM-EECS499-251/router-config/tree/main/mplsvpn_bgpfreecore). The GNS3 project will be added in this folder before the lecture. 

![Cisco MPLS VPN in GNS3](../mplsvpn_bgpfreecore/MPLS-VPN.png)

### References: 
\[1] Cisco, [Configure a basic MPLS VPN](https://www.cisco.com/c/en/us/support/docs/multiprotocol-label-switching-mpls/mpls/13733-mpls-vpn-basic.html).
