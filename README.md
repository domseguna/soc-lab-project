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

**Real-Time Dashboard (3 Attacks)**  
![Dashboard](final-dashboard.png)

**Nmap Raw Logs**  
![Nmap Logs](nmap-raw-logs.png)

**Hydra Brute Force Volume**  
![Hydra Timeline](hydra-timeline.png)

**Full ELK Stack Running**  
![ELK Home](elastic-home.png)

**Kali Nmap Attack**  
![Nmap Terminal](nmap-attack.png)

**Kali Hydra Attack**  
![Hydra Terminal](hydra-attack.png)

**UTM Lab Running**  
![UTM VMs](utm-vms.png)

---

## Next Project (Already Started)
Python automation:  
- Auto Nmap scan  
- Parse Kibana logs  
- Send Slack alerts  

**Cyber Security Engineer in Training — Australia**  
Learning in public. One project at a time.

#CyberSec #ELKStack #Kibana #AppleSilicon #SecurityEngineering #Learning
