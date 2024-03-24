# Information Gathering tools
## 1. dmitry (Deepmagic Information Gathering Tool)
### High-Level Summary
> Dmitry is a free and open-source tool which is used for information gathering. Dmitry stands for DeepMagic Information Gathering Tool. It’s a command-line tool Using Dmitry tool You can collect information about the target, this information can be used for social engineering attacks. It can be used to gather a number of valuable pieces of information.
### Recommendations
> Information Gathering Tool through which we can get all basic required information of it
### Methodologies
> In Kali Linux only it is pre defined tool which can be used for Information Gathering Scope of this Tool is to scan possible subdomains, email addresses, tcp port scan of a host, lookup on the IP address of a host.
### Service Enumeration
> By this we can get to know which all are live application running on the system
### Penetration
> N.A
### System Vulnerable:
> dmitry -s domain
### Report – House Cleaning
> Clean up was conducted after assessment of each target to remove any artifacts from the penetration test. The removals included any user accounts created and any files uploaded to the targets. Additionally, any configuration changes made were reverted to their original state.

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/6d64e983-7499-4f54-8d4b-fc39f3b966c1)

We can scan all subdomains of an Ip address of a host

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/40181af0-a8dc-4722-b816-8e8e62f882c2)

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/672a45e3-f35a-4185-bb9d-928696671ce5)

## 2. Nmap(Network Mapper)
### High-Level Summary
> NMAP uses raw IP packets in novel ways to determine which hosts are available on the network, what services (application name and version) those hosts are offering, which operating systems (and OS versions) they are running, what type of packet filters/firewalls are in use, etc.
### Recommendations
> This Tool is majorly used in port scanning and security auditing
### Methodologies
> Its free utility tool available in kali linux
### Information Gathering
Discovers Hosts, Scanning order and port specification, The detection of service or version and operating system, Scanning Ports.
### Service Enumeration
> N.A
### Penetration
> We can get the information of open ports in that particular domain

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/5bd027c8-d4e7-4dbb-a1cf-83de96b6e34c)

### Report – House Cleaning
> Clean up was conducted after assessment of each target to remove any artifacts from the penetration test. The removals included any user accounts created and any files uploaded to the targets. Additionally, any configuration changes made were reverted to their original state.

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/c933f7bf-31e4-4c5f-93a9-59f1fa32b441)

## 3. Maltego
### High-Level Summary
> Maltego is an open-source intelligence forensic application. Which will help you to get more accurate information and in a smarter way. In simple words, it is an information-gathering tool.
### Recommendations
> This Tool is majorly used in port scanning and security auditing.
### Methodologies
> Its free utility tool available in kali linux

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/0f857cad-a44a-493c-8ed5-03acb009ea0e)

### Information Gathering
> Discovers Hosts, Scanning order and port specification, The detection of service or version and operating system, Scanning Ports.
### Service Enumeration
> N.A.
### Penetration
> We can get the information of open ports in that particular domain
### Report – House Cleaning
> Clean up was conducted after assessment of each target to remove any artifacts from the penetration test. The removals included any user accounts created and any files uploaded to the targets. Additionally, any configuration changes made were reverted to their original state.

# Vulnerability Analysis Tools
## 1. Nikto
### High-Level Summary
> Nikto is an open-source web server scanner which performs comprehensive tests against web servers for multiple items. You can use Nikto with any web servers like Apache, Nginx, IHS, OHS, Litespeed, and so on. Nikto can check for server configuration items such as the presence of multiple index files, HTTP server options, and will attempt to identify installed web servers and software. Items and plugins scanned by Nikto are frequently updated and can be automatically updated.
### Recommendations
> This Tool is majorly used in port scanning and security auditing.
### Methodologies
> Its free utility tool available in kali linux

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/fba81a2d-9fc1-4b5d-a33b-7e7de22ce4a8)

