# Threat Analysis By Wazuh Open Source 

### Make wazuh server configuration
```
- Enable the Vulnerability Detector module by modifying the Wazuh server configuration file at /var/ossec/etc/ossec.conf.
Set the value for the <enabled> tag to yes for the Vulnerability Detector module and for every operating system you intend to scan.
```

![image](https://github.com/jayshah17/Implementation-of-Cyber-Security-Lab/assets/76842630/0ca72d9d-41d0-435b-b389-6a64ef35ee28)

Add Vulnerability Detector Code in config file 

```
<vulnerability-detector>
    <enabled>yes</enabled>
    <interval>5m</interval>
    <min_full_scan_interval>6h</min_full_scan_interval>
    <run_on_start>yes</run_on_start>

    <!-- Ubuntu OS vulnerabilities -->
    <provider name="canonical">
      <enabled>yes</enabled>
      <os>trusty</os>
      <os>xenial</os>
      <os>bionic</os>
      <os>focal</os>
      <os>jammy</os>
      <update_interval>1h</update_interval>
    </provider>

    <!-- Debian OS vulnerabilities -->
    <provider name="debian">
      <enabled>yes</enabled>
      <os>buster</os>
      <os>bullseye</os>
      <os>bookworm</os>
      <update_interval>1h</update_interval>
    </provider>

    <!-- RedHat OS vulnerabilities -->
    <provider name="redhat">
      <enabled>yes</enabled>
      <os>5</os>
      <os>6</os>
      <os>7</os>
      <os>8</os>
      <os>9</os>
      <update_interval>1h</update_interval>
    </provider>

    <!-- Amazon Linux OS vulnerabilities -->
    <provider name="alas">
      <enabled>yes</enabled>
      <os>amazon-linux</os>
      <os>amazon-linux-2</os>
      <os>amazon-linux-2022</os>
      <os>amazon-linux-2023</os>
      <update_interval>1h</update_interval>
    </provider>

    <!-- SUSE OS vulnerabilities -->
    <provider name="suse">
      <enabled>yes</enabled>
      <os>11-server</os>
      <os>11-desktop</os>
      <os>12-server</os>
      <os>12-desktop</os>
      <os>15-server</os>
      <os>15-desktop</os>
      <update_interval>1h</update_interval>
    </provider>

    <!-- Arch OS vulnerabilities -->
    <provider name="arch">
      <enabled>yes</enabled>
      <update_interval>1h</update_interval>
    </provider>

    <!-- Alma Linux OS vulnerabilities -->
    <provider name="almalinux">
      <enabled>yes</enabled>
      <os>8</os>
      <os>9</os>
      <update_interval>1h</update_interval>
    </provider>

    <!-- Windows OS vulnerabilities -->
    <provider name="msu">
      <enabled>yes</enabled>
      <update_interval>1h</update_interval>
    </provider>

    <!-- Aggregate vulnerabilities -->
    <provider name="nvd">
      <enabled>yes</enabled>
      <update_interval>1h</update_interval>
    </provider>

  </vulnerability-detector>
```

In our wazuh-server we have to make changes in ossec.conf file

![image](https://github.com/jayshah17/Implementation-of-Cyber-Security-Lab/assets/76842630/7358b111-1d35-49bb-9ff7-a6c9d0e41eda)

It will start downloading all the Vulnerability databases of each and every OS

![image](https://github.com/jayshah17/Implementation-of-Cyber-Security-Lab/assets/76842630/b5457dc8-d01b-4625-ae5d-f1fe257712f9)

### Vulnerability Configuration for agents

Running vulnerability scans in Wazuh requires enabling the Vulnerability Detector module and setting the configuration for the scan.

![image](https://github.com/jayshah17/Implementation-of-Cyber-Security-Lab/assets/76842630/a113ce9e-e8e3-4ad0-8a93-33b7666d7a5b)

Change this conf with respect to the above screenshot:
This conf is present in both agent and server location in agent.conf

### Windows Agent

![image](https://github.com/jayshah17/Implementation-of-Cyber-Security-Lab/assets/76842630/74a4302c-8e14-4888-b211-8d6828f62dbc)

![image](https://github.com/jayshah17/Implementation-of-Cyber-Security-Lab/assets/76842630/9b79cd45-0327-4714-9b76-b6feebdc9bed)

![image](https://github.com/jayshah17/Implementation-of-Cyber-Security-Lab/assets/76842630/5dbbe90e-c374-4a5f-9828-5be1fa24f0e2)

As we open Wazuh server, it will show all the vulnerabilities after scanning the os 

Here is the graphical representation of all vulnerabilities and no. of vulnerabilities in terms of severity

![image](https://github.com/ananthan05/Cyber-Security-/assets/140697378/7d1c8688-a5c2-43b2-8379-02bb9c852b97)

If we click the critical vulnerability, we will able to analyse

![image](https://github.com/ananthan05/Cyber-Security-/assets/140697378/1353f830-29a4-497c-bbfc-379a85d43e94)

We have analysed Windows 11 also which is having 

![image](https://github.com/ananthan05/Cyber-Security-/assets/140697378/2c4e0e6a-33ba-4d3b-a6eb-17a6150e6232)

![image](https://github.com/ananthan05/Cyber-Security-/assets/140697378/9119724e-418f-40a8-a077-cfdf5fa36859)

CVE (common vulnerability and exposure) doesn’t only include the malicious software, the outdated software which are present in the system is also considered as a CVE

![image](https://github.com/jayshah17/Implementation-of-Cyber-Security-Lab/assets/76842630/6a5ef89f-f1e9-4a89-89eb-f971a51af028)


We can navigate to Mitre Attack

![image](https://github.com/ananthan05/Cyber-Security-/assets/140697378/1d85f6ea-f35e-4605-b161-8f82aeb00c56)

We can view Security Events as performing any authentication failure 

![image](https://github.com/ananthan05/Cyber-Security-/assets/140697378/11c9053d-0c0a-4d30-aaa3-456cd199d787)
