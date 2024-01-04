<h1> Email Phishing Lab </h1>



 



<h2>Introduction/Description</h2>

This is a real-life phishing attempt that I found while browsing through my emails. In this lab, I will walk you through how I confirmed that this is a malicious attempt to steal more information about me and what I did to mitigate this user from attempting something like this again.

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


<br /> As shown in the malicious email, there are multiple things that are off about the email. The first thing that raised suspicion was that they claimed I had a LifeLock account from the company Norton but could not state my first name and addressed me as ADMIN.

Another problem with this email is that it claims to be from the company Norton, but if you look at the email header, the email address that sent this email does not match the domain name for the company Norton; it is a random Gmail account. This alone is enough to indicate that this is a phishing email with an attempt to steal your information.

Another red flag about this email is how they are urging you to take action as soon as possible. The email was sent on Dec 11th, and this was included in the end of the message: "In case you don't want to continue with us, then make sure you call us on 909 907 9883 before 12/11/2023 to avoid any recurring payment." This makes it seem like you are going to get charged since you missed the due date, even though the email was sent on the same day. Unfortunately, if you are an elderly person, not tech-savvy and aware of malicious attacks like this, or maybe just a super busy or stressed individual, you can easily fall victim to this. After gathering all this information, it was enough to continue my investigation.
<br />



## Raw Email Messeage Syantax:  <br/>

<img src="https://imgur.com/YIzole7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>  

<br />  This window displays the Raw Email Message Syntax, providing more information about the email itself. My main objective in examining the raw contents of the email was to identify the IP address that sent this email to further confirm that this is a malicious attack. As you can see, I highlighted the IP address that was used to send this email to my account.

<br />



 ## Virus Total Analysis :  <br/>

<img src="https://imgur.com/nGIcdWe.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<br />  As you can see in the window above, as soon as I ran the IP address into the OSNIT tool VirusTotal, it confirmed that the user who sent this email has a malicious IP address, indicating they have been reported by security vendors for malicious activity. I conducted a deeper analysis to find out more about the history of this IP address. I discovered that this IP address is in communication with a handful of malicious files.

Further analysis of this IP address revealed that the malicious files it is communicating with are mostly related to information gathering or stealing. Below is the VirusTotal window where I conducted a more in-depth analysis on this IP address. 

<img src="https://imgur.com/eBODNwh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<br />



## Investigation report:  <br/>

<img src="https://imgur.com/DhSMqZP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br /> 
"In this window, you can see the investigation report that I created for this incident. To view its contents, you can click on the picture. It includes the hostname, username, time of the event, MITRE ID, a brief description of what happened, evidence/artifacts, and recommendations to mitigate this malicious activity."

<br />



## Conclusion <br/>  

<br> "In conclusion, this overall wasn't a complex event to investigate, as long as you knew the right places to look, it was relatively easy. Especially since there were no links to redirect you to another domain or downloadable files in the email, which made the analysis portion of this investigation relatively quick. What you could also take from this real-life scenario is that malicious actors are getting really good at fabricating emails and posing as real companies, so you have to be really careful when clicking on emails. The email that was sent to my inbox looked like a legitimate email from Norton. It only raised suspicion because I do not have any active memberships with the company, which is what led me to my investigation of the email." <br/>  


















<h1> Email Phishing Lab 2 </h1>



 



<h2>Introduction/Description</h2>

This is another real-life phishing attempt that I found while browsing through my emails. In this lab, I will walk you through how I confirmed that this is a malicious attempt to steal more information about me and what I did to mitigate this threat actor from attempting something like this again.

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

 <br/> In the first window, you can see the email message I received in my inbox. Compared to the first email that I investigated, there are very few red flags left throughout the email, if any. The one thing that caught my attention was how the malicious actor tried to redirect the user to WhatsApp, which is not a common practice for established companies, raising further suspicion on this email. Other than that, it seemed like a legitimate email from a travel company <br/>
  <img src="https://imgur.com/OlK0JUz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 