### Information Gathering
> Discovers Hosts, Scanning order and port specification, The detection of service or version and operating system, Scanning Ports. 
### Service Enumeration
> N.A.
### Penetration
> We can get the information of open ports in that particular domain
### Report – House Cleaning
> Clean up was conducted after assessment of each target to remove any artifacts from the penetration test. The removals included any user accounts created and any files uploaded to the targets. Additionally, any configuration changes made were reverted to their original state.

## 2. Legion
### High-Level Summary
> Legion tool is a super-extensible and semi-automated network penetration testing framework.GUI with panels and a long list of options that allow pentesters to quickly find and exploit attack vectors on hosts. It has the feature of real-time auto-saving of project results and tasks. Legion also provides services like Automatic recon and scanning with NMAP, whataweb, sslyzer, Vulners, webslayer, SMBenum, dirbuster, nikto, Hydra, and almost 100 auto-scheduled scripts are added to it. Modular functionality of Legion Tool allows users to easily customize Legion.
### Recommendations
> Automatic detection of CVEs (Common Vulnerabilities and Exposures and CPEs (Common Platform Enumeration).
### Methodologies
> Its free utility tool available in kali linux which is GUI Based and also we can customize it.

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/c9993f06-6a8c-4fce-82d0-1e453978dcfc)

### Information Gathering
> We can conduct host discovery, custom port scanning, and custom discovery options.

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/4a95b41e-cda3-4db2-98c4-0529f81fe744)

### Service Enumeration
> N.A.
### Penetration
> We can get the information of open ports of host and many more options like auto detecting CVE
### Report – House Cleaning
> Clean up was conducted after assessment of each target to remove any artifacts from the penetration test. The removals included any user accounts created and any files uploaded to the targets. Additionally, any configuration changes made were reverted to their original state.

## 3. Nmap Scripting Engine (NSE)
### High-Level Summary
> The Nmap Scripting Engine (NSE) is a powerful component of the Nmap (Network Mapper) tool that allows users to automate a variety of tasks during network exploration and security scanning. NSE is designed to extend the functionality of Nmap by enabling users to run scripts to perform tasks beyond traditional port scanning. These scripts can be used to gather additional information about target systems, detect vulnerabilities, or even automate exploitation. Nmap Scripts are written in Lua Language
### Recommendations
> Automatic detection of CVEs (Common Vulnerabilities and Exposures and CPEs (Common Platform Enumeration).
### Information Gathering
> We can conduct host discovery, custom port scanning, and custom discovery options.

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/b94e77d7-5900-45c7-afaa-bbd40ae0a2ad)

### Service Enumeration
> N.A.
### Penetration
> We can get the information of open ports of host and many more options like auto detecting CVE
### Report – House Cleaning
> Clean up was conducted after assessment of each target to remove any artifacts from the penetration test. The removals included any user accounts created and any files uploaded to the targets. Additionally, any configuration changes made were reverted to their original state.

# Web Application Analysis Tools
## 1. Burp Suite
### High-Level Summary
> Burp Suite is a cybersecurity tool designed for web application security testing. It is help in finds bugs in the websites and is gui based tool. There are 3 additions of burp suite
*  Burp suite community (Free)
*  Burp suite professional
*  Burp suite Enterprise

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/db6ca6cb-d27f-441f-9e6f-ce832b15dad2)

### Recommendations
> It is used to perform security testing in web application and also finding exploits in that surface.
### Methodologies
> It contain many features some them are
* Proxy: Burp Suite acts as a proxy server between the user's browser and the target web application. It allows the user to intercept and modify the communication between the two, enabling the analysis and manipulation of HTTP requests and responses.
* Intruder: Burp Intruder is a powerful tool for performing automated attacks against web applications. It can be used to test the susceptibility of an application to different types of attacks, such as brute force and parameter tampering.

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/64670b3b-eb28-42e5-945c-39f3aa57a08c)

### Information Gathering
> We can conduct host discovery, custom port scanning, and custom discovery options.
### Service Enumeration
> N.A
### Penetration
> We can get the information of open ports of host and many more options like auto detecting CVE
### Report – House Cleaning
> Clean up was conducted after assessment of each target to remove any artifacts from the penetration test. The removals included any user accounts created and any files uploaded to the targets. Additionally, any configuration changes made were reverted to their original state.

