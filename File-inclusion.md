# File Inclusion

`Summary :` An attacker can use Local File Inclusion (LFI) to trick the web application into exposing or running files on the web server. An LFI attack may lead to information disclosure, remote code execution, or even Cross-site Scripting (XSS). Typically, LFI occurs when an application uses the path to a file as input. If the application treats this input as trusted, a local file may be used in the include statement.

`Severity :` High

`Complexity :` Easy

`From :` Remote / External

`Steps to Reproduce:`

1. Attacker identfies a vulnerable injection point (parameter)
2. Attacker tries to read and execute the internal file
3. Attacker is successfully able to perfrom File Inclusion Attack

`Proof of Concept :`**Attached in the Video**

`Impact :` An Adversary can carry out Directory Listing to gain sensitive information from the target server

`Affected IP's :` IP Address Port[https://www.example.com/](https://www.example.com/) 443

`Recommendations :`The application should have proper whitelist of files and ignore every other filename and path.

References :[https://medium.com/@jonathanbouman/local-file-inclusion-at-ikea-com-e695ed64d82f](https://medium.com/@jonathanbouman/local-file-inclusion-at-ikea-com-e695ed64d82f)[https://hacker101.linuxsec.org/vulnerabilities/file_inclusion](https://hacker101.linuxsec.org/vulnerabilities/file_inclusion)

`Proof of Concept :`
