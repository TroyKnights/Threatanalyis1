<h1>Wireshark Threat analysis/h1>


<h2>Description</h2>
This project uses Kali Linux Tools along with wireshark to exploit a "Troll" test virtual machine and gain root access to retreive a file. 
<br />


<h2>Languages and Utilities Used</h2>

- <b>Virus Total</b>
- <b>Wireshark</b>

<h2>Environments Used </h2>

- <b>Windows 11</b>
  

<h2>Project walk-through:</h2>

<p align="center">
1. Where did the user contract the virus from?<br/>
  <br/> [Full request URI: http://puskovayaustanovka.ru/pusk.exe]<br/>
  <br/><br/>
<img src="https://i.imgur.com/TQomRCw.png" height="80%" width="80%" alt="Threatanalysis1"/>
  <br />
  <img src="https://i.imgur.com/LQfGSPU.png" height="80%" width="80%" alt="Threatanalysis1"/>
  <br />
  <img src="https://i.imgur.com/jEZ6zen.png" height="80%" width="80%" alt="Threatanalysis1"/>
  <br />
  <img src="https://i.imgur.com/2NufhGV.png" height="80%" width="80%" alt="Threatanalysis1"/>
<br />
<br />
2. Identify Malware if possible <br/>
  <br/>Malware Identified by VirusTotal.com<br/>
  <br />
<img src="https://i.imgur.com/EeUxUYj.png" height="80%" width="80%" alt="Threatanalysis1"/>
<br />
<br />
3. What kind of calls to the internet does it make?  <br/>
  <br/>Tried to connect to these websites below using DNS name resolution<br/>
  <br/><br/>
<img src="https://i.imgur.com/1ySRi7E.png" height="80%" width="80%" alt="Threatanalysis1"/>
  <br/><br/>
  <br/>Finally made a connection to these websites below<br/>
  <br/><br/>
  <img src="https://i.imgur.com/shdMZON.png" height="80%" width="80%" alt="Threatanalysis1"/>
<br />
<br />
4. Does it try to self-propogate through the internal network?<br/>
  <br/><br/>
  <br/>Did not find any propogation through the internal network. Internal Ip unreachable during the attack<br/>
  <br/><br/>
<img src="https://i.imgur.com/Ch76AVa.png" height="80%" width="80%" alt="Threatanalysis1"/>
<br />
<br />
5.Possible Network traffic signatures?<br/>
  <br/><br/>
  <br/>Based on the analysis there was alot of DNS requests and TCP connection attempts<br/>
<img src="https://i.imgur.com/K9W2tbM.png" height="80%" width="80%" alt="Threatanalysis1"/>
  <br />
  <img src="https://i.imgur.com/Pw35cge.png" height="80%" width="80%" alt="Threatanalysis1"/>
<br />
<br />
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