## 2. WPScan-(WordPress Scan)
### High-Level Summary
> WordPress is known to have many flaws and vulnerabilities. WPScan will scan the WordPress website for its version, plugins, users and also has an in-built password cracker
### Recommendations
> This is used specifically for Websites hosted on WordPress.
### Methodologies
> Checking the version of WordPress used and associated vulnerabilities for that version. Checks for database dumps that may be openly accessible.
### Information Gathering
> We can conduct host discovery, custom port scanning, and custom discovery options.

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/ed627d70-d3a8-4912-91f3-00d39205e4f0)

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/085db268-b9ef-43f1-bb5f-cba13c4ce2f8)

### Service Enumeration
> N.A.
### Penetration
> We can get the information of open ports of host and many more options like auto detecting CVE
### Report – House Cleaning
> Same as above

## 3. WhatWeb
### High-Level Summary
> WhatWeb identifies websites. It recognises web technologies including content management systems (CMS), blogging platforms, statistic/analytics packages, JavaScript libraries, web servers, and embedded devices.
### Recommendations
> It scans website with aggression level set to 1 -v is for more readablility
### Methodologies
> This tool can identify and recognize all the web technologies available on the target website. This tool can identify technologies used by websites such as blogging, content management system, all JavaScript libraries. .
### Information Gathering
> We can conduct host discovery, custom port scanning, and custom discovery options.

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/d8d583a3-cc81-4dbc-aa24-3bd33b7f8c86)

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/680ac296-4977-4663-990a-34964897da80)

### Service Enumeration
> N.A.
### Penetration
> WhatWeb is responsible for grabbing particular information from the target website. Whatweb works as an information-gathering tool and can identify all the email addresses, SQL errors, technology used in the website.
### Report – House Cleaning
> Same as above

# Database Management Tools
## 1. SqlMap
### High-Level Summary
> Sqlmap is a python based tool; therefore it should operate on any system that supports Python. The purpose of sqlmap is to find and take benefit of SQL injection vulnerabilities in web applications.
### Recommendations
> It includes a robust detection engine, numerous specialist features for the ultimate penetration tester, and a wide range of switches that span database fingerprinting, data retrieval from databases, access to the underlying file system, and executing commands on the operating system via out-of-band connections.
### Methodologies
> When it detects one or more SQL injections on the target host, the user can choose from a number of options, including performing an extensive back-end database management system fingerprint, retrieving DBMS session user and database, enumerating users, password hashes, privileges, databases, dumping entire or user-specific DBMS table/columns, running his own SQL statement, reading particular files on the file system and more.
### Information Gathering
The purpose of sqlmap is to find and take benefit of SQL injection vulnerabilities in web applications.

![Screenshot 2024-01-07 224121](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/bda05b12-51a2-438f-b9cb-9b3513770c28)

### Service Enumeration
> N.A.
### Penetration
> By giving DBMS credentials, IP address, port, and a database name, it is possible to connect to the database directly without using SQL injection.
### Report – House Cleaning
> Same as above

# Password Attacks Tools
## 1. Medussa
### High-Level Summary
> Medusa is a modular, speedy, and parallel, login brute-forcer. It is a very powerful and lightweight tool. Medusa tool is used to brute-force credentials in as many protocols as possible which eventually lead to remote code execution. It currently has over 21 modules, some of which are: PcAnywhere, POP3, CVS, FTP etc.
### Recommendations
> N.A.
### Methodologies
> It works on bruteforce method
### Information Gathering

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/ca6e09b1-6994-4cf8-92ca-0c816ecf54c5)

### Service Enumeration
> N.A.
### Penetration
> It uses the wordlist which is available on kali linux and apply brute force method
### Report – House Cleaning
> Same as above

