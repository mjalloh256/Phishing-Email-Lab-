<h1> Email Phishing Lab </h1>



 



<h2>Introduction/Description</h2>

This is an real life  phishing atempt that I found while browsing through my emails. In this lab I will do a walk through of how I confirmed that this is a malicous attempt to steal more information on me and what i did to mitigate this user from atempting something like this again. 

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


















<h1> Email Phishing Lab 2 </h1>



 



<h2>Introduction/Description</h2>

This is another real life  phishing atempt that I found while browsing through my emails. In this lab I will do a walk through of how I confirmed that this is a malicous attempt to steal more information on me and what I did to mitigate this user from atempting something like this again. 

<br />






<h2>Languages and Utilities Used</h2>



- <b> Virus Total </b> 

- <b>  Victim Computer </b>
- <b> Mitre&ATT&CK </b>
- <b> ANY.RUN sandbox tool</>



<h2>Environments Used </h2>



- <b> Virus Total  </b>
- <b> Victim Computer </b>
- <b> ANY.RUN sandbox </b> 







<h2>Program walk-through:</h2>



<p align="left">


## Malicious Email




 <img src="https://imgur.com/mjgaVGG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>  

 <br/> In the first window you can see the email messeage I got in my inbox. Compared to the first email that I investiagted there are very few red flags that are left through out the email if any. The one thing that caught my attention was how the malicious actor  tried to redirect the user to whatsapp which is not a common thing established companies do which rasied futher suspision on this email. Other than that it seemed like a legit email from a travel company. <br/>
  <img src="https://imgur.com/OlK0JUz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 


<br /> The next image was the rest of the email that provided links to diffrent domains. I still was not sure if the email was malicious or not so I avoided clicking the links for my saftey. 
<br />



## Raw Email Messeage Syantax:  <br/>
  <img src="https://imgur.com/GfxEFRx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 


<br />  To futher continue my investigation I pulled up the Raw Email Messeage Syantax so I could find the IP address of the user who sent this email. I would then scan the IP address in virus total to help aid me in my investigation. 

<br />



 ## Virus Total Analysis :  <br/>

<img src="https://imgur.com/SGoy1Ec.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<br />  After I ran the IP address of the user that sent this email to me. Virus total marked this user as non malicious with 0 security vendors stating it is malicious. However I was able to see that the IP address was in communications with other files. This lead me to do a deeper analysis on virius total and investigate the communicating files within this IP address.

<img src="https://imgur.com/t7KYIsz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

As I continued my investigation with the communicating files for that IP address I found out that 2 of the 13 files this IP address was communicating with were marked as malicious which rasied even futher suspicion. The first file had a score of 1/60 security vendors makrking the file as malicious and the second file had a score of 1/59 security vendors marking it as malicious.Even though the IP address was not marked for malicious activity that didnt mean it was totally clean. 


<br />



## Sandbox analysis/report <br/>

<img src="https://imgur.com/vSONIYg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br /> As my suspicions of this email being malicious increased. I decided that the best course of action was a sandbox analysis. I took the links that were attachted to the email and ran a sandbox analysis on it to see any process,executions or downloadable files that could possably appear if an actual user was to click on the link. The sandbox analysis would also allow me to see if there were any threats to a user who clicks on one of these links. 


<br />



## Sandbox analysis/report 2  <br/>  
<img src="https://imgur.com/Z7K05AK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br> As I continuned my investigation you can see that there are a total of 20 connections to that redirected link that was presented in the email that I recevied. You have IP addresses from Belgium,Germany and the United States all connecting with that domain. The next course of action that I did was scan these IP address to confirm if they were malicous or not.   <br/>
<img src="https://imgur.com/rf2w71F.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
<img src="https://imgur.com/ebDzbXB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>  

<br> After just scanning the first 3 IP addresses I could confrim that those address were malicious or was communicating with malicious files. In conclusion all 20 of the IP addresses that were in connection with the redirected link from the email were all malicious or in communication with malicous files. Above is one example of one of the malicous IP address that was in communication with this link. In the second window you can see communicating files that is assosiated with this IP address. The total number of files is about 1 Million. And about 90 percent of those files are malicous.  <br/>
## Sandbox analysis/report 3 <br/>  

<img src="https://imgur.com/2UveA2z.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
<b> For the last portion of my sandbox analysis on this email I was able to see the threat that would be exposed to a user if they were to click this link. The picture above shows this. The threat was marked as malicous by ANY.RUN the sandbox tool. The data was  from a Suricata IDS. The threat was URL shortening. The main reason a malicious actor would shorten a URL link would be to hide the exact location a URL would take a user. The main reason would be becuase it is a malicous domain that can contain malware, dangerous downloadable files, virius or more. <br




