# OWASP TOP 10 2025 Writeups:

## Task 1: Intro
1.	A01: Broken Access Control
2.	A07: Authentication Failures
3.	A09: Logging & Alerting Failures

## Task 2: IAAA

What does IAAA stand for?

Identity, Authentication, Authorisation, Accountability

## Task 3: A01:Broken Access Control

If you don't get access to more roles but can view the data of another users, what type of privilege escalation is this?

Ans: Horizontal

What is the note you found when viewing the user's account who had more than $ 1 million?
Ans: THM{Found.the.Millionare!}
 
## Task 4: A07: Authentication Failures
In this Challenge we get into admins user account by just changing the admin name with aDmiN and have a password that we choose and we get the flag

##FLAG: THM{Account.confusion.FTW!}
 <img width="940" height="494" alt="image" src="https://github.com/user-attachments/assets/d27cf2f5-751f-4b4a-8d0a-868ec8f766f3" />



#### It looks like an attacker tried to perform a brute-force attack, what is the IP of the attacker?

Correct Answer:  203.0.113.45

#### Looks like they were able to gain access to an account! What is the username associated with that account?

Correct Answer:  admin

#### What action did the attacker try to do with the account? List the endpoint the accessed.
Correct Answer:  /supersecretadminstuff 
 
Where a same ip address is being addressed for 3 to 4 times so they applied brute-force attack to get the admin details the endpoint they accessed is /supersecretadminstuff.

# OWASP Top 10 2025: Application Design Flaws

## Task 1: Introduction

AS02: Security Misconfigurations
AS03: Software Supply Chain Failures
AS04: Cryptographic Failures
AS06: Insecure Design

## Task 2: AS02 Security Misconfigurations

Security misconfigurations happen when systems, servers, or applications are deployed with unsafe defaults, incomplete settings, or exposed services. These are not code bugs but mistakes in how the environment, software, or network is set up.They create easy entry points for attackers.

<img width="1915" height="1145" alt="Screenshot 2026-03-20 003119" src="https://github.com/user-attachments/assets/52b8f983-3278-487f-8255-b16ebbffde71" />

## Task 3: AS03 Software Supply Chain Failures

In this Challenge from the python code we can able to run data = debug and then changing in burpsuite.

<img width="446" height="329" alt="image" src="https://github.com/user-attachments/assets/deb5543d-697d-4b3c-b60d-be178aab4f71" />


<img width="1919" height="1199" alt="Screenshot 2026-03-20 005354" src="https://github.com/user-attachments/assets/caf708cb-d942-4db7-8e84-81dabffe340b" />

## Task 4: AS04 Cryptographic Failures

<img width="1919" height="1055" alt="Screenshot 2026-03-20 010227" src="https://github.com/user-attachments/assets/0d4c6c4e-5a78-4e27-9860-b577aa83d84a" />

<img width="1911" height="1058" alt="Screenshot 2026-03-20 010510" src="https://github.com/user-attachments/assets/b5f7cf81-6e40-4bc2-9300-ee40f88f5d99" />

From that give secret key and and bits we can able to decrypt and retrive the flag

## Task 5: Insecure Design

<img width="1681" height="715" alt="Screenshot 2026-03-20 224849" src="https://github.com/user-attachments/assets/72985acb-2d78-4e0f-acd1-ba69583f3e9c" />

From this we can able to see that /messages and  /users and we try it out th flag is found

<img width="1914" height="1076" alt="Screenshot 2026-03-20 212736" src="https://github.com/user-attachments/assets/beb86d28-aaf0-4a50-88a7-721651d2cbb2" />

# OWASP Top 10 2025: Insecure Data Handling

## Task 1 :AS04 Cryptographic Failures

<img width="1906" height="1002" alt="Screenshot 2026-03-20 213552" src="https://github.com/user-attachments/assets/cf21820e-5ac8-4bc1-b347-f2c2044c22e8" />

the ciphertext is in the form of base 64 and it is decoded and when it is decrpyted with Key 1 and hence we can able to get the flag.

<img width="1782" height="938" alt="Screenshot 2026-03-20 214149" src="https://github.com/user-attachments/assets/4f70fd1f-8dc9-4b2a-b31f-cbb1fc7df98e" />

## Flag: THM{WEAK_CRYPTO_FLAG}

Task 3: A05 Injection


<img width="1914" height="1051" alt="Screenshot 2026-03-20 214240" src="https://github.com/user-attachments/assets/18c5e910-2d7b-4a13-b535-d19460039028" />

<img width="1916" height="1052" alt="Screenshot 2026-03-20 215247" src="https://github.com/user-attachments/assets/2a5082d7-d2c5-4ec7-8eb3-e7d3e933c483" />

SSTI Payload:
<img width="1916" height="1052" alt="Screenshot 2026-03-20 215247" src="https://github.com/user-attachments/assets/e880fd85-2914-4adc-a1c0-f0d640f23249" />

## Task 4: Software or Data Integrity Failures

<img width="1917" height="1000" alt="Screenshot 2026-03-20 215756" src="https://github.com/user-attachments/assets/03eb9168-c674-4d05-afda-a17d871793d5" />

when the base 64 is deslarize we can find the flag

## Flag :THM{INSECURE_DESERIALIZATION}








