## 2. Crunch
### High-Level Summary
> In order to hack a password, we have to try a lot of passwords to get the right one. When an attacker uses thousands or millions of words or character combinations to crack a password there is no surety that any one of those millions of combinations will work or not
### Recommendations
> This collection of a different combination of characters is called a wordlist. And in order to crack a password or a hash, we need to have a good wordlist which could break the password. So to do so we have a tool in Kali Linux called crunch.
### Methodologies
> crunch is a wordlist generating tool that comes pre-installed with Kali Linux. It is used to generate custom keywords based on wordlists. It generates a wordlist with permutation and combination. We could use some specific patterns and symbols to generate a wordlist.
### Information Gathering

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/892d67b8-1eb8-43b7-b4db-2350e1e98c1d)

### Service Enumeration
> N.A.
### Penetration
> It uses the wordlist which is available on kali linux and apply brute force method
### Report – House Cleaning
> Same as above

## 3. Hash Identifier
### High-Level Summary
> As the name is it used to identify the type of hashes that is given as input further based on the hash information we can crack hash using any other tools.
### Recommendations
> This collection of a different combination of characters is called a wordlist. And in order to crack a password or a hash, we need to have a good wordlist which could break the password. So to do so we have a tool in Kali Linux called crunch.
### Methodologies
> It simply suggests type of hash whether its of MD5 or hash
### Information Gathering

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/388f1951-a9e5-4279-a7f8-7dc84f2afd7c)

### Service Enumeration
> N.A.
### Penetration
> N.A
### Report – House Cleaning
> Same as above

# Wireless attacks Tools

## 1.Wifite
### High-Level Summary
> Wifite is a tool to audit WEP or WPA encrypted wireless networks. It uses aircrack-ng, pyrit, reaver, tshark tools to perform the audit.
### Recommendations
> This collection of a different combination of characters is called a wordlist. And in order to crack a password or a hash, we need to have a good wordlist which could break the password. So to do so we have a tool in Kali Linux called crunch.
### Methodologies
> When cracking the passwords for multiple networks it sorts them based on their signal strength. Packed with a lot of customizing options to improve the effectiveness of the attack. Changes mac address while attacking to make the attacker anonymous.
### Information Gathering
> If an attacker finds any target not appropriate to be attacked, so it allows the attacker to block the attack for the specific network. It saves all passwords to a separate file.

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/caccddc9-22a1-4493-9166-4f2feb59c90f)

### Service Enumeration
> N.A.
### Penetration
> N.A
### Report – House Cleaning
> Same as above

## 2. Revear
### High-Level Summary
> Reaver is a package that is a handy and effective tool to implement a brute force attack against Wifi Protected Setup (WPS) registrar PINs to recover WPA/WPA2 passphrases. It is depicted to be a robust and practical attack against WPS, and it has been tested against a wide variety of access points and WPS implementations. In today’s time hacking WPA/WPA2 is exceptionally a tedious job.
### Recommendations
> Normal Dictionary attack could take days, and still will not succeed. On average Reaver will take 4-10 hours to recover the target AP’s plain text WPA/WPA2 passphrase, depending on the AP. Generally, it takes around half of this time to guess the correct WPS pin and recover the passphrase.
### Methodologies
> First we can scan the available networks with airodump-ng and selected one network and we will take the bssid of that network and we will give the input to the reaver and try to brutteforce the password.
### Information Gathering

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/46574fbc-3666-4274-8bd5-78568a68c7ef)

### Service Enumeration
> N.A.
### Penetration
> N.A
### Report – House Cleaning
> Same as above

## 3. Aircrack Ng
### High-Level Summary
> Aircrack-ng is a popular open-source tool suite used for penetration testing and network security assessments. It is specifically designed for assessing the security of Wi-Fi networks. 
### Recommendations
> Normal Dictionary attack could take days, and still will not succeed. On average Reaver will take 4-10 hours to recover the target AP’s plain text WPA/WPA2 passphrase, depending on the AP. Generally, it takes around half of this time to guess the correct WPS pin and recover the passphrase.
### Methodologies
> First we can scan the available networks with airodump-ng and selected one network and we will take the bssid of that network and we will give the input to the reaver and try to brutteforce the password.
### Information Gathering

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/5014890a-f137-487b-8d17-534abbdfee2a)

