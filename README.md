
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

![Screenshot 2024-05-07 084242](https://github.com/kavisree86/Enumeration/assets/145759687/209308b8-1716-4630-a20f-b12c70748e75)



filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
## filetype:
![Screenshot 2024-05-07 085427](https://github.com/kavisree86/Enumeration/assets/145759687/69de6f3c-eb40-47c8-9e64-788d3ea13d1c)



intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
## intext:
![Screenshot 2024-05-07 085427](https://github.com/kavisree86/Enumeration/assets/145759687/618b343c-3d99-4ebd-91ec-133ab7f46d44)



inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

## inrul:
![Screenshot 2024-05-07 085717](https://github.com/kavisree86/Enumeration/assets/145759687/15a316a7-f030-42b7-be2a-07be3b6f98de)


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

![image](https://github.com/kavisree86/Enumeration/assets/145759687/c23a250c-87cd-4893-a2fd-cf8708760914)




link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

![image](https://github.com/kavisree86/Enumeration/assets/145759687/69921fae-2f9e-4ed1-a5c9-65d340da44dc)



cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.


![image](https://github.com/kavisree86/Enumeration/assets/145759687/a256999e-9981-49a0-a0b2-8b4559cf7cfc)


 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
![image](https://github.com/kavisree86/Enumeration/assets/145759687/60bf4d4e-dd48-4af6-8e57-531e26deb990)








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

![image](https://github.com/kavisree86/Enumeration/assets/145759687/ed40ceda-60e7-4da1-9dae-ca35c21529fc)


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
![image](https://github.com/kavisree86/Enumeration/assets/145759687/d9691427-6972-4c25-bbf0-970e6380ec79)


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same
![image](https://github.com/kavisree86/Enumeration/assets/145759687/35b4120d-3d02-49e1-a254-22581f289ef4)


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output
 ![image](https://github.com/kavisree86/Enumeration/assets/145759687/16f4df7e-9028-43d2-9f4f-b4242013d072)

  
  

## nmap –script smtp-enum-users.nse <hostname>
![image](https://github.com/kavisree86/Enumeration/assets/145759687/c0fdb08f-7cb5-4254-8c49-b2e15a728daa)


The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.




## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

