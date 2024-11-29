<h1>Network Packet analyzer using Wireshark Lab</h1>



<h2>Description</h2>
Welcome!
In this lab, we're gonna go through a Wireshark Packet capture lab from Security Blue Team. This a great introduction for beginners to understand how wireshark can used and how to navigate the different tools and techniques on the wireshark environment. This will also be good practice to develop networking skills for those who are tyring to adopt a blue team mindset for investigation and incident response. Even for IT professionals, it will be good practice to go over this tool and utilize the information on hand. Let's get started... 
<br />


<h2> Utilities Used</h2>

- <b>Wireshark</b> 

<h2>Environments Used </h2>

- <b>Windows 11</b> (21H2)
- <b>Blue Team Labs: Security Blue Team</b>
<h2>Program walk-through:</h2>

<h2> Packet Capture 1</h2>
<p align="center">
 1. Find which protocol was used over port 3942?<br>
  
- <b>Navigate to statistics > Endpoints > UDP </b>
- <b>Right-click to port 3942, Apply as a filter > Selected </b>
 
![image alt](https://github.com/Light89byte/NetworkAnalyzer/blob/deee934d71c61b102c6d8f56aba053a3108301e9/port%203942.png)
<br />
<br />

- <b>The protocol is SSDP.

![image alt](https://i.imgur.com/ylzf5nN.png)
<br />
<br />

<p align="center">
What is the IP address of the host that was pinged twice?<br>
  
- <b>8.8.4.4</b>
  
![image_alt](https://i.imgur.com/0tKLFmM.png)
<br />
<br />

<p align="center">
How many DNS query response packets were captured?<br>
  
- <b>Type "Dns" in the filter bar.</b>
- <b> Click "Standard query Response"</b>
- <b>In the bottom left corner, go to domain name system and then flags. After which, right-click "response:message..." Apply as filter> selected </b>
- <b>In the bottom right corner, you'll see 90 packets were captured</b>

![image_alt](https://i.imgur.com/sJTDYOM.png)
<br />
<br />

<p align="center">
What is the IP address of the host which sent the most number of bytes?<br>

- <b>Stats > Endpoints > IPv4</b>
- <b>Click on Tx bytes. The IP address is "115.178.9.18"</b>

![image alt](https://i.imgur.com/6LlTKzo.png)
<br />
<br />

<p align="center">
 

<br />
<br />