### Service Enumeration
> N.A.
### Penetration
> N.A
### Report – House Cleaning
> Same as above

# Reverse Engineering Tools
## 1. Nasm
### High-Level Summary
> NASM stands for Netwide Assembler. It's a popular assembler for the x86 architecture used in many Unix-like operating systems, including Linux.
### Recommendations
> This tool Nasm very useful when we have understand the machine level language and what it does.
### Methodologies
> NASM take assembly language code, which is a low-level programming language that closely maps to machine code, and convert it into machine code or object code that a computer's processor can understand and execute.
### Information Gathering

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/9b6af4fd-4c0e-4f2f-8f9b-381557e57f56)

### Service Enumeration
> N.A.
### Penetration
> N.A
### Report – House Cleaning
> Same as above

## 2. Radare2
### High-Level Summary
> Radare2 is an open-source framework for reverse engineering and binary analysis. It provides a comprehensive set of tools for examining, analyzing, and understanding binary files.
### Recommendations
> Radare2 is used by a diverse group of individuals, including security professionals, researchers, and hobbyists. It is particularly useful for reverse engineers, who rely on tools like r2 to understand and analyze code at a low level. This article will introduce you to radare2 and explore its key features and benefits.
### Methodologies
> Disassembling and analyzing code, Debugging with Radare2 is also possible
### Information Gathering

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/2a95372c-6393-487b-95ea-cfacbd850a77)

### Service Enumeration
> N.A.
### Penetration
> N.A
### Report – House Cleaning
> Same as above

# Exploitation tools
## 1. Metasploit
### High-Level Summary
> Metasploit is an open-source platform that supports vulnerability research, exploit development, and the creation of custom security tools.It contains many exploits and we can get exploit to many well known vulnerabilities. And it also supports some scanners to.

### Recommendations
> N.A.
### Methodologies
> Disassembling and analyzing code, Debugging with Radare2 is also possible
### Information Gathering

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/c9030a50-e73f-4315-86dc-1cf2044516d5)

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/be99d993-8fb4-45d1-a702-2677c2325f51)

### Service Enumeration
> N.A.
### Penetration
> N.A
### Report – House Cleaning
> Same as above

## 2. Searchsploit
### High-Level Summary
> SearchSploit is a command-line search tool for Exploit-DB that allows you to take a copy of the Exploit Database with you.
### Recommendations
> SearchSploit is very useful for security assessments when you don’t have Internet access because it gives you the power to perform detailed offline searches for exploits in the saved Exploit-DB.
### Methodologies
> suppose we are taking the vulnerable machine here i.e 192.168.219.129 we get some info about the services that are running on the port here take port 21 so the service running on the port 21 is vsftpd 2.3.4 if try check for the possible exploit in searchsploit we can get the result.
### Information Gathering

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/e74e35ac-dbf8-4021-81ef-340940ac9bb6)

### Service Enumeration
> N.A.
### Penetration
> N.A
### Report – House Cleaning
> Same as above

# Sniffing and Spoofing tools
## 1. Wireshark
### High-Level Summary
> Wireshark is a free and open-source packet analyzer tool used for network troubleshooting, analysis, and communication protocol development and education.
### Recommendations
> It captures network traffic from ethernet, Bluetooth, wireless (IEEE.802.11), and frame relay connections, among others, and stores that data for offline analysis.
### Methodologies
> This image shows the main page of the wireshark it contains many options for capturing the traffic the we select interface eg eth0 for etherenet we can see that some traffic going through eth0 we can select the interface and start the capture.
### Information Gathering

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/07cc7917-9f94-4290-ad6c-edb0460788fb)

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/a7f05912-8443-47dd-b9d5-2dedce616dbe)
### Service Enumeration
> N.A.
### Penetration
> We can filter as per our requirement which we need.
### Report – House Cleaning
> Same as above

