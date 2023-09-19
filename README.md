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

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
![image](https://github.com/Raja8334/Enumeration/assets/120719634/6caaa262-965b-4c82-9bd5-239d5641b0c9)
filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files. Following searches for pdf file in the domain yahoo.com
# OUTPUT:
![image](https://github.com/Raja8334/Enumeration/assets/120719634/71a90d4b-bb1c-467d-90bb-7cdd560bf500)
intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
# OUTPUT:
![image](https://github.com/Raja8334/Enumeration/assets/120719634/09f6ff08-3557-4aaa-a144-ab7d82dc3111)
inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
# OUTPUT:
![image](https://github.com/Raja8334/Enumeration/assets/120719634/ac7f0b2b-3dde-44aa-a160-8421d83d2a20)
intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
# OUTPUT:
![image](https://github.com/Raja8334/Enumeration/assets/120719634/38551de5-b144-474b-814e-51b9eca3873f)
link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
# OUTPUT:
![image](https://github.com/Raja8334/Enumeration/assets/120719634/3005c095-b5e4-4eaf-8a2d-764d26be9737)
cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
# OUTPUT:
![image](https://github.com/Raja8334/Enumeration/assets/120719634/0c4b1698-b07f-458f-8231-8c275a5bc82c)
#DNS Enumeration ##DNS Recon provides the ability to perform: Check all NS records for zone transfers Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT) Perform common SRV Record Enumeration Top level domain expansion
# OUTPUT :
![image](https://github.com/Raja8334/Enumeration/assets/120719634/06720748-2e1c-4886-a338-1ab5e675ae56)
![image](https://github.com/Raja8334/Enumeration/assets/120719634/576ad4ae-69f5-49ba-b9f3-dc52651ac264)
## dnsenum:
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations: Get the host’s addresses (A record). Get the namservers (threaded). Get the MX record (threaded). Perform axfr queries on nameservers and get BIND versions(threaded). Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”). Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded). Calculate C class domain network ranges and perform whois queries on them (threaded). Perform reverse lookups on netranges (C class or/and whois netranges) (threaded). Write to domain_ips.txt file ip-blocks. This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.
# OUTPUT:
![image](https://github.com/Raja8334/Enumeration/assets/120719634/521105dd-e0e2-4351-8351-202a15821722)
user-enum Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
![image](https://github.com/Raja8334/Enumeration/assets/120719634/66e15746-e1c2-48bd-a0e8-02f8f221673e)
metasploit list all the usernames using head /etc/passwd or cat /etc/passwd: select any username in the first column of the above file and check the same
![image](https://github.com/Raja8334/Enumeration/assets/120719634/9ed5bca7-24b4-487a-ad36-114339f107c6)
smtp enumeration Telnet allows to connect to remote host based on the port no. For smtp port no is 25 telnet 25 to connect and issue appropriate commands
![image](https://github.com/Raja8334/Enumeration/assets/120719634/2e25d4e7-a7f9-453f-8204-e94ec07f100a)
## nmap –script smtp-enum-users.nse
The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.
![image](https://github.com/Raja8334/Enumeration/assets/120719634/eba745b0-769c-48c5-a1ad-bfe8c4b4e7e1)























## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

