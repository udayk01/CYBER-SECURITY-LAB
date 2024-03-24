Use the tool NMAP [Command line only]to perform the below task. Run Wireshark in the background and capture only the necessary packets to showcase for the corresponding question.

## a) Explain the subnet and use the NMAP Command to scan the services for the whole subnet.

> A subnet, short for subnetwork, is a logical subdivision of an IP network. It allows for the division of a larger network into smaller, manageable parts. Subnetting is primarily used to improve network performance, security, and organization. Each device on a network is assigned an IP address, and subnetting helps in efficient routing of data packets within the network.

Command to scan entire subnet nmap -sV <subnet/CIDR notation>

> Victim Machine

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/6d1ae313-489c-4949-86c5-8ee96d109cfa)

> Attacker Machine

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/86d69854-2736-497f-ab37-c154fde009da)

## b) What is a firewall, and mention its types. Use the NMAP command to detect that a firewall protects the host

### Firewall 
* A firewall is a type of network security appliance that keeps an eye on and regulates inbound and outgoing network traffic in accordance with pre-established security rules. Its main goal is to defend devices and networks from malicious activity, assaults, and unauthorized access. It is possible to deploy firewalls using hardware, software, or a combination of the two. They function by looking at network traffic packets and comparing them to the administrator's preset rules or policies.
* A packet is permitted to get across the firewall if it matches a rule. If it doesn't fit any of the rules, it's either rejected or forwarded to another place for more examination.

### Types of Firewall
* Software firewall.
* Hardware firewall.
* Packet filtering firewall.
* Circuit-level gateway.
* Proxy service application firewall.

> The NMAP command to detect if a host is protected by a firewall. Here’s an example of how you might do this:
`nmap -sS -p- <target-ip>`

In this command:

> -sS option tells NMAP to perform a SYN scan, which is a type of stealth scan. -p- option tells NMAP to scan all 65535 ports. This command will send a TCP SYN packet to each port on the target host. If the port is open, the target will respond with a SYN/ACK packet. If the port is closed, the target will respond with a RST packet. If there is no response, or the packet is dropped, it’s likely that a firewall is protecting the host.

>> Victim machine when firewall is ON

![Screenshot 2024-02-20 201646](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/4f0fb1dd-e635-4501-87e8-a0060952a46b)

>> Attacker Machine

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/795d42a4-a7d8-45d5-a54f-2d40bee3483a)

There is no response. So it’s likely that a firewall is protecting the host

>> Victim Machine when firewall is off

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/8db9e651-eac1-460d-b1e6-0ae09082e6ba)

>> Attacker Machine

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/29cbf835-6fbf-4dad-a42d-0925fdcf30b9)

## c) Use the NMAP command to scan a network and determine which devices are running.

> Command -`nmap -sn <ip>/<CIDR> ` 

>> Attacker Machine

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/063c3a05-a8dc-42f5-a371-dbadff59339f)

## d) What are vertical and horizontal scanning?
* Horizontal scanning  sends requests to the same port on different hosts. Attackers use horizontal scanning to prepare for a mass attack.
* Vertical scanning sends requests to different ports on the same host. Attackers typically use vertical scanning to look for vulnerabilities in a preselected target.

## e) Use the NMAP command to scan multiple hosts. [HINT: Add hosts into a file and scan it].

>> Attacker Machine

WE need to add the ip address of the Victim Machine `192.168.192.131` to `/etc/hosts` file.

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/0c819508-cd99-4f66-b538-f6802a85dbd3)

## f) Use NMAP commands to export the output in XML format.

>> Attacker Machine

Use the `nmap -sV <target-ip> -oX name.xml`

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/2636a1a1-44f4-4336-b988-41176a6e17b6)

## g) Use the NMAP command to get OS information about a host. 

>> Attacker Machine

`nmap -O <target-ip>`

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/bd8f531e-8e75-49a8-8f0b-e65f462aa2be)

## h) Explain ping sweeping and Perform ping sweeping using Nmap

### Ping Sweep

> A method of network reconnaissance called "ping sweeping" is used to find out which IP addresses are active and reachable within a network. To find out which IP addresses are reachable and available, it entails sending a string of ICMP echo request messages, or pings, to a variety of addresses, usually in a sequential manner.

> Network administrators frequently use ping sweeping to map the network and find active hosts.

> Nmap command to perform ping sweep - `nmap -sn <network address>/<CIDR>`.

>> Attacker Machine

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/3b75e190-f5bb-413b-a779-525d29e84277)

## Try these below questions after completing the above commands. 

### 1. What is a web application firewall? How do you use Nmap to detect a WAF? Perform WAF fingerprint detection using NMAP.

* A Web Application Firewall (WAF) is a security tool designed to protect web applications from various attacks, such as SQL injection, cross-site scripting (XSS), and other common web exploits. WAFs monitor and filter HTTP traffic between a web application and the Internet, identifying and blocking malicious requests before they reach the application.

* To detect a WAF using Nmap, you can use its HTTP WAF fingerprinting feature. This feature sends specially crafted HTTP requests to the target web server and analyzes the responses to identify patterns that indicate the presence of a WAF.

sudo `nmap --script http-waf-fingerprint <target>`

>> Victim machine when firewall is ON

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/69d55705-e7fc-498c-9333-004ccaf34f95)

>> Attacker Machine

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/77f6dcb1-1d76-4b58-9d3f-59a4789d161c)

### 2. What is EXIF data? Try to find EXIF data of images on a website using NMAP NSE.
* EXIF DATA
-EXIF (Exchangeable Image File Format) data is a standard for storing metadata in image files, typically used by digital cameras and smartphones. This metadata can include information such as the camera model, exposure settings, GPS coordinates, and timestamps.

* -To find EXIF data of images on a website using Nmap NSE (Nmap Scripting Engine), you can use the http-exif-spider script. This script crawls a website, downloads images, and extracts EXIF data from them. Here's how you can do it:

> sudo `nmap --script http-exif-spider <website>`

>> Attacker Machine

Applying on Victim IP

![Screenshot 2024-02-20 211715](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/aaa84318-6010-4318-bcc7-27a18468af0a)

### 3. Use NMAP NSE to find all subdomains of the website.

> All the nse scripts are located in `/usr/share/nmap/scripts/`

sudo nmap --script dns-brute <website>

![Screenshot 2024-02-20 212259](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/4c303341-4069-42d6-bb19-7c441cdf5326)

![Screenshot 2024-02-20 212339](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/5ff48556-9bf5-4d57-8547-43b7da9b4aff)

### 4. Perform a vulnerability scan on the target host using NMAP NSE.

>> Command - `nmap -sV --script=vuln <target ip>`

>> Attacker Machine

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/8d471e07-bc28-4f6d-8dc9-0df03979f32e)