## 2. TcpDump
### High-Level Summary
> This program allows you to dump the traffic on a network. tcpdump is able to examine IPv4, ICMPv4, IPv6, ICMPv6, UDP, TCP, SNMP, AFS BGP, RIP, PIM, DVMRP, IGMP, SMB, OSPF, NFS and many other packet types.
### Recommendations
> It can be used to print out the headers of packets on a network interface, filter packets that match a certain expression. You can use this tool to track down network problems, to detect attacks or to monitor network activities.
### Methodologies
> we use tcpdump command to run tcpdump -i to specify interface here we are using eth0 interface that is ethernet -v increase the verbosity are make the output more readable.
### Information Gathering

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/fbb71917-7c4d-4ea9-ac64-2fae83513c53)

###Service Enumeration
> N.A.
### Penetration
> N.A.
### Report – House Cleaning
> Same as above

## 3. Macchanger
### High-Level Summary
> GNU MAC Changer is an utility that makes the maniputation of MAC addresses of network interfaces easier. MAC addresses are unique identifiers on networks, they only need to be unique, they can be changed on most network hardware.
### Recommendations
> Kali linux comes pre installed with a tool called macchanger which allows us to change mac address on a temporary basis.
### Methodologies
> If you have prior experience with Kali Linux then you would understand that eth0 is the name of the system’s networking interface card or NIC.Always remember to specify the name of the interface whenever working with macchanger. Let us now change into a particular mac address,If you observe the help option then you can see that in order to that we need to use the -m argument.Use the help option well if you want to get proficient in using professional tools.
### Information Gathering

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/bb00af0d-3a4e-418c-8c4c-884d58af42bb)

### Service Enumeration
> N.A.
### Penetration
> Sometimes to manipulate the mac address we have to change the device Mac Address
### Report – House Cleaning
> Same as above

# Post Exploitation Tool
## 1. Netcat
### High-Level Summary
> A simple Unix utility which reads and writes data across network connections using TCP or UDP protocol. It is designed to be a reliable “back-end” tool that can be used directly or easily driven by other programs and scripts
### Recommendations
> At the same time it is a feature-rich network debugging and exploration tool, since it can create almost any kind of connection you would need and has several interesting built-in capabilities.
### Methodologies
> suppose when generated and ran the payload in the target machine we got the reverse shell using netcat
### Information Gathering

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/b9ee43f3-f5b6-4a33-a698-3734970fb2d5)

### Service Enumeration
> N.A.
### Penetration
> N.A
### Report – House Cleaning
> Same as above

## 2. Weevely
### High-Level Summary
> Weevely is a stealth PHP web shell that simulate telnet-like connection. It is an essential tool for web application post exploitation, and can be used as stealth backdoor or as a web shell to manage legit web accounts, even free hosted ones.
### Recommendations
> At the same time it is a feature-rich network debugging and exploration tool, since it can create almost any kind of connection you would need and has several interesting built-in capabilities.
### Methodologies
> suppose when generated and ran the payload in the target machine we got the reverse shell using netcat
### Information Gathering

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/51d7cf25-e6da-4beb-8335-36875dcd4ee9)

### Service Enumeration
> N.A.
### Penetration
> N.A
### Report – House Cleaning
> Same as above

## 3. mimikatz
### High-Level Summary
> Mimikatz is also capable of assisting in lateral movements and privilege escalations. Attacks like Pass-the-Hash, Pass-the-Ticket, Over-Pass-the-Hash, Kerberoasting etc. can also be achieved with Mimikatz.
### Recommendations
> Mimikatz abuses and exploits the Single Sign-On functionality of Windows Authentication that allows the user to authenticate himself only once in order to use various Windows services.
### Methodologies
> After a user logs into Windows, a set of credentials is generated and stored in the Local Security Authority Subsystem Service (LSASS) in the memory. As the LSASS is loaded in memory, when invoked mimikatz loads its dynamic link library (dll) into the library from where it can extract the credential hashes and dumps them onto the attacking system, and might even give us cleartext passwords.
### Information Gathering

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/5223d6bd-52c3-45a5-9479-3435a7bd84c7)

