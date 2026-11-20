# Exploring Your System's Security

## Task 1 --- List System Users

Run:

    cat /etc/passwd

### Screenshot

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/2d55d64c-8521-47a2-9828-7b5140379351" />


### Questions

1.  How many users exist on the system?
ans: 37
2.  Which accounts appear to be system accounts?
ans: root, daemon,bin,sys etc
3.  Why do operating systems create system accounts?
ans: System accounts are created to run background services and manage system process securely.

### Reflection

Explain why understanding system users is important for cybersecurity.
Understanding system user is important for cybersecurity because it helps identify who has access to the system.

## Task 2 --- Inspect Running Processes

Run:

    ps aux

### Screenshot

<img width="859" height="950" alt="image" src="https://github.com/user-attachments/assets/f848d038-3e87-4207-a4fd-2998ecc4cf84" />


### Questions

1.  Which processes are running as `root`?
ans: The processes with root in the user column are running as root.
2.  Why can processes running as root be dangerous?
ans: Root has administrator privileges. If a process has a security problem, it could affect the entire system.
3.  What could happen if a malicious program ran with root privileges?
ans: It could access sensitive files, change system setting, and compromise system security.

### Reflection

What did you learn about system processes and security?
I learned that system processes run under different users. Root has the highest privileges, so it is important to monitor processes and manage permissions carefully.

## Task 3 --- Identify Open Network Ports

Run:

    ss -tuln

### Screenshot


<img width="733" height="1009" alt="image" src="https://github.com/user-attachments/assets/a96b84b5-05d4-488b-a26f-ea0bfe3f4920" />

### Questions

1.  Which ports are open?
ans: The open listening ports are displayed in the Local Address: Port column.
2.  Which services appear to be listening?
ans: The command shows the listening portocols. Additional information may be needed to identify the exact services.
3.  Why might open ports represent a security risk?
ans: Open ports can allow network connections. If unnecessary or insecure services are listening, attackers may try to exploit them.

### Reflection

Explain the relationship between open ports and potential attack
surfaces.
Open ports represent potential attack surfaces. Monitoring open ports helps identify unnecessary network services and improve system security.
