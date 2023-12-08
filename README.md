# Burp Suite Project Documentation

This README.md file documents the steps I took during the Burp Suite project. The project involved setting up a proxy, launching a target, performing spidering, vulnerability scanning, brute force attacks, and exploiting a known SQL injection vulnerability using Burp Suite.

## Table of Contents

- [Setup Proxy](#setup-proxy)
- [Launch Target](#launch-target)
- [Fast & Hybrid Spidering](#fast--hybrid-spidering)
- [Vulnerability Scan](#vulnerability-scan)
- [Brute Force Attack](#brute-force-attack)
- [Exploit SQL Injection](#exploit-sql-injection)

## Setup Proxy

I did the following steps to set up the proxy:

1. I opened Burp Suite and navigated to the "Proxy" tab.
2. I configured my browser to use Burp Suite as a proxy.
   - I set the proxy settings to:
     - Proxy Type: HTTP
     - IP: [127.0.0.1]
     - Port: [8080]

![Proxy Setup](images/proxy_setup.png)

## Launch Target

1. I identified the target website for testing which was (http://testphp.vulnweb.com)
2. I launched the target website in my browser.
3. I observed the requests captured in Burp Suite.

![Launch Target](images/launch_target.png)

## Fast & Hybrid Spidering

1. Spidering wasn't available on my version of Burpsuite so I made use of the OWASP ZAP tool.
2. Using this tool, I was able to perform a vulnerability scan and also carry out Spidering on my test web application.
3. I used the "Spider" tool for fast and hybrid spidering(crawling) of the web application.

![Spidering](images/spidering.png)

## Vulnerability Scan

1. I used the "Scanner" tool in Burp Suite for vulnerability scanning.
2. I analyzed the scan results and identified potential vulnerabilities.
3. After analyzing the vulnerabilities, I identified a high-risk vulnerability which was SQL Injection amongst others.
![sqld details](images/sql_details.png)

![Vulnerability Scan](images/vulnerability_scan.png)

## Brute Force Attack
Using the "Reaper tool" in burpsuite
1. I navigated to the "Engagement Tools" in Burp Suite.
2. I used the "Intruder" tool for brute force attacks.
3. I configured payload sets and ran the attack.

![Brute Force](images/brute_force.png)

## Exploit SQL Injection

1. I identified a target page vulnerable to SQL injection.
2. I used the "SQLi" tool in Burp Suite to exploit the SQL injection vulnerability.

![SQL Injection](images/sql_injection.png)


## Conclusion

This project demonstrated the effectiveness of Burp Suite by identifying vulnerabilities in the online application (http://testphp.vulnweb.com). The practical experience highlights the significance of strong security protocols, and the knowledge acquired will benefit upcoming undertakings.

