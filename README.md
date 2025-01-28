# Elastic-Lab

## Objective

The goal of this lab was to set up a virtual network using Kali Linux, VirtualBox, and utilize Elastic (SIEM) to detect and respond to potential threats. After integrating Elastic, I was able to query and search for specific threats and create alerts. I instructed the SIEM to ingest data and visualize it for stakeholders and team members.

### Skills Learned

- Kali Linux: Constructed a virtual network using Kali Linux. Various commands were used to identify network connections, such as `ifconfig` and `nmap`.
- Virtual Machine: By using a virtual machine, I was able to create a safe environment for testing and configuring networks. It also allowed me to ethically and safely use port scanning tools such as `nmap`.
- Port Scanning.
- Search queries by threat identifiers.
- Alert/Rule Creation.
- SIEM Integration.

### Tools Used

- Kali Linux.
- Virtual Box.
- Elastic (SIEM).
- `Nmap`.
- KQL (Kusto Query Language).

## Examples

<img width="1440" alt="Kali VMSetup" src="https://github.com/user-attachments/assets/2b14314e-9b9e-497b-8b75-103c51d692a1" />
I first initiated a virtual machine using the Kali Linux virtualization tool. By using the virtual machine, I was able to safely configure a network for a lab environment.

<img width="1440" alt="Elastic - Agent intergration - Agent enrollment" src="https://github.com/user-attachments/assets/8388aa82-43a4-4175-9c1d-3d6584a01adb" />
Next, I integrated Elastic (SIEM) with the Kali Linux session in the virtual machine.

<img width="1440" alt="Elastic - Kali nmap" src="https://github.com/user-attachments/assets/6a255f3e-c608-4f0b-bd94-5201ab93b1f2" />
After using `ifconfig` to identify the IP address assigned to the virtual network, I ran a series of `Nmap` scans to build a log of data on the network.

<img width="1440" alt="Elastic - Query nmap (KQL)" src="https://github.com/user-attachments/assets/d41a9054-2992-413d-8a84-fcd7ce525ba3" />
Then, within Elastic (SIEM), I performed a search query using KQL by filtering the logs for any commands containing `Nmap`.

<img width="1440" alt="Elastic - Nmap Rule" src="https://github.com/user-attachments/assets/96a9c3bf-b216-454f-b3d0-61895fc6872e" />
Following the KQL query, I created a rule in Elastic (SIEM) to notify of any `nmap` port scanning commands on the network I also increased the severity and risk score associated with the command.

<img width="1440" alt="Elastic - Data Visualization" src="https://github.com/user-attachments/assets/da324b53-dea0-4684-b11b-d6eca3962fe5" />
Finally, I used the logs collected from Elastic (SIEM) to visualize the threats on the network using graphs. The visual representation of the incident will be essential for communicating with stakeholders and team members.
