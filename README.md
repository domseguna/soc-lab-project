# soc-lab-project
Real-time SOC detection Lab - Nmap, Hydra, Metasploit detected in Kibana (ELK)


---

## Attacks Simulated
| Attack              | Tool       | Events     | Detected In |
|---------------------|------------|------------|-------------|
| Network Recon       | Nmap       | 10+ logs   | <10s        |
| SSH Brute Force     | Hydra      | 1,100+ failures | Real-time   |
| Exploit Attempt     | Metasploit | 12 attempts| Immediate   |

---

## Challenges Solved 
| Challenge                                   | Solution                                   | Learning Outcome                         |
|---------------------------------------------|--------------------------------------------|------------------------------------------|
| No Splunk/Wazuh on Apple Silicon            | Chose **ELK Stack** (ARM-native)           | Modern SIEM selection                    |
| Nmap logs not showing                       | Forced SSH pre-auth logs + KQL wildcard    | Log enrichment & query optimization      |
| Filebeat stalling                           | Debug mode (`-d "publisher"`)              | Production pipeline troubleshooting      |

---

## Screenshots

**Real-Time Dashboard (3 Attacks)**  [Dashboard]
<img width="1065" height="625" alt="Screenshot 2025-11-18 at 2 59 11 pm" src="https://github.com/user-attachments/assets/ebdbd1f9-3c14-425e-8d34-2bfed7ad2536" />


**Nmap-Logs**  [Nmap Logs]
<img width="1744" height="1035" alt="Screenshot 2025-11-17 at 1 31 57 pm" src="https://github.com/user-attachments/assets/6fd56359-ee67-4092-a9b0-91c3f4081ca0" />

**Metasploit-Logs** [Metasploit TimeLine]
<img width="1065" height="621" alt="Screenshot 2025-11-18 at 5 08 35 pm" src="https://github.com/user-attachments/assets/f1ddf5b1-510c-4e70-9c71-06001ad0091c" />


**Hydra-Brute-Force0Volume** 
[Hydra Timeline]
<img width="1056" height="620" alt="Screenshot 2025-11-18 at 5 20 31 pm" src="https://github.com/user-attachments/assets/5607497a-e7b7-4d5a-b14c-9b85bf72a53b" />


**Full ELK Stack Running**  [ELK Home]
<img width="2056" height="1329" alt="Screenshot 2025-11-16 at 9 59 17 am" src="https://github.com/user-attachments/assets/f2e458d2-3cfe-40f8-9e57-b2d0cb5fb36f" />

**Kali Nmap Attack**  [Nmap Terminal]
<img width="640" height="482" alt="Screenshot 2025-11-18 at 5 32 24 pm" src="https://github.com/user-attachments/assets/c982e246-adfb-46c4-b7d8-6bbb03429051" />

**Kali Hydra Attack**  [Hydra Terminal]
<img width="642" height="174" alt="Screenshot 2025-11-18 at 5 33 30 pm" src="https://github.com/user-attachments/assets/69a2d38a-a59c-4fe1-ac7d-0d547a19aacd" />

**Kali Metasploit Attack** [Metasploit Terminal]
<img width="631" height="192" alt="Screenshot 2025-11-18 at 5 34 40 pm" src="https://github.com/user-attachments/assets/9f4be370-2da6-4050-9482-9c0c52982d3a" />


**UTM Lab Running**  
[UTM VMs]
<img width="1998" height="1279" alt="Screenshot 2025-11-18 at 5 44 15 pm" src="https://github.com/user-attachments/assets/72fbd888-0dd9-41d1-b02c-dfc5c1b4b048" />



Next Project (Already Started)
Python automation:  
- Auto Nmap scan  
- Parse Kibana logs  
- Send Slack alerts  
