# Lab 1: Performing Reconnaissance and Probing using Common Tools
This repository compiles the different steps I took during the lab and shows the results.

## Exploring and testing with common network scanning and anaylsis tools
### Tools used:
* Wireshark - a protocol analyzer tool taht is used to capture IP traffic from different sources
![image](https://github.com/Ttokkime/Lab-1/blob/e54321585f72cc90683a5f2ad187b58444c0747f/Ping%20Test.png)


When using Wireshark, I used the tool in order to capture the ping traffic between vWorkstation and TargetWindows02 that were not port 3389. This was done by having a filter placed for my interfaces so that all the RDP trafic generated would qualify the condition of "not port 3389". After having set this filter, I started the capture and proceeded to go to the command prompt and use the ping command.
> ping 172.18.0.1




* Command prompt
* NetWitness Investigator - a tool used to categorize information on traffic
* Nessuss - a computer vulnerability scanner
* FileZilla - a protocol software tool that connects suers with FTP servers



## Conduct network probing on machines in the Virtual Security Cloud Lab (VSCL)
## Use Zenmap to do an intense scan on subnetworks
## Generate charts taht show the relationsihps between devices within the network


Below is a diagram showing the network topology of the virtual machines used in the lab

![image](https://github.com/Ttokkime/Lab-1/blob/main/Lab%201%20Topology.png)
