## Tools Used

### ETTERCAP
> Ettercap is a comprehensive, open-source network security tool used for analyzing, monitoring, and manipulating network traffic in a computer network. Originally developed for Unix-like operating systems, it has since been adapted for Windows as well. Ettercap operates as a man-in-the-middle (MITM) attack tool, allowing cybersecurity professionals, penetration testers, and ethical hackers to inspect and modify data as it passes through a network.

### Familiarization with tool

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/c7a0e531-e76a-40fb-8f47-ed54fa99d34f)

>> So here we set the interface on which have to start sniffing and related attacks. Then we start sniffing on the interface.

## ARP Spoofing
> ARP spoofing is the process of linking an attacker’s MAC address with the IP address of a legitimate user on a local area network using fake ARP messages. As a result, data sent by the user to the host IP address is instead transmitted to the attacker.

### Cause of the attack
> The main cause of ARP spoofing attacks is the fundamental trust issue within the Address Resolution Protocol (ARP) itself. ARP is a network communication protocol that helps devices translate IP addresses, which are easy for humans to remember, into MAC addresses, which are the unique identifiers used by network devices.

### Prevention
> We can prevent it by implementing the IDS(Intrusion detection system). Using the Arp-spoof detecting software.

### Performing the attack
> First we discover all the hosts and choose the target on which we want to perform Arp spoofing attack.

![Screenshot 2024-01-29 221725](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/e4085e27-a118-4b02-89af-339f265d1767)

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/45070b80-16f8-4070-980b-bcade2e5b688)

>> So here the target is 192.168.142.2 and the target gateway is 192.168.142.131

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/628885ae-6624-444c-ba1e-1012efdf08b1)

>> After we set the targets perform ARP poisoning.

![Screenshot 2024-01-29 222544](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/0c8f6ae3-0a39-49dc-8205-a9178f3080f3)

>> In the Victim we are logging in on an HTTP 

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/38ecdcce-9026-4e99-be39-4832ee77876b)

>> As we can see the ETTERCAP has captured the username and password

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/6ba113c1-1baf-4c7e-a04a-b5eadf22cd0d)

### Splunk Logs
![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/6349199d-f15a-4857-8d00-33f837b73d6a)

## DNS Spoofing
> In a DNS spoofing attack, the attacker exploits vulnerabilities in the DNS resolution process to provide false information to a DNS resolver, which is responsible for translating domain names into IP addresses. The goal of DNS spoofing is to redirect users to a fraudulent website or to intercept sensitive information.

### Cause of the attack
> 1. Weaknesses in DNS Protocol: 
The DNS protocol itself can have vulnerabilities that attackers exploit. For example, if the DNS messages are not adequately protected, an attacker might inject false DNS responses into the system.
> 2. Lack of DNS Security Extensions (DNSSEC): 
DNSSEC is a suite of extensions to DNS designed to add an additional layer of security by signing DNS data with cryptographic signatures. If DNSSEC is not implemented or configured incorrectly, it can leave the DNS system susceptible to spoofing attacks

### Prevention
> To prevent DNS spoofing, organizations and individuals should implement several key measures. Firstly, deploy DNS Security Extensions (DNSSEC) to authenticate and verify the integrity of DNS data through cryptographic signatures. Additionally, configure DNS resolvers to limit open access, ensuring they respond only to authoritative queries.

### Performing the attack
> So to perform the attack we will be using the DNS spoof plugin that is available in Ettercap that we previously used.

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/5980928b-fc30-4e77-a7d8-1f813f747835)
![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/63b6c643-199d-4484-b3f6-393b1722b7d7)

>> We have to modify /etc/ettercap/etter.conf file and /etc/ettercap/etter.dns to change to perform the dns spoofing attack.


>> conf 

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/6e81b73e-a3bc-4de0-931d-44c9432e525e)

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/20ca5aaa-4793-47c5-9f5e-cd42ab2cef7b)

>> dns

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/ac7a901c-9c66-40df-a2cc-a06d57473340)

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/505c25ba-e6cf-4dc2-9532-643fd2246526)

So first start the dns spoofing using the plugin in the Ettercap plugins.

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/e4f67e86-62bd-425f-99f1-be2ba20ee407)

>> So we can see that we have dns_spoof plugin. After starting the dns spoofing we will use Arp poisoning again to make the attack successful.

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/09c7a1d8-b969-4e24-8780-1d05dc5e22d9)

>> Now if we try to navigate to the specified website it should goto Apache server running on the attacker machine

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/a5589686-8c9c-4dc2-ab94-72414b5a9998)

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/08645aed-a407-4f74-8362-39dca14c7d12)

> As we can see the attack was successful. 

### Splunk Logs

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/d29d0319-a936-4206-ac6b-c841845e3ceb)

So we can see in the splunk logs that we were redirected to other website that is a Apache server

























