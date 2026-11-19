# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com



intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
## OUTPUT:
 ## Google Hacking — Search Operators:
 <img width="927" height="952" alt="Screenshot 2026-11-19 083752" src="https://github.com/user-attachments/assets/3b55dc13-baf0-4f1e-af5d-04e1f8417c72" />
<img width="902" height="970" alt="Screenshot 2026-11-19 084018" src="https://github.com/user-attachments/assets/33b6c93f-18c2-4b0b-9df7-eb5cdef7b99b" />
<img width="956" height="976" alt="Screenshot 2026-11-19 084111" src="https://github.com/user-attachments/assets/3be26a70-8b3f-490f-9f58-8b4c6029d511" />
<img width="917" height="976" alt="Screenshot 2026-11-19 084041" src="https://github.com/user-attachments/assets/1e38fde8-33bf-4bbb-8095-3c9aec7df864" />



##DNS Enumeration


## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion

## OUTPUT:
<img width="641" height="222" alt="image" src="https://github.com/user-attachments/assets/60d0a7d8-4180-49a8-93ee-edadda9940f9" />







## dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.
## OUTPUT:
<img width="640" height="422" alt="image" src="https://github.com/user-attachments/assets/c60c586b-b16a-42b2-a7d2-9e595ae6a598" />
## DNS lookup-dig:
## OUTPUT:
<img width="612" height="450" alt="image" src="https://github.com/user-attachments/assets/f9fca20b-43e0-4905-a3f6-f96a1dbe6322" />

<img width="646" height="285" alt="image" src="https://github.com/user-attachments/assets/9592a369-d3a3-4f9d-aab1-4449dfba6a43" />



## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same
## OUTPUT:
<img width="637" height="340" alt="image" src="https://github.com/user-attachments/assets/8f9887c6-b0ec-4fb7-a822-8124c7286154" />

## Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
## OUTPUT:
  <img width="616" height="207" alt="image" src="https://github.com/user-attachments/assets/073a6091-1318-47df-8560-5727590eb0bb" />
<img width="650" height="372" alt="image" src="https://github.com/user-attachments/assets/a016f9d9-0151-4045-b579-8cd58226a167" />


  


  
  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.
## OUTPUT:

<img width="640" height="203" alt="image" src="https://github.com/user-attachments/assets/db92d098-d862-4693-a3ed-e9733916ee71" />


<img width="637" height="277" alt="image" src="https://github.com/user-attachments/assets/c1dc8de8-e95e-4f09-9fa5-319a4fce37f3" />


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

