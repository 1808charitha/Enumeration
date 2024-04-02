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
![image](https://github.com/1808charitha/Enumeration/assets/132996838/0cbaecbf-60c3-4469-8360-70e5c31422c7)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
![image](https://github.com/1808charitha/Enumeration/assets/132996838/c1c20884-da49-4d30-8efc-af5a37cc26a1)



intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
![image](https://github.com/1808charitha/Enumeration/assets/132996838/8df24f1a-097c-4a02-a221-7733acdc9fcb)



inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
![image](https://github.com/1808charitha/Enumeration/assets/132996838/07d63022-3840-45d1-8411-59b9b854b173)


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
![image](https://github.com/1808charitha/Enumeration/assets/132996838/aa5eb04a-2a15-40ad-9610-a0111eff41d7)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
![image](https://github.com/1808charitha/Enumeration/assets/132996838/a5d74f5d-0d9e-4a73-ba1e-5448de09056c)


cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
![image](https://github.com/1808charitha/Enumeration/assets/132996838/82876daa-a256-4b18-a59a-c80fd9912a42)


 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
![image](https://github.com/1808charitha/Enumeration/assets/132996838/9ce2805b-0413-4cde-97f3-0a9623e551ea)








##dnsenum
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
![image](https://github.com/1808charitha/Enumeration/assets/132996838/d97f68a6-0422-419c-bdf2-1df41c2e5252)



##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
![image](https://github.com/1808charitha/Enumeration/assets/132996838/9d497159-c19c-41c6-8b7d-5051ef741d32)


select any username in the first column of the above file and check the same
![image](https://github.com/1808charitha/Enumeration/assets/132996838/9128921e-c9b8-4f6d-90af-8ea50d9e2663)



#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output
 ![image](https://github.com/1808charitha/Enumeration/assets/132996838/ac8623de-7aa9-43ce-ab9a-e060b4123a9a)

  
  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
![image](https://github.com/1808charitha/Enumeration/assets/132996838/afbb285f-c0dd-4e91-89a2-3fc6968db3a5)



## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

