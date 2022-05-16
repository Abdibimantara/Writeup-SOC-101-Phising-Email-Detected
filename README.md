# Writeup-SOC-101-Phising-Email-Detected

Lets Defend Writeup

![defend](https://user-images.githubusercontent.com/43168046/168586256-8c8b8496-d9db-4e53-bf3c-5e6f605a9b67.png)

SOC101 Phsing Email Detected is a blue team challenge available on https://app.letsdefend.io/.

Our first step goes to the "Monitoring" section. focus on the soc101- Phishing Detected section.

![image](https://user-images.githubusercontent.com/43168046/168586516-397e1611-822f-474e-acbb-335ee70d9540.png)

the details of the alerts that we have to analyze

![image](https://user-images.githubusercontent.com/43168046/168588962-0f0626f8-25bd-44e9-92c2-b00485dcf899.png)
 
After knowing the details of the alert, enter the investigation section

![image](https://user-images.githubusercontent.com/43168046/168589029-c3191814-33bf-4db7-8631-bf7457ba16a1.png)
 
click playb0ok to start investigation

 ![image](https://user-images.githubusercontent.com/43168046/168589049-5d279d06-7d2e-4a72-96cb-1dfc75cf23c0.png)

The investigative alert stage is divided into 3 points
1. Detect
- Parse email
- Checking email, is there an attached URL in the email?
2. Analysis
- Email Url Analysis
- Add notes / important points	
- Delete Email if indicated phishing
3. Conclusion
-conclusion





Step 1- Detect
-	Parse Email 
![image](https://user-images.githubusercontent.com/43168046/168589085-9eb645e4-8b3b-458a-b986-1baf02acd83f.png)

-	When was it sent?
 
-	What is the email's SMTP address?
146.56.195.192

-	What is the sender address?
Lethuyan852@gmail.com

-	What is the recipient address? 
mark@letsdefend.io

-	Cheking email, is there an attached URL in the email?
Yes
 ![image](https://user-images.githubusercontent.com/43168046/168589241-81f41080-9d6c-4e49-a051-0714929821ac.png)


Step 2- Analysis
-	Is the mail content suspicious?
on the attached link, I tried to analyze through several tools

Virus Total : 

 ![image](https://user-images.githubusercontent.com/43168046/168589299-53deabef-caea-4260-9b17-1b25ef9ad0d2.png)

judging by the total viral results, the links generally read clean

Analysis Using Joe Sandbox 

![image](https://user-images.githubusercontent.com/43168046/168589331-6ccbdd80-bb8f-4cb9-9433-f88eaf676f77.png)
 
The URL indicates trojan activity

-	Important Points
Link url : http://nuangaybantiep.xyz/
Gmail : Lethuyan852@gmail.com
C2 : 146.56.195.192

-	Deleted Email 
because the email is phishing, the best advice is to delete it via mailbox
 ![image](https://user-images.githubusercontent.com/43168046/168589353-6283b1a0-4603-449f-9933-1335428bc5de.png)

Step 3- Conclusion
	The email contains a malicious link. The email is actually indicated as phishing. the link is involved in trojan activity