<br />The next image shows the rest of the email, which provided links to different domains. I still wasn't sure if the email was malicious or not, so I avoided clicking the links for my safety.
<br />



## Raw Email Messeage Syantax:  <br/>
  <img src="https://imgur.com/3lVnGlC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 


<br />  To further continue my investigation, I pulled up the Raw Email Message Syntax so I could find the IP address of the user who sent this email. I would then scan the IP address in VirusTotal to help aid me in my investigation.

<br />



 ## Virus Total Analysis :  <br/>

<img src="https://imgur.com/FVvfm90.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<br />  After I ran the IP address of the user who sent this email through VirusTotal, it marked this user as non-malicious with 0 security vendors stating it is malicious. However, I was able to see that the IP address was in communication with other files. This led me to do a deeper analysis on VirusTotal and investigate the communicating files within this IP address.

<img src="https://imgur.com/254MFIF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

As I continued my investigation with the communicating files for that IP address I found out that 2 of the 13 files this IP address was communicating with were marked as malicious which rasied even futher suspicion. The first file had a score of 1/60 security vendors makrking the file as malicious and the second file had a score of 1/59 security vendors marking it as malicious.Even though the IP address was not marked for malicious activity that didnt mean it was totally clean. 


<br />



## Sandbox analysis/report <br/>

<img src="https://imgur.com/vSONIYg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br /> As I continued my investigation with the communicating files for that IP address, I found out that 2 of the 13 files this IP address was communicating with were marked as malicious, which raised even further suspicion. The first file had a score of 1/60, with security vendors marking the file as malicious, and the second file had a score of 1/59, with security vendors marking it as malicious. Even though the IP address was not marked for malicious activity, that didn't mean it was totally clean.


<br />



## Sandbox analysis/report 2  <br/>  
<img src="https://imgur.com/Z7K05AK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br> As I continued my investigation, you can see that there are a total of 20 connections to that redirected link presented in the email I received. There are IP addresses from Belgium, Germany, and the United States, all connecting with that domain. The next course of action I took was to scan these IP addresses to confirm if they were malicious or not.   <br/>
<img src="https://imgur.com/rf2w71F.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
<img src="https://imgur.com/ebDzbXB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>  

<br> After scanning just the first 3 IP addresses, I could confirm that those addresses were malicious or were communicating with malicious files. In conclusion, all 20 of the IP addresses that were in connection with the redirected link from the email were all malicious or in communication with malicious files. Above is one example of one of the malicious IP addresses that was in communication with this link. In the second window, you can see communicating files that are associated with this IP address. The total number of files is about 1 million, and about 90 percent of those files are malicious. <br/>
## Sandbox analysis/report 3 <br/>  

<img src="https://imgur.com/2UveA2z.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>  

<b>  For the last portion of my sandbox analysis on this email, I was able to see the threat that would be exposed to a user if they were to click this link. The picture above shows this. The threat was marked as malicious by ANY.RUN, the sandbox tool. The data was from a Suricata IDS. The threat was URL shortening. The main reason a malicious actor would shorten a URL link would be to hide the exact location a URL would take a user. The main reason would be because it is a malicious domain that can contain malware, dangerous downloadable files, viruses, or more <br/>  

## Investigation Report

<img src="https://imgur.com/vEmwHrx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>   



## Conclusion 
<b> In conclusion to this real-life email phishing lab, I was able to triage two different examples of email phishing attempts. The first email I found was relatively easy to detect and analyze. I was able to confirm it was a malicious email relatively quickly. The second email, however, I had to conduct a deeper analysis. I was not able to confirm it was a malicious email until I had scanned the redirected domains the email was trying to take a user to. I confirmed it was malicious when I saw all IP addresses connected to the redirected domain were marked as malicious by VirusTotal. Overall, what I gained from this lab is that malicious actors are getting better at creating fake email messages to compromise a user. This just serves as a reminder that you shouldn't give out your email to anyone, open emails you suspect are malicious, or click links in emails if you are not sure where the email is from." <b/> 




