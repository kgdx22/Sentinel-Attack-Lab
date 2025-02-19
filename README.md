# Sentinel-Attack-Lab

## Objective
  
Leverage hands-on experience in Azure security operations by deploying a honeypot VM, configuring Microsoft Sentinel, analyzing logs with KQL, and visualizing threats using Sentinel Workbooks for real-time attack detection and investigation.
 <br>
 <br>
## Skills Used

* Created a Windows 10 Virtual Machine in Azure, disabling Windows Firewall for honeypot functionality

* Configured Network Security Groups (NSG) for inbound traffic

* Used Event Viewer to analyze security logs

* Created a central log repository (LAW) and connected it to Sentinel instance

* Queried logs using KQL 

* Created watch list to derive attacker location/Created an attack map
 <br>

 ## Tools Used
* Kali Linux
  
* Microsoft Azure 
 
* Microsoft Sentinel


* VMware
   
* Windows Client

<br>
<br>

# Lab Setup 

A. Resource Group Visualization:

![Screenshot 2025-02-18 222458](https://github.com/user-attachments/assets/0d46b514-41d4-412c-b0c3-752a00cc534a)


B. Windows Virtual Machine:

<img width="507" alt="tgtdvc" src="https://github.com/user-attachments/assets/7004299f-82f2-4d83-87b1-3bc4a75887a2" />

C. Initial Log Query:

<img width="507" alt="ATTCKS" src="https://github.com/user-attachments/assets/42b7beaa-333a-4d4a-bb0e-7c5e17c8b1df" />

D. Detailed Log Query:

<img width="507" alt="loclog" src="https://github.com/user-attachments/assets/9731dbc6-3295-4512-8f0b-bc25a87e3a24" />

E: Attack Maps:

<img width="507" alt="bfmap" src="https://github.com/user-attachments/assets/d3e8f935-b438-4106-9ccb-29bea7b82531" />

+8hrs <img width="507" alt="8hrmap" src="https://github.com/user-attachments/assets/fe8f077b-56b5-4797-927c-98d7751edc88" />

+18hrs <img width="507" alt="18hrmap" src="https://github.com/user-attachments/assets/7d9d0947-1c5f-460b-96bf-17a89dfc085f" />





<br>
<br>
<br>

A: Map showing layout of Resource Group including virtual machine, virtual network, workbooks, DCR, LAW, and virtual network security group   

B: Windows Virtual Machine started inside of Azure with Windows Firewall turned off<br/>

C: Initial log query run in Azure that displays the first **561** failed login attempts into my virtual machine from attackers using EventID: 4625<br/>

D: A more detailed query that contains a watchlist allowing us to locate the attacker. Results now return in order of last event.<br/>

E: Progressing Attack Maps that display location and frequency of attackers targeting the virtual machine 

## Conclusion

I gained hands-on experience in log forwarding, enrichment with geo-location data, and visualizing attacks through Sentinel Workbooks. These skills enhanced my ability to perform threat detection, incident response, and SIEM management in a cloud-based environment. By turning off the firewall, the VM was intentionally left exposed to inbound traffic, making it an attractive target for attackers. This allowed for the collection of security event logs related to unauthorized access attempts, which were later analyzed in Microsoft Sentinel.
