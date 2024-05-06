# AlphaSecure
# Scanner and Patcher [![Build Status](https://github.com/makandra/angular_xss/workflows/Tests/badge.svg)](https://github.com/Riya73/AlphaSecure)
***
<a href="https://github.com/Riya73/AlphaSecure" target="_blank">
    <img alt="Maintenance" src="https://img.shields.io/badge/Maintained%3F-yes-green.svg" />
  </a>
  <a href="https://github.com/Riya73/AlphaSecure/blob/main/README.md" target="_blank">
    <img alt="Documentation" src="https://img.shields.io/badge/Documentation-yes-brightgreen.svg" />
  </a>
    <a href="https://github.com/Riya73/AlphaSecure/blob/main/LICENSE" target="_blank">
    <img alt="License: MIT" src="https://img.shields.io/github/license/Riya73/AlphaSecure" />
  </a>
  
### This tools is very helpful for finding vulnerabilities present in the Web _**Applications**_.
*  A web application scanner explores a web application by crawling through its web pages and examines it for security vulnerabilities, which involves generation of malicious inputs and evaluation of application's responses. 
    *   These scanners are automated tools that scan web applications to look for security vulnerabilities. They test web applications for common security problems such as cross-site scripting (XSS), SQL injection, and cross-site request forgery (CSRF).
    *   This scanner uses different tools like nmap, dnswalk, dnsrecon, dnsenum, dnsmap etc in order to scan ports, sites, hosts and network to find vulnerabilites like OpenSSL CCS Injection, Slowloris, Denial of Service, etc.



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
  
## Working
---
### Phase 1
* User has to write:- "python3 Alpha.py (https or http) ://example.com"
* At first program will note initial time of running, then it will make url with "www.example.com".
* After this step system will check the internet connection using ping.
* Functionalities:-
* * To navigate to helper menu write this command:-  --help for update --update
* * If user want to skip current scan/test:-  CTRL+C
* * To quit the scanner use:-   CTRL+Z
* * The program will tell scanning time taken by the tool for a specific test.

### Phase 2
* From here the main function of scanner will start: 
* The scanner will automatically select any tool to start scanning.
* Scanners that will be used and filename rotation (default: enabled (1)
* Command that is used to initiate the tool (with parameters and extra params) already given in code 
* After founding vulnerability in web application scanner will classify vulnerability in specific format:- 
* * [Responses + Severity (c - critical | h - high | m - medium | l - low | i - informational) + Reference for Vulnerability Definition and Remediation]
* * Here **c or critical** defines most vulnerability wheres **l or low** is for least vulnerable system 

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
*  * Response time 
*  * Total time for scanning
*  * Class of vulnerability
 
 
#### Remediation

* Now, Scanner will tell about *harmful effects* of that specific type vulnerabilility. 
* Scanner tell about sources to know more about the vulnerabilities. (websites).
* After this step, scanner suggests some *remdies* to overcome the vulnerabilites.

### Phase 3

* Scanner will **Generate a proper report** including 
* * Total number of vulnerabilities scanned
* * Total number of vulnerabilities skipped
* * Total number of vulnerabilities detected
* * Time taken for total scan
* * Details about each and every vulnerabilites.
*  Writing all scan files output into SA-Debug-ScanLog for debugging purposes under the same directory
*  For Debugging Purposes, You can view the complete output generated by all the tools named SA-Debug-ScanLog.
  

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

