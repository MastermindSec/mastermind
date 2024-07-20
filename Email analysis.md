
# Email Threat Analysis: A Comprehensive Approach

I have Applied My theoretical understanding to examine an email's details without the need to open it in an email application, and conduct Open Source Intelligence (OSINT) to extract additional data.

## Objective: 

### Demonstrate advanced email forensics techniques to identify and mitigate potential phishing threats.

[Second_Email.zip](https://github.com/user-attachments/files/16321662/Second_Email.zip)


Used the attachment titled: Second_Email.eml

Initial Sender Analysis

![1](https://github.com/user-attachments/assets/85e71684-2e15-4a1e-985d-e28b4b5ee35e)

Identified the sender's email infrastructure (Microsoft Office 365)

Examined 'Received' and 'Message-ID' fields for origin verification

<img width="468" alt="2" src="https://github.com/user-attachments/assets/2568eaac-059a-41cc-b80a-e9c062216ce7">

## IP Reputation Assessment
<img width="468" alt="3" src="https://github.com/user-attachments/assets/d0db48be-3d54-4da8-a30b-6826a3f1396c">

Evaluated sender's IP (40.107.215.98) with consideration for cloud service providers

<img width="468" alt="4" src="https://github.com/user-attachments/assets/74c48673-e7b4-4b63-b8c7-8da172df388c">


Noted potential limitations of IP blocking for major cloud platforms.
 
## Temporal Analysis


Documented email timestamp for investigation timeline

Correlated date with potential ongoing phishing campaigns


<img width="316" alt="5" src="https://github.com/user-attachments/assets/69f43b2f-2dfa-46ee-91c7-8cef1843a7f2">

## Sender Authenticity Verification

<img width="468" alt="6" src="https://github.com/user-attachments/assets/f344d341-a2c7-493e-905d-eb9320fc0e6e">

Detected misalignment between 'From' name and email domain
Identified suspicious domain: comunidadeduar.com[.]ar

## Subject Line Threat Indicators

<img width="468" alt="7" src="https://github.com/user-attachments/assets/5cc81240-c3c5-46a9-bf8e-ffdb701da5de">


Recognized urgency tactics in subject line suggestive of phishing attempts

## Technical Header Examination


<img width="468" alt="9" src="https://github.com/user-attachments/assets/e6690686-cf9b-4ff1-af4f-06f16c7441e2">


Analyzed 'X-Mailer' field to determine email client used
Utilized whatismybrowser[.]com for user agent identification


## Content Structure Analysis

<img width="468" alt="10" src="https://github.com/user-attachments/assets/370d0b9f-1cdf-42c7-ace7-849b17f52c62">


Identified multipart/mixed content type

Located and examined email boundaries for different content sections
<img width="468" alt="11" src="https://github.com/user-attachments/assets/8e2e73d2-4983-42bf-8795-2732c544878b">

## URL and Attachment Inspection


Discovered potentially malicious Google script URL

<img width="468" alt="12" src="https://github.com/user-attachments/assets/2ecf18b9-222b-4231-a991-f2493e64c8ca">


<img width="468" alt="13" src="https://github.com/user-attachments/assets/3444442f-fe7c-4db1-8ece-31794a9de8bb">


Analyzed base64 encoded attachment using CyberChef for decoding


<img width="468" alt="14" src="https://github.com/user-attachments/assets/ebe897c8-3c20-4b72-b44d-cf2c8d2fb9ee">


![15-1](https://github.com/user-attachments/assets/1d87afd8-d97d-48ef-87c3-1e4dd43c6929)



<img width="468" alt="17" src="https://github.com/user-attachments/assets/4cad46a5-82cb-48a4-9f2f-cb1ca83143b7">



![20](https://github.com/user-attachments/assets/b7891274-0213-4d49-8af1-d5d85a9a199e)


## Email Authentication Protocol Verification


<img width="468" alt="21" src="https://github.com/user-attachments/assets/7ac7aa72-6a1d-445c-980c-03aa0ffe1106">


Evaluated SPF, DKIM, and DMARC results
Noted passing SPF but absent DKIM configuration

## Domain OSINT

<img width="468" alt="22" src="https://github.com/user-attachments/assets/661d7935-040c-499c-8867-c310f94b56a6">



Conducted domain age analysis using DomainTools Whois

<img width="468" alt="24" src="https://github.com/user-attachments/assets/52b4c282-2071-41db-a48a-3f0d1a89cd6f">
<img width="317" alt="25" src="https://github.com/user-attachments/assets/a0964b40-8cb6-473c-a9b5-e986a72ab8cd">



Performed reputation check on VirusTotal

## URL Analysis and Threat Intelligence

Attempted URL analysis using SquareX sandbox

<img width="468" alt="27" src="https://github.com/user-attachments/assets/1898ef60-9da4-4dbd-9ef9-e3021a5d7a3a">


Pivoted to URLscan.io for similar URL patterns and potential threats

<img width="468" alt="28" src="https://github.com/user-attachments/assets/3e10eb0d-1cf2-4f3e-92c7-b6445adb44ed">



## Comprehensive Findings Documentation

Compiled key artifacts and indicators of compromise

<img width="468" alt="29" src="https://github.com/user-attachments/assets/da14cb60-08c8-4b54-862d-7862ff978f78">

<img width="468" alt="30" src="https://github.com/user-attachments/assets/2f51b961-6781-46ec-9550-37c396650d40">

Formulated actionable next steps for incident response


#### This methodical approach demonstrates proficiency in email forensics, threat intelligence gathering, and incident response planning. It showcases the ability to leverage various tools and techniques to thoroughly analyze potential threats and provide actionable insights for organizational security.






