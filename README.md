# AlphaSecure 

***
[![Build Status](https://github.com/makandra/angular_xss/workflows/Tests/badge.svg)](https://github.com/Riya73/AlphaSecure)
<a href="https://github.com/Riya73/AlphaSecure" target="_blank">
    <img alt="Maintenance" src="https://img.shields.io/badge/Maintained%3F-yes-green.svg" />
  </a> 
  <a href="https://github.com/Riya73/AlphaSecure/blob/main/README.md" target="_blank">
    <img alt="Documentation" src="https://img.shields.io/badge/Documentation-yes-brightgreen.svg" />
  </a>
    



  
## AlphaSecure Working:
AlphaSecure framework designed with precaution to identify vulnerability of any web
application in such a way that it only looks for those vectors values which could cause a
vulnerability like SSL, open port, misconfiguration. We have divided all those attacking
vector to our different use of platform to check the vulnerability with respective tools.The Vulnerability detection and classifying types of vulnerability being identifies
with respective attacking vector with the respective supporting tools utilized. Whole process
is divided into three segments.


*** 
## Tools Used
***
  |Serial No.|Tool Name|  |Serial No.|Tool Name|    
  |:---------:|:--------|:--|:---------:|:--------:|
  |1|whatweb|  |2|nmap| 
  |3|golismero| |4|host| 
  |5|wget| |6|uniscan| 
  |7|wafw00f| |8|dirb| 
  |9|davtest| |10|theharvester|
  |11|xsser| |12|fierce|
  |13|dnswalk| |14|dnsrecon|
  |15|dnsenum| |16|dnsmap|
  |17|dmitry| |18|nikto|
  |19|whois| |20|lbd|
  |21|wapiti| |22|devtest|
  |23|sslyze| 
  ***
  
![image](https://github.com/Riya73/AlphaSecure/assets/86009160/6b0c2a45-3e87-4efb-8fa4-bfa495da66f0)

---
### Phase 1
* **Pre-processing Phase:**
  * **Network Check:** Ensures a stable connection to the target web application for efficient scanning and to avoid wasted time.
  * **URL Creation:** Constructs the appropriate URL for vulnerability scanning by:
    * Modifying the provided URL if necessary.
    * Verifying pre-installed tool requirements.
    * Encoding high-priority tools (marked with "1") for parallel execution.
* **Initialization:**
  * Generates proper URLs by appending paths to the base URL based on scanning needs.
  * Checks for pre-installed tools and their strengths for vulnerability identification.
  * Marks high-priority tools (marked with "1") for parallel execution.
* **Randomized Tool Selection:**
    * Selects tools at random from pre-verified options for various vulnerabilities.
    * Avoids time and resource limitations associated with individual tool selection.


### Phase 2
* **Threat Estimation and Scoring Phase** 
* **Completion Time Estimation:**
  * Calculates the expected time for each vulnerability scan based on:
    * Selected tool
    * Parallel processes running concurrently
    * Detection of attack vectors
* **Vulnerability Assessment:**
  * Analyzes the web server/application's response to attack vectors to identify vulnerabilities.
* **Threat Level Classification:**
  * **Uses the following frameworks to label threats:**
    * CVSS v2.0 scoring (Low, Medium, High)
    * MITRE ATT&CK framework threat levels
* **Threat Remediation:**
  * Provides recommendations for users to mitigate vulnerabilities, including:
    * Reference to the specific threat identified
    * Description of potential consequences if not addressed
* **After founding vulnerability in web application scanner will classify vulnerability in specific format:-**
  * [Responses + Severity (c - critical | h - high | m - medium | l - low | i - informational) + Reference for Vulnerability Definition and Remediation]
  * Here **c or critical** defines most vulnerability wheres **l or low** is for least vulnerable system 

#### Definitions:-
* > **Critical**:- *Vulnerabilities that score in the critical range usually have most of the following characteristics:
Exploitation of the vulnerability likely results in root-level compromise of servers or infrastructure devices.Exploitation is usually straightforward, in the sense that the attacker does not need any special authentication credentials or knowledge about individual victims, and does not need to persuade a target user, for example via social engineering, into performing any special functions.*
* > **High**:- *An attacker can fully compromise the confidentiality, integrity or availability, of a target system without specialized access, user interaction or circumstances that are beyond the attacker’s control. Very likely to allow lateral movement and escalation of attack to other systems on the internal network of the vulnerable application. The vulnerability is difficult to exploit. Exploitation could result in elevated privileges. Exploitation could result in a significant data loss or downtime.*
* > **Medium**:- *An attacker can partially compromise the confidentiality, integrity, or availability of a target system. Specialized access, user interaction, or circumstances that are beyond the attacker’s control may be required for an attack to succeed. Very likely to be used in conjunction with other vulnerabilities to escalate an attack.Vulnerabilities that require the attacker to manipulate individual victims via social engineering tactics.  Denial of service vulnerabilities that are difficult to set up. Exploits that require an attacker to reside on the same local network as the victim.  Vulnerabilities where exploitation provides only very limited access. Vulnerabilities that require user privileges for successful exploitation.*
* > **Low**:- *An attacker has limited scope to compromise the confidentiality, integrity, or availability of a target system. Specialized access, user interaction, or circumstances that are beyond the attacker’s control is required for an attack to succeed. Needs to be used in conjunction with other vulnerabilities to escalate an attack.*
* > **Info**:- *An attacker can obtain information about the web site. This is not necessarily a vulnerability, but any information which an attacker obtains might be used to more accurately craft an attack at a later date. Recommended to restrict as far as possible any information disclosure.*


* > |CVSS V3 SCORE RANGE|SEVERITY IN ADVISORY|
  > |:-------------------:|:--------------------:|
  > |0.1 - 3.9|Low|
  > |4.0 - 6.9|Medium|
  > |7.0 - 8.9|High|
  > |9.0 - 10.0|Critical|

#### Vulnerabilities

* After this scanner will show results which inclues: 
   * Response time 
   * Total time for scanning
   * Class of vulnerability
 
 
#### Remediation

* Now, Scanner will tell about *harmful effects* of that specific type vulnerabilility. 
* Scanner tell about sources to know more about the vulnerabilities. (websites).
* After this step, scanner suggests some *remdies* to overcome the vulnerabilites.

### Phase 3

* **Vulnerability Reporting and Patch Suggestions**
* **Vulnerability Logging:**
  * Creates a detailed record of vulnerabilities, including:
    * Severity level
    * Associated logs
    * Debug logs (if available)
* **Patch Recommendations:**
  * Suggests potential patches to mitigate vulnerabilities, incorporating:
    * References to the most reliable solutions
    * Remediation guidance (e.g., Apache logic4j vulnerability reference)
* **Log Management:V
  * Records and manages user system logs related to:
   * System errors
    * Other relevant events
* **Vulnerability Assessment:**
  * Analyzes identified vulnerabilities to suggest possible patches.
  * Prioritizes reliable solutions and remediation steps.
  

![image](https://github.com/Riya73/AlphaSecure/assets/86009160/b2319042-9721-4d43-b638-2f83fe22a09b)

## Use
```
Use Program as python3 Alpha.py (https or http) ://example.com
```
```
--help
--update
```


|Serial No.|Vulnerabilities to Scan|   |Serial No.|Vulnerabilities to Scan|
|:----------:|:---------------------:|---|:----------:|:---------------------:|
|1|IPv6||2|Wordpress|
|3|SiteMap/Robot.txt||4|Firewall|
|5|Slowloris Denial of Service||6|HEARTBLEED|
|7|POODLE||8|OpenSSL CCS Injection|
|9|FREAK||10|Firewall|
|11|LOGJAM||12|FTP Service|
|13|STUXNET||14|Telnet Service|
|15|LOG4j||16|Stress Tests|
|17|WebDAV||18|LFI, RFI or RCE.|
|19|XSS, SQLi, BSQL||20|XSS Header not present|
|21|Shellshock Bug||22|Leaks Internal IP|
|23|HTTP PUT DEL Methods||24|MS10-070|
|25|Outdated||26|CGI Directories|
|27|Interesting Files||28|Injectable Paths|
|29|Subdomains||30|MS-SQL DB Service|
|31|ORACLE DB Service||32|MySQL DB Service|
|33|RDP Server over UDP and TCP||34|SNMP Service|
|35|Elmah||36|SMB Ports over TCP and UDP|
|37|IIS WebDAV||38|X-XSS Protection|


### Installation

```
git clone https://github.com/Riya73/AlphaSecure.git
cd AlphaSecure/setup
python3 -m pip install --no-cache-dir -r requirements.txt
cd ../
python3 Alpha.py
```

### Screenshots of Scanner
![Screenshot from 2022-04-02 02-14-31](https://user-images.githubusercontent.com/86009160/161339137-3732c16e-5034-4f1c-9018-894e8c031ac0.png)
***

![Screenshot from 2022-04-02 02-26-22](https://user-images.githubusercontent.com/86009160/161340411-1d4157fe-daf8-4b2d-bfa8-c240601b2572.png)

***

### Real Time Result

![image](https://github.com/Riya73/AlphaSecure/assets/86009160/e18e9d35-98e7-410b-8651-9760a85d8102)
***

