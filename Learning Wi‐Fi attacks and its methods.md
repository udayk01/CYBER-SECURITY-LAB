# 1. Learn the basic working of Wi-Fi and its types with various types of attacks on it.

## Basic Working of Wi-Fi

Radio Signals: Wi-Fi works by transmitting data over radio waves. Devices communicate in the Wi-Fi network by sending and receiving radio signals.

Access Points (APs) act as the central hub for Wi-Fi connections. They receive data from connected devices and transmit it to other devices on the network.

Network Identification: Wi-Fi networks are identified by their Service Set Identifier (SSID) which in simple terms is the network name.

Authentication and Encryption: When a device connects to a Wi-Fi network, it undergoes an authentication process to verify its identity. Wi-Fi protocols such as WPA2 or WPA3 are used to secure data transmissions over the network.

# Types of Wi-Fi

802.11 b/g/n: These are older Wi-Fi standards operating primarily in the 2.4 GHz frequency band. They offer relatively slower speeds compared to newer standards.

802.11 ac: Also known as Wi-Fi 5, this standard operates in both the 2.4 GHz and 5 GHz bands, providing faster speeds and improved performance compared to older standards.

802.11 ax: Also referred to as Wi-Fi 6, this is the latest Wi-Fi standard offering even higher speeds, lower latency, and improved efficiency, especially in high-density environments.

# Types of Wi-Fi Attacks

Eavesdropping (Passive Attacks): Attackers can intercept Wi-Fi signals to capture sensitive information such as passwords or financial data without actively engaging with the network.

Man-in-the-Middle (MITM) Attacks: In this type of attack, the attacker intercepts communication between two parties, potentially altering or eavesdropping on the data being transmitted.

Brute Force Attacks: Attackers attempt to crack Wi-Fi passwords by systematically trying all possible combinations until they find the correct one.

Evil Twin Attacks: Attackers set up rogue access points with the same SSID as a legitimate network, tricking users into connecting to it and potentially exposing their data.

Denial of Service (DoS) Attacks: Attackers flood a Wi-Fi network with an overwhelming amount of traffic, causing it to become unavailable to legitimate users.

WPS Vulnerabilities: Wi-Fi Protected Setup (WPS) is a feature that simplifies the process of connecting devices to a Wi-Fi network, but it can also introduce security vulnerabilities if not properly configured, allowing attackers to gain unauthorized access.

# Connecting the wireless adapter

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/08c81c76-342a-486b-8855-ae2224bf14e4)

# 2. Perform Wi-Fi fingerprinting. 

> We switch to sudo user and start wifite and scan the wi-fi network the around the area

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/f94dc5a5-b9d7-42e0-a3fb-a8aedfcb9f55)

> So we can see it shows all the available networks and how many clients are connected to it.

# 3. Create an Access point with any Wi-Fi encryption standard and start testing the security of that connection using any Wi-Fi security testing tools, which should include (Aircrack-Ng, Wifite, not limited). Try to capture the 4-way handshake using these methods.

> So our target here _Uday__Krishna_  so we will be attacking this network and it's using the wpa-p

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/8bd8f5cb-4259-4266-bbd3-7676318da391)

> Handshake is captured.

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/a5e5e956-e481-4929-b0a4-d69b88480c89)

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/9a73ad27-3c73-4129-8992-30c880abf6a8)

> It saves it as a pcap file and try to crack the password using the specified wordlist and we can see the key after cracking the i.e 123456789.

> So we try analyze the wireshark pcap that is saved along with this we can see that the 4 hand shake was captured.

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/c7cc0238-970d-46d7-9437-7a236b44ba3a)

# 4. After capturing the required files for testing, use dictionary generation and password cracking tools to crack the Wi-Fi password. 

> To generate a wordlist, we can use the crunch command.

`crunch 8 12 012345678abcdefghijklmnopqrstuvwxyz -o wordlist.txt`

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/0c931ae1-5c12-4b16-b7d3-4a510bbdd8ad)

# 5. Use Rouge AP (WifiPhisher) to create an Evil twin, perform a basic phishing attack using this rouge AP, and document the difference between the two attacks you have performed.  

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/08aa2e2f-4441-410a-9a2d-23541a3c7924)

> Then run WifiPhisher, we have to select which wifi fake have to create.

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/bff15bb3-9a8c-47d3-9f81-3d4e3529360f)

> We have to select what phishing we have to perform. I have selected auth login

![Screenshot 2024-03-03 095831](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/e66dbd8a-cdc8-4760-bd0a-750978630717)

![WhatsApp Image 2024-03-03 at 10 00 11_3bceacaa](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/39e1db73-8a2c-41af-bb09-803f3985fd48)

> So with help of WifiPhisher we created fake _Uday__Krishna_ wifi and we will try to connect ot it.

![WhatsApp Image 2024-03-03 at 10 04 28_65daf3a9](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/e0d819df-5787-4a8d-a226-572320fccd06)

> So as soon as the android device is connected it shows in the screen.

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/16a6443d-1c2c-4a54-9e81-0f870a8d16cd)

> And we enter the password in the website it reflected back when we close the tool.

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/40f20958-9c7c-412f-9c57-ad54db0b1469)

# 6. Learn the protocol level working of WPA3 and how it differs from WPA2. 

WiFi Protected Access 3 (WPA3) is the security protocol for WiFi networks succeeding WPA2. It enhances the security features and addresses some of the security vulnerabilities provided by WPA2.

Key Establishment and Authentication WPA3 introduced a handshake protocol called Simultaneous Authentication of Equals (SAE), which is based on DragonFly Key Exchange Protocol. This mitigated the vulnerabilities present in WPA2's four way handshake, hence making the WPA3 resistant to offline dictionary attacks and password guessing attacks.

Encryption WPA3 introduced support for Galois Counter Mode (GCMP). This offers similar security to Chaining Message Authentication Code Protocol (CCMP) but is more efficient in terms of processing power, which can improve battery life of the devices.

Protection against Brute Force Attacks WPA3 incorporated stronger protections against brute force attacks through the use of hash to group feature in the DragonFly handshake protocol. This made it significantly harder for attackers to guess the passphrase by making repeated brute force attempts.

Forward Secrecy WPA3 offers perfect forward secrecy ensuring that even if an attacker were to compromise the network's security key in the future, they would not be able to decrypt past data transmitted in the network.






