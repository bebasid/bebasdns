<p align="center">
  <img src="https://www.pngitem.com/pimgs/m/10-107139_confused-anime-girl-png-transparent-png.png" width="250px"><br>
  <i>I want to access R**ddit or Vimeo but am still unable to access them even with BebasID Host File / BebasDNS?</i><br><br>
  <b>That is because your internet provider is using DPI technology to enforce blocking so changing DNS or using the host file is not enough.</b><br><br>
  <i>What is DPI?</i><br><br>
  <b>Yo! Let's find out!</b>
</p>

## What is DPI?
<p align="center">
  <img src="https://media.discordapp.net/attachments/1117725697646014484/1121259982776717383/cLXczluYcjR4kkGH93X4.png?width=1080&height=222">
</p>
DPI is the acronym for <b>Deep Packet Inspection</b> which is a method to monitor and analyze internet traffic by inspecting data packets that are being sent via the computer network. DPI analyses information and content in every data packet, including header and payload, to identify the type of application, protocol, or service. 

**Still do not understand?**

Imagine if the computer network is a motorway and the data packet is the car which queuing to pay at the booth. You can see booth for payment, right? That booth is DPI Firewall because that is the final point of the car on the motorway before exiting the motorway / continuing to the next route.

Because of this queuing process, this is why car speed becomes slower (This can form an analogy to why our internet is slower during peak hours. Because the DPI Firewall within the provider side must read billion of traffic before the connection is established and within it there is a delay or traffic jam)

Every car (Traffic that you want to send with your ISP) must prove themselves that they are legitimate drivers on that motorway by paying (In this case, 'legitimate drivers' are sites that are permitted to be accessed and 'by paying' is an analogy from traffic that we send to the provider side that must be identified by the provider before they can pass)

## What is the Impact of ISP using DPI

DPI can cause internet connection to be slower and disrupt user privacy in several ways:
1. Packet inspection and stoppage: DPI can be used to inspect every packet that is being sent within the network, this consumes an enormous amount of time and resources. This can cause a delay (latency) during packet delivery, causing the internet connection to be slower.
2. Filtering and blocking: DPI can be used to enforce security policy and access limitation. It means that internet service providers (ISP), the government, or other entities that implement DPI can block or limit access to certain websites, applications, or services. This can reduce speed and limit user internet access, affecting their privacy and disrupting internet freedom.
3. Privacy monitoring: By analyzing content within the data packet, DPI can collect users' private information, for example, browsing detail, online activity, and private communication. If not properly managed, this practice can violate user privacy and endanger their data security.

In some countries, the government or ISP implementing DPI as a part of a wider monitoring program to observe or controling internet traffic. But, improper DPI usage or without clear user consent can cause privacy issues and limit user freedom to access and use the internet.

## How National DPI in Indonesia work?

Great Firewall of Indonesia works by sending an RST packet to the client (and sometimes to the server as well) if detecting that user is visiting a blocked website by looking at the header. This is why changing the DNS and such will not work if your ISP is using DPI to block the website.

The header that is being targeted to block websites by DPI are
- Host header<br>
  Host header is an identifier within the http header containing website information that we will visit and it is not encrypted so Great Firewall of Indonesia can read, spoof as destination server, and redirect the request to `http://lamanlabuh.aduankonten.id` because http website does not have a certificate like https<br>
  
  ![image](https://github.com/bebasid/KominFudge/assets/115700386/848147a7-a296-4686-a83e-52a844aeaeaf)<br> 
 
 - SNI (Server Name Indication)<br>
   SNI (Server Name Indication) is an identifier within the https header containing the website that we will visit and usually send as plaintext to be decodable. Because https is secure and encrypted, to block the https website the only way is to send an RST packet to make it inaccessible because all passing data are encrypted with an SSL certificate
   
   ![image](https://github.com/bebasid/KominFudge/assets/115700386/1e774621-2495-4434-860c-6a3d747d47e0)<br>
   ![image](https://github.com/bebasid/KominFudge/assets/115700386/f0c4c87d-e172-44f6-8102-d3996b3e3669)<br>
