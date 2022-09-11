# Lab 1: Performing Reconnaissance and Probing using Common Tools

This lab will cover concepts such as:


* Network scanning and analysis tools.
* Zenmap
* Fisheye Bubble charts


<p align="center">
<img src = "https://github.com/Ttokkime/Lab-1/blob/main/Lab%201%20Topology.png" width="700" height="400">
</p>
  
**Note**: This picture is a reference that shows the different virtual machines and devices that were used in the lab and the connections between them.


## Exploring and testing with common network scanning and anaylsis tools
### Tools used:
* **Wireshark**: a protocol analyzer tool that is used to capture IP traffic from different sources
   * When using Wireshark, I used the tool in order to capture the ping traffic between vWorkstation and TargetWindows02 that were not port 3389. This was done by having a filter placed for my interfaces so that all the RDP trafic generated would qualify the condition of "not port 3389". After having set this filter, I started the capture and proceeded to go to the command prompt and use this ping command below.

```
ping 172.18.0.1
```

<img src = "https://github.com/Ttokkime/Lab-1/blob/e54321585f72cc90683a5f2ad187b58444c0747f/Ping%20Test.png" align="left" width="700" height="400">
The results are shown above in this ping test picture. The Wireshark window shows all the packets that were captured along with additional details such as the arrival source, destination, protocol, length and hex data.


















* **NetWitness Investigator** - a tool used to categorize information on traffic  
<p align="center">

<img src = "https://github.com/Ttokkime/Lab-1/blob/5365ed4500c399194b815bca3e232a7a47a051ea/creditcards.txt%20file%20details.png" width="700" height="400">
</p>
  
* Nessuss - a computer vulnerability scanner




* FileZilla - a protocol software tool that connects suers with FTP servers

![image](https://github.com/Ttokkime/Lab-1/blob/86bae5be59adc3448180dd12c4933f096b3eecd4/FileZilla%20logs.png)

## Use Zenmap to do an intense scan on subnetworks
## Generate charts that show the relationships between devices within the network