### Service Enumeration
> N.A.
### Penetration
> N.A
### Report – House Cleaning
> Same as above

# Social Engineering Tools
## 1. SET(Social Engineering Tool kit)
### High-Level Summary
>The Social-Engineer Toolkit (SET) is an open-source Python-driven tool aimed at penetration testing around Social-Engineering.It can be used to perform various social engineering attacks like email phisphing, site phisphing etc.
### Recommendations
> The Spear-phishing module allows you to specially craft email messages and send them to your targeted victims with attached FileFormatmalicious payloads. For example, sending malicious PDF document which if the victim opens, it will compromise the system.
### Methodologies
> The web attack module is a unique way of utilizing multiple web-based attacks in order to compromise the intended victim. This module is used by performing phishing attacks against the victim if they click the link. There is a wide variety of attacks that can occur once they click a link.
### Information Gathering

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/710bb834-499f-4ebb-8fbd-465f6163e9ed)

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/bd0f8dac-fb67-4fa7-86cd-c00ec3483e9f)

### Service Enumeration
> N.A.
### Penetration
> N.A
### Report – House Cleaning
> Same as above

# Forensic Tools
## 1. BinWalk
### High-Level Summary
> Binwalk is a great tool when we have a binary image and have to extract embedded files and executable codes out of them.
### Recommendations
> It is even used to identify the files and codes which are embedded inside the firmware images. Binwalk is compatible with magic signatures for UNIX file utility as it uses libmagic library.
### Methodologies
> binwalk supports a variety of command-line options that allow you to customize the analysis and extraction process, such as the signature database to use, the output format, or the extraction options. You can use these options to fine-tune the analysis and extraction to suit your needs.
### Information Gathering

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/48daf9ef-87d8-4890-bb24-1740f5bdf800)

### Service Enumeration
> N.A.
### Penetration
> N.A
### Report – House Cleaning
> Same as above

## 2. Autopsy
### High-Level Summary
> Autopsy is a digital forensics tool that is used to gather the information form forensics. Or in other words, this tool is used to investigate files or logs to learn about what exactly was done with the system.
### Recommendations
> It could even be used as a recovery software to recover files from a memory card or a pen drive.
### Methodologies
> Autopsy comes pre-installed in Kali Linux Just type “autopsy” in the terminal.
### Information Gathering

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/4fc04452-ad54-45b9-89c8-22ddacaeb592)

### Service Enumeration
> N.A.
### Penetration
> N.A
### Report – House Cleaning
> Same as above

# Reporting Tools
## 1. Cherry tree
### High Level summary
> CherryTree is a hierarchical note taking application, featuring rich text, syntax highlighting, images handling, hyperlinks, import/export with support for multiple formats, support for multiple languages, and more.\
### Recommendation
> It is recommended use for affective note and report making
### Information Gathering

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/2acf524e-2034-4471-b7e1-e6c2d84c18fe)

### Service Enumeration
> N.A.
### Penetration
> N.A
### Report – House Cleaning
> Same as above

## 2. Pipal
### High Level summary
> Pipal is a password analysis and research tool used to analyze password lists and patterns, providing insights into password security and helping identify common or weak passwords.
### Recommendation
> It is recommended to use when we have analyze certain wordlist that is manually created and test it's efficiency.
### Information Gathering 

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/28c31fbc-7cab-46b0-809d-037404100475)

### Service Enumeration
> N.A.
### Penetration
> N.A
### Report – House Cleaning
> Same as above

## 3. Cutycapt
### High Level summary
> CutyCapt is a small cross-platform command-line utility to capture WebKit’s rendering of a web page into a variety of vector and bitmap formats, including SVG, PDF, PS, PNG, JPEG, TIFF, GIF, and BMP.
### Recommendation
> Cutycapt is recommended for use when there is a need to capture screenshots of web pages from the command line.
### Information Gathering 
 
![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/b1373c0a-7e87-4c1b-91e5-d81a8cda031a)

### Service Enumeration
> N.A.
### Penetration
> N.A
### Report – House Cleaning
> Same as above










