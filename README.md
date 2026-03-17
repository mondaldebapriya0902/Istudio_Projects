# Istudio_Projects


Here we used the portswigger.net for solving the Cross-site Scripting (Xss) Labs. We use the access the lab and solve the labs and copy the script what we found in the solution statement.
then complete your labs.

Task 1

Cross-site scripting (XSS) is a web security vulnerability that allows an attacker to inject malicious client-side scripts (typically JavaScript) into web pages viewed by other users. The victim's browser executes this malicious code because it believes it came from a trusted source, enabling the attacker to bypass the same-origin policy and perform actions on behalf of the user, such as stealing session cookies, credentials, or sensitive data. 

Types of XSS Attacks
XSS vulnerabilities are typically categorized into three primary types, based on how the malicious script is stored and delivered to the victim's browser: 


Stored XSS (Persistent or Type I): This is generally the most severe type. The malicious script is permanently stored on the target server, for example, in a database, a comment field on a blog, or a forum post. The attack is triggered when a victim views the compromised page, and their browser automatically executes the malicious script. The attacker doesn't need to individually target victims, as anyone who accesses the affected page can be compromised.

Reflected XSS (Non-Persistent or Type II): In this type, the malicious script is part of the current HTTP request and is immediately "reflected" back in the web server's response, such as in an error message or search result. The data is not permanently stored by the application. The attacker must use social engineering (e.g., a malicious link in an email or social media post) to trick the victim into making the specific request that contains the payload.

DOM-based XSS (Type 0): This advanced form of XSS occurs entirely on the client-side within the victim's browser. The vulnerability exists in client-side JavaScript code that processes data from an untrusted source (like a URL fragment) in an unsafe way, usually by writing the data directly to the Document Object Model (DOM). The malicious payload never reaches the server, making it difficult to detect with server-side tools like web application firewalls (WAFs) or server logs. 


Task 2

:we work three investigation here
1) Authentication Bypass via SQL Injection,
2) ErrorBased / Boolean-Based SQL Injection and
3) Insecure Direct Object Reference (IDOR) / Broken Access Control
 first and second are vulnerable. Third isnot vulnerable.
