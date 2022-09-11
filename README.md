# Lab 1: Performing Reconnaissance and Probing using Common Tools

This lab will cover concepts such as:


* Network scanning and analysis tools.
* Zenmap
* Fisheye Bubble charts

<p align="center">
<img src = "https://github.com/Ttokkime/Lab-1/blob/main/Lab%201%20Topology.png" width="700" height="400">
</p>

<p align="center">
Note: This picture is a reference that shows the different virtual machines and devices that were used in the lab and the connections between them.
</p>

## Exploring and testing with common network scanning and anaylsis tools
### Tools used:
* **Wireshark**: A protocol analyzer tool that is used to capture IP traffic from different sources.
  * When using Wireshark, I used the tool in order to capture the ping traffic between vWorkstation and TargetWindows02 that were not port 3389. This was done by having a filter placed for my interfaces so that all the RDP trafic generated would qualify the condition of "not port 3389". After having set this filter, I started the capture and proceeded to go to the command prompt and use this ping command below.

```
ping 172.18.0.1
```

<img src = "https://github.com/Ttokkime/Lab-1/blob/e54321585f72cc90683a5f2ad187b58444c0747f/Ping%20Test.png" align="left" width="650" height="400">
<p align="left">
The results of the wireshark ping traffic capture are shown in this picture. The Wireshark results display, which is split into three different windows, shows all the packets that were captured along with additional details such as the frame number, source, destination, protocol, length, hex data and extra information. 
</p>

In this example, the data for frame 1 is shown with the source, destination, protocol, and length being in the top window, additional details in the middle window, and the letters of the alphabet in the bottom window. 





* **NetWitness Investigator**: A tool used to organize and categorize traffic in order to identify specific patterns.
   * By accessing the Demo Collection and reviewing the files under each name in the user account category, I was able to identify the creditcard details file that I was tasked with finding.
<p align="center">
<img src = "https://github.com/Ttokkime/Lab-1/blob/5365ed4500c399194b815bca3e232a7a47a051ea/creditcards.txt%20file%20details.png" width="700" height="400">
</p>
The above picture is a screenshot of my access to the credit card details file that was under the user account, joann.sample.


* **Nessuss**: A computer vulnerability scanner that does remote scans on network infrastructures and can perform network discoveries on a range of services and devices. 
  * By conducting basic network scans on different ip addresses, I was able to identify vulnerabilities such as the one below. 


<img src = "https://github.com/Ttokkime/Lab-1/blob/4c22609a1753aa168a7e42e312a106e3aa6a6738/Medium%20Risk.png" align = "left" width="400" height="300">



<img src = "https://github.com/Ttokkime/Lab-1/blob/ecca769d492ea7bfd69c9b35fa0d2dcdd148e4c7/vulnerability%20detail%20screen.png" width="400" height="300">


* **FileZilla**: A protocol software tool that connects severs with FTP servers.
  * By connecting the FileZilla Server application, the connection activity that was occuring at the host 172.30.0.10 can be seen in the server logs. 
<p align="center">
<img src = "https://github.com/Ttokkime/Lab-1/blob/86bae5be59adc3448180dd12c4933f096b3eecd4/FileZilla%20logs.png" width="600" height="400">
</p>



## Use Zenmap to do an intense scan on subnetworks
By conducting targeted IP subnetwork intense scans, I was able to identify what hosts were currently available on the network, the services that the individual hosts were offering, the operating systems that were in use for these services, and the different types of firewalls and filters that were used. 


* For example, a line that returns the information that a certain host is down would look like this: 
```
Nmap scan report for 172.30.0.0 [host down]
```



## Generate charts that show the relationships between devices within the network



