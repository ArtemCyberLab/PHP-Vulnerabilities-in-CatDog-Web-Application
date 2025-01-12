Project Title: "Exploit and Escalate: PHP Vulnerabilities in CatDog Web Application"

In this project, I explored vulnerabilities in a web application designed for viewing cat and dog images, built using PHP. The goal was to exploit these vulnerabilities to gain access to the server and execute commands.

Project Steps:
Port Scanning: Identified open ports 22 (SSH) and 80 (HTTP), indicating the web application was accessible.
Exploring the Webpage: Analyzed the URL format for image access and reviewed the source code.
Finding Hidden Directories: Used Gobuster to discover additional subdirectories.
LFI (Local File Inclusion) Analysis: Identified the potential to use the ?view= parameter for path traversal and access to system files.
Using PHP Filters: Applied the php://filter/convert.base64-encode filter to extract protected files.
Command Execution: Manipulated HTTP headers to execute commands on the server.
Privilege Escalation: Gained root access by utilizing the sudo -l command to escalate privileges.
Project Outcome:
I investigated several vulnerabilities, including LFI and remote code execution, and learned techniques for bypassing filters and escalating privileges.
