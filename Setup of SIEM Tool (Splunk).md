# Usage of SIEM Tool
* Log Analysis
* Security Investigation
* Log Monitoring and perform Incident Response
* Customized Dashboards can be created to analysis and investigate Logs
* Analyze data through patterns in a Analytical Manner

# Components of SIEM Tool:
* Forwarders: Collect Data from various sources and send it to Splunk Indexer
* Indexers: Store and Index the data for fast search and monitoring purpose
* Search Head: Interface for users to search, visualize, and analyze data.
* Splunk Apps/ Add-on: Plugin can be added for specific task
* Deployment Server: Manages configurations and updates across multiple Splunk Instances

# Architecture of SIEM Tool:
* Forwarders - collect data from sources.
* Indexers - store and index the data.
* Search Heads - provide the interface for users to interact with and analyze the indexed data.

# Advantages:
* Real-time Monitoring: Enables real-time monitoring and analysis of machine-generated data.
* Scalability: Distributed architecture allows horizontal scaling to handle increasing data volumes.
* Can add multiple Plug-ins so we can create our own customized dashboards
* Search Capabilities - Powerful search language (SPL) for complex queries and analytics.
* Large community support and numerous pre-built apps and integrations.

# Disadvantages:
* Licensing costs can be significant for large-scale deployments.
* Setting up and maintaining Splunk in a distributed environment can be complex.
* Requires significant hardware resources, especially for large deployments.
* There should be enough knowledge to work with search queries and other apps so effectively one can resolve the security breaches

# Features:
* Search Processing Language (SPL): Allows complex querying and analysis.
* Customized Dashboards: Enables creation of customizable visualizations and dashboards.
* Machine Learning Toolkit: Allows predictive analytics and anomaly detection.
* Data Ingestion: Supports various data sources and formats (logs, metrics, etc.).
* Security and Compliance: Provides features for securing data and meeting compliance requirements.

# Steps to Install and Configure Splunk
1. First of all install Splunk Enterprise on your host OS can be windows, kali Linux , Mac

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/d6c11bfd-3c86-4837-9b85-6f24aa126c23)

2. After Installing setup with Username and Password in Splunk Enterprise

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/673eda89-5b79-4216-96bb-efb71279c153)

3. Go into Settings and Configure the universal forwarder to send data to the Splunk Enterprise indexer by adding a new receiving port as 9997

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/6d1f3bd2-d406-49d8-8ecf-61eaf78c1945)

4. Now Start Installing Universal Forwarder in the system where you usually attack in my case i have done in kali linux

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/49449996-9c5c-4414-81b2-a6c665125826)

5. Now start with accepting license and set up username and Password

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/24c6514c-f8d4-4a1e-92c5-e9b88c5b005c)

6. Now Configure with 2 parameters
* ./splunk add forward-server :9997
* ./splunk set deploy-poll : (This you have to enable on Universal Forwarder where host ipaddress will be of the system on which universal forwarder is downloaded and management port no. you have to specify)

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/ec3d0b3e-2aab-43b6-92f8-28d3e5a79f57)

7. We have to write a command what to monitor

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/05b52ee0-dc95-4e96-b790-cf3b8d69facb)

8. Now restart the splunk

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/15016a53-9f39-46b6-bb64-1ea9f08613a2)

9. Realtime Logs on SIEM Tool:

![image](https://github.com/udayk01/CYBER-SECURITY-LAB/assets/52235763/20327a27-f34e-4afb-91c1-cfb78d753fa3)




