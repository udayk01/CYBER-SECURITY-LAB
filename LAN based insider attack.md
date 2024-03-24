## TOOL USED HERE
### ETTERCAP
Ettercap is a comprehensive, open-source network security tool used for analyzing, monitoring, and manipulating network traffic in a computer network. Originally developed for Unix-like operating systems, it has since been adapted for Windows as well. Ettercap operates as a man-in-the-middle (MITM) attack tool, allowing cybersecurity professionals, penetration testers, and ethical hackers to inspect and modify data as it passes through a network.

### Familiarization with tool

![image](https://github.com/ananthan05/Cyber-Security-/assets/140697378/c925e528-b037-416f-bbd9-e0d9f40a41e7)


So here we set the interface on which have to start sniffing and related attacks. Then we start sniffing on the interface.

## ARP Cache Poisoning
ARP spoofing is the process of linking an attacker’s MAC address with the IP address of a legitimate user on a local area network using fake ARP messages. As a result, data sent by the user to the host IP address is instead transmitted to the attacker.

### CAUSE OF ATTACK
The main cause of ARP spoofing attacks is the fundamental trust issue within the Address Resolution Protocol (ARP) itself. ARP is a network communication protocol that helps devices translate IP addresses, which are easy for humans to remember, into MAC addresses, which are the unique identifiers used by network devices.

### PREVENTION
We can prevent it by implementing the IDS(Intrusion detection system).
Using the Arp-spoof detecting software.

### PERFORMING THE ATTACK
First we discover all the hosts and choose the target on which we want to perform ARP spoofing attack.

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/1abc621e-b30d-4f61-b425-49dbefa1f168)

To find the Victim gateway.

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/4241f597-7659-4b8b-83fb-23fa7b4afafe)

So here the target is 192.168.142.131 and the target gateway is 192.168.142.2

Then we perform the ARP poisoning attack

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/02f628b4-26e2-432c-9bc2-7981d68fe0f3)

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/f0bd6060-d291-403c-b595-a3881cd8490a)

## Perform Denial of Service (DoS) attacks using ARP Cache Poisoning attacks.

The DoS (Denial of Service) attack plugin in ettercap is used to overload a target system or network with traffic in order to prevent the system or network from operating normally. This attack aims to prevent authorised users from accessing the target system or network. The way the DoS attack plugin in ettercap operates is by flooding the target with a lot of network traffic. Requests sent over the network, such as HTTP or DNS inquiries, might be considered genuine traffic.

As like the previous steps,

Scan for hosts

Add hosts as target (only the target ip & not the gateway ip)

Start arp poisoning the victim. 

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/6df7ca18-70cf-490a-a634-929c3e8f357b)

And now run the dos_attack plugin.

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/fc7375f3-1f07-4063-af9b-747d0209b941)

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/f30552dd-7865-4afa-b7ab-305fc9bcc61d)

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/8a06f62f-f8fa-4e87-8e5b-6ea9e93608b7)

IN victim Machine.

The victim becomes sluggish as soon as we enable the plugin since the target IP starts sending the victim a large number of packets. Therefore, the victim's web searches just never stop loading.

![Screenshot 2024-02-24 091733](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/e6d10b21-98c5-498b-b736-4c89bcce98c0)

## ICMP redirect (ARP poisoning)

Now, open Ettercap and start host scanning then, add victim’s IP to target 1 and default gateway to 
target 2 

![image](https://github.com/ananthan05/Cyber-Security-/assets/140697378/d4c90c7e-7de9-4813-87f4-d7dd9ac54dab)

![image](https://github.com/ananthan05/Cyber-Security-/assets/140697378/5b9cd8ab-bd3a-443d-a19b-a2f336a871ff)

After adding the respective hosts as targets start Arp poisoning. And after starting ARP poisoning simultaneously run the Wireshark in the background.

![image](https://github.com/ananthan05/Cyber-Security-/assets/140697378/d787c234-fab6-48a8-97fb-5d436270d516)

Choose icmp redirect and add the mac address and ip address of the default gateway.

![image](https://github.com/ananthan05/Cyber-Security-/assets/140697378/bbb3ba83-0c82-48b7-a39f-a899df73bbe1)

As we can see , the redirected message displayed in wireshark. 

![image](https://github.com/ananthan05/Cyber-Security-/assets/140697378/37f78c2e-63e4-4417-82b6-8e535415bb5f)
