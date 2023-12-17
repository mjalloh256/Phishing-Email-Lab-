<h1> Email Phising Lab </h1>



 



<h2>Introduction/Description</h2>

This is an real life  phising atempt that I found while browsing through my emails. In this lab I will do a walk through of how I confirmed that this is a malicous attempt to steal more information on me and what i did to mitigate this user from atempting something like this again. 

<br />






<h2>Languages and Utilities Used</h2>



- <b> Virus Total </b> 

- <b>  Victim Computer </b>
- <b> Mitre&ATT&CK </b>



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



## Investigation report:  <br/>

<img src="https://imgur.com/DhSMqZP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br /> 
In this window you can see the investigation report that I created for this incident.To view its contents you can click on the picture.  It contains the hostname,Username ,Time of the event, Mirtre ID, Brief discription of what happpen, evidence/artifacts and recomendations to mitigate this malicous activity. 

<br />



## Conclusion <br/>  

<br> In conclusion this overall wasn't a complex event to investigate as long as you knew the right places to look, then it was relativly easy. Exspecially since there were no links to redirect you to another domain or downloadable files on the email which made my analysis portion of this investigation realtivly quick.  What you could also take from this real life scenario is that malicious actors are getting really good at fabercating emails and posing as real compaines so you have to be really carful when clicking on emails. The email that was sent to my inbox looked like a legitiment email from Norton. It only rasied suspicion becuase I do not have any active memberships with the company which is what lead me to my investigation of the email. <br/>


