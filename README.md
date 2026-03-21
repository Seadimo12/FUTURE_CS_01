# 🔐 DVWA Vulnerability Assessment

## Overview
This project presents a comprehensive **web application vulnerability assessment** conducted on Damn Vulnerable Web Application (DVWA), a deliberately insecure platform used for cybersecurity training.

The objective of this assessment was to identify, analyze, and document common web security vulnerabilities, understand their real-world impact, and propose effective remediation strategies.

## Objectives
- Identify common web application vulnerabilities  
- Perform controlled exploitation (proof-of-concept)  
- Analyze security risks and impact  
- Provide remediation recommendations  
- Align findings with OWASP Top 10  

## Tools & Technologies
- DVWA (Damn Vulnerable Web Application)  
- XAMPP (Apache, MySQL)  
- Google Chrome  
- Chrome Developer Tools  

## Vulnerabilities Identified

### 1. Insecure Communication (HTTP)
- Application uses HTTP instead of HTTPS  
- Data transmitted in plaintext  

Evidence:  
![HTTP](screenshots/02_Baseline_Assessment/05_http_connection.png)

### 2. Insecure Session Cookies
- Missing **Secure** and **HttpOnly** flags  

Evidence:  
![Cookies](screenshots/02_Baseline_Assessment/06_insecure_session_cookie.png)

### 3. SQL Injection
- User input not sanitized  
- Database queries can be manipulated  
Evidence:  
![SQL Injection](screenshots/03_SQL_Injection/09_sql_injection_success.png)

### 4. Cross-Site Scripting (XSS)
- JavaScript executed in browser  

 Evidence:  
![XSS](screenshots/04_XSS/12_xss_alert_execution.png)

### 5. Command Injection
- System commands executed via input  

Evidence:  
![Command Injection](screenshots/05_Command_Injection/15_command_injection_success.png)

## OWASP Top 10 Mapping
This project aligns with the following OWASP Top 10 categories:

- Injection (SQL Injection, Command Injection)  
- Cross-Site Scripting (XSS)  
- Security Misconfiguration  

## Key Learnings
- Importance of input validation and sanitization  
- Risks of improper session management  
- Impact of insecure system configurations  
- Real-world exploitation techniques  
- Secure coding best practices  

## Conclusion
This project demonstrates practical experience in identifying and analyzing web application vulnerabilities within a controlled environment. The findings highlight the importance of secure development practices and proactive security testing.

## Author
Seadimo Bugqwangu

## Notes
This project was completed as part of a cybersecurity internship task and is intended for educational purposes only.
