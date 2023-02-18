# Homework 2

## 0) Summarize

## OWASP: OWASP 10 2021: Intelligence-Driven 

### A05:2021-Security Misconfiguration

Security misconfiguration is a prevalent vulnerability in web apps that can have severe impacts. 

Reasons for it include improper security setting configuration, unsecured default credentials, inadequate logging and monitoring, and exposed sensitive files and directories. The consequences may include unauthorized access to confidential information, data and functional tampering, and DDoS attacks. 

To avoid security misconfiguration, organizations should follow established security and configuration management practices, such as using strong passwords that are updated regularly, limiting access to sensitive data, constantly monitoring and logging security events, and updating all software and systems with the latest patches and security updates.

### A06:2021-Vulnerable and Outdated Components

+ Outdated and vulnerable components in an application can pose security threats such as well-known exploits, malware, and unaddressed vulnerabilities.
+ This risk can be reduced by conducting frequent scans to identify such components and updating them promptly.
+ Automated tools can aid in detecting these components and streamlining the update process.
+ Keeping tabs on component utilization and maintaining updated component licenses are critical for reducing security risks.
+ Staying informed about security risks through frequent review of component-related security alerts and bulletins.
+ Adopting secure development practices and conducting regular security assessments of the entire application can minimize these risks.



### a) A03:2021-Injection


Injection flaws are a prevalent and dangerous attack vector. They happen when an attacker injects malicious code into a vulnerable system, thereby gaining control or access to confidential information. 

Injection attacks can be executed in various forms, such as SQL injection, script injection, and command injection. The consequences of these attacks can range from data theft, system compromise, and service denial. To prevent injection attacks, it's crucial to implement input validation and sanitization, utilize parameterized queries, and limit access to sensitive information. 

Monitoring and detecting potential injection attacks, as well as having a well-prepared incident response plan, are also essential to quickly address any incidents that may occur.

## Darkent Diaries Podcast: EP 77: OLYMPIC DESTROYER

On the episode of Darken Diaries, the hosts delve into the Olympic Destroyer attack that took place during the 2018 Winter Olympics in Pyeongchang, South Korea. The attack aimed at the IT systems used in the Olympics, causing widespread disruption and making some critical systems inaccessible. The podcast provides an in-depth analysis of the threat actors behind the attack, the techniques used, the vulnerabilities exploited, and the impact of the attack. Additionally, the hosts offer insights on how the attack could have been prevented and how the attackers could have improved their approach.

The takeaway from this episode can be summarized as follows:

+ Impact: The Olympic Destroyer attack caused significant disruptions to the 2018 Winter Olympics, affecting critical systems like the official website and the scoreboard.

+ Mitigation: To guard against similar attacks, organizations should keep all software updated and patched, enforce robust password policies, and use cutting-edge security tools to detect and respond to threats.

+ Improvement: The attackers could have enhanced their attack by using more advanced tools and techniques to avoid detection, such as encryption or covering their tracks.

+ Threat Actors: The Olympic Destroyer attack was executed by an unknown, highly skilled and advanced group of threat actors.

+ Exploits: The attackers utilized a mix of exploits, such as exploiting unpatched software and spear-phishing emails, to gain access to the targeted systems.

+ Vulnerabilities: The attackers capitalized on various vulnerabilities in the targeted systems, including weak passwords and insecure networks.

The Olympic Destroyer attack serves as a warning for organizations to always be on high alert and proactive in protecting against cyber threats. By comprehending the threat actors, exploits, vulnerabilities, and impact, organizations can take measures to better defend against similar attacks and reduce the risk of compromise.


## CVE 

CVE is a dictionary of publicly known information security vulnerabilities and exposures. CVE is a service of the MITRE Corporation, a not-for-profit organization that operates federally funded research and development centers (FFRDCs).

More information about CVE can be found at
[Link to sources](https://www.redhat.com/en/topics/security/what-is-cve "CVE")) 

### CVE-2021-44228

CVE-2021-44228 is a security vulnerability that was assigned a unique identifier by the Common Vulnerabilities and Exposures (CVE) program, which is maintained by the non-profit organization MITRE.

This specific vulnerability is related to the Linux kernel, the core component of the Linux operating system. The vulnerability is related to the kernel's implementation of the Bluetooth subsystem and can allow a malicious attacker to cause a denial-of-service (DoS) condition or potentially execute arbitrary code with elevated privileges on the affected system.

The vulnerability affects Linux kernels version 5.11 and later, and it is recommended that users update their systems to a patched version to address the issue. This may involve installing a software update provided by the Linux distribution's vendor or recompiling the kernel with the appropriate patches.

More information about CVE-2021-44228 can be found at
[Link to sources](https://nvd.nist.gov/vuln/detail/CVE-2021-44228 "CVE-2021-44228")) 

# Sequel: SQLZoo
## 0) SELECT basics
1.
```
SELECT population FROM world
  WHERE name = 'Germany';
```
2.
```
SELECT name, population FROM world
  WHERE name IN ('Sweden', 'Norway', 'Denmark');
```
3.
```
SELECT name, area FROM world
  WHERE area BETWEEN 200000 AND 250000;
```

## 2 SELECT from World, from first subtask to 5 "France, Germany, Italy"
1.
```
SELECT name, continent, population FROM world
```
2.
```
SELECT name FROM world
  WHERE population >= 200000000;
```
3.
```
SELECT name, gdp/population FROM world
  WHERE population >= 200000000;
```
4.
```
SELECT name, population/1000000 FROM world
  WHERE continent = 'South America';
```
5.
```
SELECT name, population FROM world
  WHERE name IN ('France', 'Germany', 'Italy');
```
## b) A1 injection using Webgoat
A1 Injection is a type of security vulnerability that can occur in web applications. Injection flaws occur when untrusted data is sent to an interpreter as part of a command or query. The untrusted data can then be used to alter the intended command or query, allowing an attacker to inject malicious code into the system.

In the context of WebGoat, a deliberately vulnerable web application used for teaching and demonstrating web application security, A1 Injection refers to a specific type of injection flaw known as SQL Injection. This type of injection flaw occurs when user-supplied input is used in a SQL query without proper validation or sanitization, allowing an attacker to inject malicious SQL code into the query.

SQL injection attacks can be used to gain unauthorized access to sensitive data stored in a database, alter data, execute administrative functions, and cause denial-of-service conditions. To prevent SQL injection attacks, organizations should follow secure coding practices and validate and sanitize all user-supplied input before using it in SQL queries.

In the context of WebGoat, A1 Injection is used as a training exercise to demonstrate the dangers of SQL injection and to teach users about secure coding practices and mitigation techniques. By completing the A1 Injection exercise in WebGoat, users can gain a deeper understanding of the risks associated with SQL injection and how to defend against these types of attacks.

To be continued...







