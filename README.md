<h1> Email Phising Lab </h1>



 



<h2>Introduction/Description</h2>

This is an real life  phising atempt that I found while browsing through my emails. In this lab I will do a walk through of how I confirmed that this is a malicous attempt to steal more information on me and what i did to mitigate this user from atempting something like this again. 

<br />






<h2>Languages and Utilities Used</h2>



- <b> Virus Total </b> 

- <b>  Victim Computer </b>



<h2>Environments Used </h2>



- <b> Virus Total  </b>
- <b> Victim Computer </b>







<h2>Program walk-through:</h2>



<p align="left">


## Malicious Email




 <img src="https://imgur.com/VHvNSYD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<br /> As shown in the malicous email there are multiple things that are off about the email. The first thing that was off was that they was claiming that I had a life lock account from the company Norton but could not state my first name and addressed me as ADMIN. Another problem with this email is that it claims is from the company Norton but if you look at the email header the email address that sent this email does not match the domain name for the company Norton and it is a random gmail account. This alone is enough to show that this is a phising email with an atempt to steal your information. Another red flag anout this email is how they are requering you to take action asap. The email was sent on Dec 11th and this was what was included in the end of the messeage. "In case you don't want to continue with us then make sure you call us on 909 907 9883 before 12/11/2023 to avoid any recurring payment" This makes it seems like you are going to get charged since you missed the due date even though the email was sent on the same day. Unfortunetly if you are an elderly person, not tech savy and aware of malcious attacks like this or maybe just a super busy or stressed indivdual, you can easily fall victim to this. After I gathered all this information it was enough to continue my investigation.
<br />



## Raw Email Messeage Syantax:  <br/>

<img src="https://imgur.com/3uxNLQb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br />  This window shows the Raw Email Messeage Syantax which gives me more information on the email itself. My main objective of opening up the raw contents of the email was to see the IP address that sent this email so I can futher confirm that this is a malicious attack. As you can see I highlighted the Ip address that was used to send this email to my account. 

<br />



 ## Virus Total Analysis :  <br/>

<img src="https://imgur.com/nGIcdWe.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<br />  As you can see in the window above. As soon as I ran the IP address into the  OSNIT tool virus total. It confirmed that the user who sent this email has a malicous IP address, meaning they have been reported by security vendors for malicous activity. I did a little deeper analysis to see if I could find out a little more history about this IP address. I found out that this IP Address is in communication with a handful of malicious files. As I futher analylzed this Ip Address futher I found out that the malicous communicating files are mostly pertaing to information gathering or stealing. Below is the virus total window where I did a futher analysis on this Ip Address. 

<img src="https://imgur.com/ijDfetd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<br />



## Vulnerblites On Mac OS:  <br/>

<img src="https://imgur.com/qes9XMK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br /> 

The specfic vulnerblites listed for the Mac OS are all potential attacks that can be executed towards the system. The way to remediate these vulnerblites would be a simple system update. The current version of Mac OS that is running on the system is 14.0 the update recommended by nessus is the Mac OS of 14.1.2 which contains security patches for the vulnerblites listed for 14.0. I later installed latest running OS for Mac.

<br />



## Vulnerblites On Mac OS for Zoom client application <br/>

<img src="https://imgur.com/3OxbcRr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<img src="https://imgur.com/IgPLdqf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>



<br /> The last vulnerblity that was found on the Mac OS was with the application zoom. The vulneriblites found by nessues include  Improper authorization in some Zoom clients may allow an authorized user to conduct an escalation of privilege via network access,Insufficient control flow management in some Zoom clients may allow an authenticated user to conduct an information disclosure via network access,Buffer overflow in some Zoom clients may allow an unauthenticated user to conduct a denial of service via network access,Improper conditions check in Zoom Team Chat for Zoom clients may allow an authenticated user to conduct a denial of service via network access and aCryptographic issues with In-Meeting Chat for soZoom clients may allow a privileged user to conduct an information disclosure via network access. These are all vulnerblites that are found with the current version of zoom found on this system 5.15.12. Nessus recommends downloading version 15.16.0 that contains the vulnerblity pataches for this application. After finding these vulnerblites on the Mac os system I downloaded the latest version of zoom client application.  

<br />



## CIA TRIAD FRAMEWORK  :  <br/>

<img src="https://imgur.com/KJuon8i.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br /> The vulnerblity assesment that I conducted on my network is a very important task that companies all around the world need to implemnt to insure their information/data security. Cyber secuirty frameworks such as the CIA Traid help us insure proper security. As I have done, the vulnerblity assesment that I conducted on my network made sure to implement this framework. Confidentiality is very big when it comes to securing your data. With the assesment that I did on my network I was able to discover vulnerblites with certain applications that leak data. Integrity is the next objective in the CIA Triad. The importance of this is to make sure that the information that an application is providing has the correct security measures so that data is not tampered with and is 100 percent authentic and can be trusted. There were also vulnerblites of this too found on my network. The last objective the CIA Triad covered on the network vulnerblity assement is avalblity. With the vulnerblity report that nessus provided some applications had vulnerblites of a dos(denial of service) attack. In conclusion the CIA TRIAD was correctly implemented in all of these applications due to updates that I installed for each api. The security vulnerblites were all mitigated for these applications which insured confidentiality, Integrity, and avalblity lity for each api on the device. 

<br /> 
